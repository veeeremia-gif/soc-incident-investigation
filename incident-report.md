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

## 9. Conclusion
