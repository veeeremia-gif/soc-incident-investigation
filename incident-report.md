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

## 7. Containment Actions

## 8. Recommendations

## 9. Conclusion
