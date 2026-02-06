# Alert Investigation: SSH Brute-force Attempt

## Alert Name
Multiple SSH Authentication Failures

## Alert Source
SIEM (Linux authentication logs)

## Severity
High

## Investigation Steps
1. Identified repeated failed login attempts
2. Correlated events by source IP
3. Verified no successful login occurred

## Verdict
True Positive

## Response Taken
- IP blocked
- Incident escalated to SOC lead
- Incident documented

