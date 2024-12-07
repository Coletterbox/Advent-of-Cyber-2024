# Day 2 (Log Analysis)

- events from different devices sent to SIEM
- alerts can be TP or FP
- SOC can confirm with users

- connect to Elastic SIEM
- click on "Discover" to view events
- filter by date range
- filter by type
- check for events related to PowerShell
- check (fields):
  - host.hostname
  - user.name
  - event.category
  - process.command_line for commands run
  - event.outcome to see if the activity succeeded
  - source.ip to find out who ran the commands
- filter for authentication events
- (can use the plus and minus next to field to filter or remove)
- event.category: process to see PowerShell commands
- -EncodedCommand can be decoded using CyberChef
- event.category: authentication for logon attempts
- event.outcome: failure
