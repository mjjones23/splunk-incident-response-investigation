# Splunk Incident Response Investigation

## Project Overview

This cybersecurity project demonstrates how Splunk can be used to investigate suspicious authentication activity, identify potential brute-force attacks, and analyze possible unauthorized access.

The investigation was conducted using simulated Windows security event logs in a controlled lab environment.

## Tools and Technologies

- Splunk Enterprise
- Search Processing Language (SPL)
- Windows Security Event Logs
- Security Incident Investigation
- Data Visualization and Dashboard Creation

## Investigation Findings

On October 15, 2026, simulated security logs revealed suspicious authentication activity involving the account `j.smith`.

Key findings:

- 8 failed login attempts from `203.0.113.25`
- A successful login from the same IP address following the failures
- Subsequent access to an application server
- 10 failed and 5 successful authentication events overall
- A separate source IP with 2 failed administrator login attempts

These findings suggest a possible brute-force or password-guessing attempt followed by successful authentication. The evidence does not independently confirm unauthorized access.

## Splunk Dashboard

Created five dashboard panels:

1. Failed Login Attempts by IP
2. Suspicious Login Activity Timeline
3. Successful Logins After Failed Attempts
4. Authentication Events by Status
5. Suspicious IP Investigation Details

## Dashboard Screenshots

![Splunk Dashboard Part 1](incident%20response%20investigation-1.png)

![Splunk Dashboard Part 2](incident%20response%20investigation-2.png)

## Recommended Security Actions

- Investigate suspicious authentication sources
- Verify whether successful logins were authorized
- Review affected account activity
- Consider account lockout policies and multifactor authentication
- Monitor for additional suspicious access attempts
- Document findings and escalate confirmed incidents

## Skills Demonstrated

- Security Information and Event Management (SIEM)
- Log Analysis
- Threat Detection
- Incident Response
- SPL Queries
- Security Dashboard Development
- Cybersecurity Documentation

## Investigation Report

See `Splunk_Incident_Response_Investigation_Report.pdf` in this repository for the full simulated incident investigation report.

**Disclaimer:** This project uses simulated security events and documentation IP addresses for educational and portfolio purposes.
