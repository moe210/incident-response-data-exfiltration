# Incident Response Investigation: Unauthorized Access & Data Exfiltration

## Overview

This project documents a simulated SOC incident involving unauthorized remote access, privilege escalation, PowerShell execution, and suspected data exfiltration from a finance workstation.

The investigation follows the incident from initial access through containment and focuses on identifying Indicators of Compromise (IOCs), analyzing security events, determining attacker activity, and assessing potential business impact.

## Incident Scenario

An external IP address generated multiple failed RDP authentication attempts against a finance workstation. A successful login was subsequently detected.

Following the successful authentication, suspicious activity was identified, including account creation, privilege escalation, PowerShell execution, unauthorized access to sensitive financial files, and outbound data transfer to an external IP address.

## Attack Flow

External IP

Multiple Failed Login Attempts
>
Successful Authentication
>
Unauthorized Access
>
New User Account Created
>
Privilege Escalation
>
PowerShell Activity
>
Sensitive Finance Files Accessed
>
Data Exfiltration
>
External IP Address

## Indicators of Compromise

- Source IP: 185.203.116.91
- Destination IP: 45.77.155.208
- Multiple failed authentication attempts
- Successful authentication
- Unauthorized user account
- Privilege escalation
- PowerShell execution
- Access to payroll and financial reports
- 118 MB outbound data transfer

## Incident Response Actions

1. Isolate the affected finance workstation.
2. Block the identified external IP address.
3. Disable the suspicious user account.
4. Reset compromised credentials.
5. Investigate PowerShell activity.
6. Review authentication and firewall logs.
7. Investigate the destination IP address.
8. Assess the scope of potential data exposure.

## Conclusion

The investigation identified a simulated compromise involving unauthorized access, privilege escalation, suspicious PowerShell activity, and suspected data exfiltration from a finance workstation.
