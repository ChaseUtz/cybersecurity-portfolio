# Splunk Security Dashboard

## Overview

This project documents the creation of a Splunk dashboard used for monitoring security events within my SOC homelab.

The dashboard provides visibility into Windows event logs, Sysmon telemetry, and endpoint activity collected through Splunk Universal Forwarder.

## Environment

### Log Sources

- Windows 11 Endpoint
- Sysmon
- Splunk Universal Forwarder

### SIEM Platform

- Splunk Enterprise
- Ubuntu Server

## Dashboard Goals

- Monitor endpoint activity
- Visualize event volume
- Detect failed logon attempts
- Observe process creation events
- Support threat hunting activities

## Searches Used

### Events by Host

```spl
index=* | stats count by host
```

### Failed Logons

```spl
index=* EventCode=4625
```

### Successful Logons

```spl
index=* EventCode=4624
```

### Process Creation Events

```spl
index=* EventCode=1
```

## Dashboard Panels

### Events by Host

Displays total event counts from all reporting systems.

### Failed Logons

Monitors Windows Event ID 4625 activity.

### Successful Logons

Tracks successful authentication activity.

### Process Creation Activity

Monitors Sysmon Event ID 1 process creation logs.

## Skills Demonstrated

- SIEM Administration
- SPL Query Development
- Log Analysis
- Security Monitoring
- Threat Hunting
- Dashboard Creation

## Screenshots

# Dashboard Screenshots

## SOC Dashboard Overview

![SOC Dashboard](Splunk%20SOC%20Dashboard.png)

## Events by Host

![Events by Host](Splunk%20Events%20by%20Host.png)

## Log Sources

![Log Sources](Splunk%20Log%20Source.png)

## pfSense Services Activity

![pfSense Activity](Splunk%20pfsense%20Service%20Activity.png)

## Total Event Volume

![Total Event Volume](Splunk%20Total%20Event%20Volume.png)