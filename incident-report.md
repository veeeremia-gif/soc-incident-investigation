# Incident Report

## 1. Executive Summary

The organization's login system experienced a security incident involving a suspected account compromise. An attacker attempted to access the system using the credentials of an employee named John Smith. After several failed login attempts, a successful login was detected from a suspicious IP address. The unusual authentication activity alerted the security team and triggered an investigation into the potentially compromised account.


## 2. Incident Details

* **Incident Type:** Suspected Brute-Force / Credential Compromise
* **Affected User:** John Smith
* **Suspicious IP Address:** 185.220.101.45
* **First Suspicious Activity:** 09:02:17 — Failed login attempt from 185.220.101.45
* **Current Status:** The security team has disabled the affected user account and initiated an investigation.


## 3. Detection

The security monitoring system detected unusual activity involving the account of the employee John Smith. The suspicious activity was detected at 09:30:05 after multiple failed login attempts followed by a successful login from the suspicious IP address 185.220.101.45. The activity was considered suspicious because the login originated from a different IP address than the employee's earlier legitimate login. The security team was alerted and began investigating the potentially compromised account.



## 4. Investigation Findings

The login attempts indicate that the organization's system may have been exposed to a potential attack. The IP address 185.220.101.45 is considered suspicious because multiple failed login attempts originated from this address within a short period of time. A successful login was subsequently detected from the same IP address. After the successful login, unusual activity was observed, including access to and download of the sensitive file customer_database.xlsx. This indicates a potential compromise of the user's credentials and possible unauthorized access to sensitive customer information.


## 5. Indicators of Compromise

The investigation identified several indicators that may point to a compromise of the John Smith user account:

* **Suspicious IP Address:** 185.220.101.45 was associated with multiple failed login attempts and a subsequent successful login.
* **Failed Login Attempts:** Four failed login attempts were recorded between 09:02:17 and 09:03:02.
* **Successful Login:** A successful login from the suspicious IP address was detected at 09:15:47.
* **MFA Not Enabled:** Multi-Factor Authentication was not enabled for the affected account.
* **Unusual Location:** The security monitoring system detected a login from an unusual location.
* **Sensitive File Access:** The account accessed `customer_database.xlsx`.
* **File Download:** `customer_database.xlsx` was subsequently downloaded.
* **Security Alert:** The security monitoring system generated an alert at 09:30:05 due to suspicious activity involving the affected account.

The combination of these indicators suggests a potential credential compromise and unauthorized access to sensitive company information. Further investigation is required to determine whether the customer data was transferred outside the organization or misused.


## 6. Impact Assessment

The security incident may have resulted in the compromise of the user's account. A successful login was detected from the suspicious IP address 185.220.101.45, and Multi-Factor Authentication (MFA) was not enabled on the account. Following the successful login, the potentially unauthorized user accessed and downloaded the customer_database.xlsx file. This indicates a potential exposure of sensitive customer information and requires further investigation to determine whether any data was exfiltrated or misused.


## 7. Containment Actions

In addition to disabling the affected account, the security team should take the following containment actions:

1. Reset the user's password to prevent further unauthorized access.
2. Terminate all active sessions associated with the compromised account.
3. Block or restrict the suspicious IP address 185.220.101.45 after validating the associated activity.
4. Enable Multi-Factor Authentication (MFA) for the affected account and require MFA for all users where possible.
5. Review authentication and file-access logs for additional suspicious activity.
6. Investigate whether customer_database.xlsx was transferred outside the organization.


## 8. Recommendations

The organization should strengthen its security controls to reduce the risk of similar incidents in the future. Key measures include implementing Multi-Factor Authentication (MFA), providing regular phishing awareness training, improving email security and monitoring, applying the Principle of Least Privilege, and strengthening password and access-control policies.

Detailed recommendations are documented in the [Recommendations](recommendations.md) document.

## 9. Conclusion

The investigation identified several indicators of a potential compromise of the John Smith user account. Multiple failed login attempts from the suspicious IP address 185.220.101.45 were followed by a successful login from the same address. After the successful login, the account accessed and downloaded the customer_database.xlsx file, which may contain sensitive customer information. The fact that Multi-Factor Authentication was not enabled increased the risk of unauthorized access to the account and company data.

The security team responded by disabling the affected account and beginning an investigation into the suspicious activity. Further analysis should determine whether the downloaded file was transferred outside the organization and whether any other systems or accounts were affected. To prevent similar incidents in the future, the organization should implement MFA, strengthen email security and monitoring, provide regular phishing awareness training, and apply the Principle of Least Privilege.

