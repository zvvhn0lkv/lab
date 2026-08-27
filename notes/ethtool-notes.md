# ethtool notes

Quick reference from the Aug 26 NIC troubleshooting session.

## Link / speed

```bash
ethtool eth0
```

Check for Speed, Duplex, and Link detected.

## Driver info

```bash
ethtool -i eth0
```

Useful for firmware version before updating.

## Stats

```bash
ethtool -S eth0 | grep -E 'rx_.*err|tx_.*err'
```

Look for drops/errors after an incident.

## Ring buffer

```bash
ethtool -g eth0
```

If drops are high, try increasing RX ring size:

```bash
ethtool -G eth0 rx 4096
```

Note: not persistent across reboots.

## Offloads

```bash
ethtool -k eth0
```

Disable/verify offloads when testing packet captures:

```bash
ethtool -K eth0 gro off gso off tso off
```