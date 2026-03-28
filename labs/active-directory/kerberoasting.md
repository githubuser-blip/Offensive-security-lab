# Kerberoasting

## Objective
Understand how Kerberoasting works in an Active Directory environment and why service accounts with weak passwords are a security risk.

## Description
Kerberoasting is an attack technique that targets service accounts associated with Service Principal Names (SPNs).  
An authenticated domain user can request a service ticket for those accounts and attempt to crack it offline.

## Why it matters
This attack can lead to credential exposure and privilege escalation if service accounts use weak or reused passwords.

## Lab context
This scenario is being studied in a controlled lab environment for educational and defensive purposes.

## Key points
- Targets accounts with SPNs
- Requires domain authentication
- Relies on offline password cracking
- Helps identify risky service account configurations

## Mitigation ideas
- Use strong, long passwords for service accounts
- Prefer managed service accounts when possible
- Reduce unnecessary SPNs
- Monitor suspicious Kerberos ticket requests
