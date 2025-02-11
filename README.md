# CVE Request: Privilege Escalation in Nagios Network Analyzer  

## Overview  
A **Broken Access Control** vulnerability in **Nagios Network Analyzer 2024R1.0.3** allows low-privilege users to perform administrative actions, such as stopping system services and deleting critical resources. This flaw compromises **system integrity** and **availability**, leading to potential operational disruptions.  

## Affected Product  
- **Product:** Nagios Network Analyzer  
- **Version:** 2024R1.0.3  
- **Vulnerability Type:** Broken Access Control  

## Impact  
- **Availability Risk:** Unauthorized system shutdowns or resource deletions may cause service disruptions.  
- **Integrity Risk:** A low-privilege user can perform unauthorized modifications, leading to unintended consequences.  
- **Operational Impact:** Could result in downtime, data loss, and reputational damage.  

## CVSS Score  
- **CVSS v3.0:** `AV:N/AC:L/PR:L/UI:N/S:U/C:N/I:L/A:L`  
- **Severity:** Medium  

## Root Cause  
The application lacks proper authorization enforcement, allowing users with **Read-Only** permissions to execute high-impact administrative operations.  

## Resolution Status  
- **Changelog Reference:** [Nagios Changelog](https://www.nagios.com/changelog/#network-analyzer)  

## Disclosure Timeline  
- **January 10, 2025:** Acknowledgment from Nagios; credited as the first reporter.  
- **January 21, 2025:** Fix released.  
- **February 4, 2025:** Public disclosure permitted.  

## References  
- [MITRE CVE Entry - Pending]  
- [Nagios Changelog](https://www.nagios.com/changelog/#network-analyzer)  

## Credits  
- **Discovered by:** Harshal Tembhurne  

## Note  
This repository is created solely for submitting a **CVE request**. It provides the necessary details for vulnerability tracking while adhering to responsible disclosure practices.  
