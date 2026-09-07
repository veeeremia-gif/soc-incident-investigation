# Indicators of Compromise (IoCs)

## Identified Indicators of Compromise

## 1. Suspicious IP Address

**IP Address:** `185.220.101.45`

This IP address is considered suspicious because multiple failed login attempts and a subsequent successful login were detected from the same address.

## 2. Failed Login Attempts

Four failed login attempts were detected from `185.220.101.45`:

* `09:02:17` — Failed login
* `09:02:24` — Failed login
* `09:02:31` — Failed login
* `09:03:02` — Failed login

The repeated failed login attempts within a short period may indicate a brute-force or credential-based attack.

## 3. Successful Login

At `09:15:47`, a successful login was detected for the account `john.smith` from the suspicious IP address `185.220.101.45`.

The successful login following multiple failed attempts increases the likelihood that the user's credentials may have been compromised.

## 4. Missing Multi-Factor Authentication

At `09:16:03`, the logs indicated that Multi-Factor Authentication (MFA) was not enabled for the affected account.

The absence of MFA may have made it easier for an unauthorized user to access the account using compromised credentials.

## 5. Unusual Location

At `09:17:21`, the security monitoring system detected an unusual login location associated with the `john.smith` account.

This activity requires further investigation to determine whether the login was legitimate or unauthorized.

## 6. Suspicious File Access

At `09:18:44`, the affected account accessed:

`customer_database.xlsx`

The file may contain sensitive customer information and therefore represents a potentially significant security concern.

## 7. Suspicious File Download

At `09:21:12`, the same file was downloaded:

`customer_database.xlsx`

The download may indicate unauthorized access to sensitive information. Further investigation is required to determine whether the file was transferred outside the organization.

## 8. Security Alert

At `09:30:05`, the security monitoring system generated an alert for suspicious activity involving the `john.smith` account.

This alert triggered the security team's investigation.

## Summary of Identified IoCs

| IoC                                 | Evidence                              | Significance                           |
| ----------------------------------- | ------------------------------------- | -------------------------------------- |
| `185.220.101.45`                    | Multiple failed and successful logins | Suspicious source IP                   |
| 4 failed logins                     | 09:02:17–09:03:02                     | Possible brute-force/credential attack |
| Successful login                    | 09:15:47                              | Possible account compromise            |
| MFA disabled                        | 09:16:03                              | Increased account risk                 |
| Unusual location                    | 09:17:21                              | Possible unauthorized access           |
| `customer_database.xlsx` accessed   | 09:18:44                              | Potential sensitive-data exposure      |
| `customer_database.xlsx` downloaded | 09:21:12                              | Possible unauthorized data transfer    |
| Security alert                      | 09:30:05                              | Incident detected                      |

## Conclusion

The combination of repeated failed login attempts, a successful login from a suspicious IP address, missing MFA, unusual login activity, and subsequent access and download of a potentially sensitive file indicates a possible compromise of the `john.smith` account. Further investigation is required to determine the full scope of the incident and whether any sensitive information was exfiltrated.


