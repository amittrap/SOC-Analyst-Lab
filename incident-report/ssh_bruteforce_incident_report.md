# Incident Report: SSH Brute-force Attack

## Incident Summary
Multiple failed SSH login attempts detected from a single external IP.

## Timeline
- Detection: SIEM alert triggered
- Analysis: Confirmed brute-force pattern
- Containment: IP blocked

## Impact
No successful compromise detected.

## Mitigation
- Firewall IP blocking
- SSH hardening
- Continuous monitoring

## Lessons Learned
- Enable MFA where possible
- Improve alert thresholds
