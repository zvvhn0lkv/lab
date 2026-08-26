# On-Call Playbook

Quick reference for common incidents.

## Pre-flight

- Check dashboards for alerts
- Acknowledge the page
- Join the bridge

## Initial triage

- `uptime` / `top` for load
- `df -h` for disk
- `journalctl -xe` for recent errors
- `tail -n 100 /var/log/syslog`

## Escalation

- If unresolved after 15 minutes, escalate to senior engineer.
