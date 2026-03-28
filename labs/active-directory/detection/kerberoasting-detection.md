# Kerberoasting Detection

## Objective
Understand how to detect Kerberoasting activity in an Active Directory environment.

## Indicators
- Unusual number of Kerberos service ticket requests (TGS)
- Requests for multiple service accounts in a short time
- Activity coming from a non-administrative user

## Logs to monitor
- Windows Event ID 4769 (Kerberos Service Ticket Request)

## Detection approach
Monitoring abnormal patterns in ticket requests can help identify potential Kerberoasting attempts.

## Mitigation actions
- Investigate suspicious accounts
- Reset compromised service account passwords
- Enforce strong password policies
