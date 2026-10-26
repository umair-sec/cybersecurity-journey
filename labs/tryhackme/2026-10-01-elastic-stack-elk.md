# Elastic Stack (ELK)

## Overview / Objective
Learn the Elastic Stack and use Kibana to investigate VPN logs.

## Platform & date
| Platform | Room | Path | Completed |
|---|---|---|---|
| TryHackMe | Elastic Stack (ELK) | SOC Level 1 | 1 October 2026 |

## What I did / key steps
- Learned the components: **Elasticsearch, Logstash, Beats and Kibana**
- Explored and analysed logs in **Kibana Discover**
- Wrote queries in **KQL** (Kibana Query Language)
- Filtered VPN logs by user, IP address, country, state and time range
- Identified anomalies and unusual spikes in VPN activity
- Investigated failed VPN connection attempts
- Created tables and visualisations
- Built a custom dashboard from saved searches and visualisations

## Key concepts
- Kibana Discover, fields and filters
- KQL
- Saved searches → visualisations → dashboards

## Findings / outcome
Because I had already worked with Splunk in earlier labs and investigations, ELK/Kibana felt fairly easy, especially exploring fields, applying filters and visualising log data.

## Lessons learned
Splunk and ELK have different interfaces and query languages, but the SOC investigation mindset is the same:
1. Understand the logs
2. Filter out the noise
3. Correlate the relevant fields
4. Investigate the anomalies

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7511570621953236992/)
