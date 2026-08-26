# On-Call Response Checklist

A quick reference for initial incident response.

## Triage
- [ ] Acknowledge the alert
- [ ] Determine severity and impact
- [ ] Identify the affected service

## Investigate
- [ ] Check dashboards and logs
- [ ] Look for recent deploys/config changes
- [ ] Correlate with upstream/downstream dependencies

## Mitigate
- [ ] Roll back if recent change is suspected
- [ ] Scale out or failover if capacity-related
- [ ] Communicate status to stakeholders

## Follow up
- [ ] Write a short incident summary
- [ ] Create/update tracking ticket
- [ ] Schedule a blameless review if needed
