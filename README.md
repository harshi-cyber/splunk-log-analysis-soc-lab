# Log Analysis & SOC Dashboards (Splunk)

This project demonstrates SOC-style security monitoring using Splunk SIEM.
Multiple log sources were analyzed to detect suspicious activity and visualize threats through dashboards.

## Objective
To monitor security logs, detect abnormal behavior, and build dashboards aligned with real-world SOC use cases.

## Environment & Log Sources
- Windows Security Logs
- Linux Authentication Logs
- Firewall Logs
- Apache Web Server Logs
(All logs were simulated for training purposes)

## Detection Use Cases (SPL)

### Windows Logs
- Failed login attempts (Event ID 4625)
- Brute-force detection based on repeated failures
- Suspicious process execution (PowerShell, cmd)
- New user account creation

### Linux Logs
- Failed SSH login attempts
- SSH brute-force activity
- Invalid user login attempts
- Sudo command usage

### Firewall Logs
- Denied connections
- Top attacking IP addresses
- Targeted destination ports
- Attack reason analysis

### Apache Web Logs
- HTTP status codes (401, 403, 500)
- Suspicious access to admin pages
- Most accessed URLs
- Top client IP addresses

## SOC Dashboards
- Failed login attempts by source IP
- Suspicious process execution trends
- SSH brute-force activity
- Firewall deny events and attacking IPs
- Web server error and access patterns

## SOC Analyst Actions
- Investigated repeated authentication failures
- Correlated activity across Windows, Linux, Firewall, and Web logs
- Identified high-risk IPs, ports, and processes
- Prioritized alerts for further investigation

## Key Learnings
- Brute-force attacks can be detected through correlation
- Firewall logs reveal targeted services and attacker behavior
- Web logs help identify abnormal access patterns
- Dashboards improve SOC visibility and response efficiency

## Conclusion
This project provided hands-on SOC experience in log monitoring, detection engineering, and dashboard analysis using Splunk SIEM.
