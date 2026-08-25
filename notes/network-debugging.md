# Network Debugging Notes

Date: 2026-08-25

Quick reference for common network issues.

- Check listening ports: `ss -tulpn`
- Trace route: `mtr -rwc 5 8.8.8.8`
- DNS lookup: `dig +short example.com`
- Packet capture: `tcpdump -ni eth0 port 53`

Remember: always check /var/log/syslog for kernel messages.
