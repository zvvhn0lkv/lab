# On-call Triage Notes

Quick reference for the 3 AM pages.

## First 5 minutes

1. Check dashboards for obvious spikes.
2. Look at recent deploys in the last hour.
3. Tail logs for the affected service.
4. Ping the team channel if it's not a known issue.

## Common alerts

- **High CPU**: Usually a runaway query. Check slow logs.
- **5xx spike**: Rollback last deploy if needed.
- **Disk full**: Clear old backups, then alert the team.

## Escalation

- 10 min: no root cause → loop in senior on-call.
- 30 min: still down → page the incident commander.

Keep this updated as we learn new failure modes.