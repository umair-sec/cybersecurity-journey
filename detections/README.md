# Detections (SPL)

Splunk SPL searches taken from my lab write-ups, kept in one place so I can reuse and improve them.

Each `.spl` file starts with a comment header: what it looks for, the data it needs, the related MITRE ATT&CK technique and a link back to the write-up it comes from.

| File | What it looks for | Source write-up |
|---|---|---|
| [sysmon-plink-process-creation.spl](sysmon-plink-process-creation.spl) | `plink.exe` in Sysmon Event ID 1 (process creation) | [plink.exe / Event ID 4688 investigation](../labs/splunk-home-lab/2026-09-10-plink-event-4688-investigation.md) |
| [win-4688-plink-parent-lookup.spl](win-4688-plink-parent-lookup.spl) | 4688 process creation for `plink.exe` and its creator process | [plink.exe / Event ID 4688 investigation](../labs/splunk-home-lab/2026-09-10-plink-event-4688-investigation.md) |
| [win-rdp-logon-type-10.spl](win-rdp-logon-type-10.spl) | Remote interactive (Logon Type 10) sessions with noise filtered out | [Threat-hunting noise-reduction workflow](../labs/splunk-home-lab/2026-09-06-noise-reduction-threat-hunting-workflow.md) |
| [win-logon-outside-hours.spl](win-logon-outside-hours.spl) | Logons outside a user's normal working hours | [Threat-hunting noise-reduction workflow](../labs/splunk-home-lab/2026-09-06-noise-reduction-threat-hunting-workflow.md) |
| [sysmon-encoded-powershell.spl](sysmon-encoded-powershell.spl) | PowerShell started with `-EncodedCommand` | [Splunk 2 (BOTS v2)](../labs/tryhackme/2026-10-28-splunk-2-bots-v2.md) |
| [c2-most-contacted-uri.spl](c2-most-contacted-uri.spl) | Most contacted URIs for a suspicious host (majority behaviour) | [Splunk 2 (BOTS v2)](../labs/tryhackme/2026-10-28-splunk-2-bots-v2.md) |

**Notes**
- Only `sysmon-plink-process-creation.spl` is copied word for word from a write-up. The others turn the steps described in the write-ups into reusable searches.
- Index, sourcetype and field names change between environments (home lab vs BOTS v2). Adjust them before running a search.
