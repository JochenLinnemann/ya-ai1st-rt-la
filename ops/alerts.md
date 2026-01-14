# Alerts

## Alerting Philosophy
- Alerts should be actionable
- Alerts should indicate user impact
- Avoid alerts on symptoms alone

## Alert Types
- Availability
- Latency
- Error rate
- Resource exhaustion

## Escalation
Describe on-call rotation and escalation paths.

## Example Alert

Name: High Error Rate  
Trigger: >5% errors over 5 minutes  
Impact: Users likely affected  
Action: Check recent deploys, roll back if needed
