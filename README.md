# ServiceNow IT Help Desk Ticketing Lab

## Overview
Portfolio lab using a **ServiceNow Personal Developer Instance (PDI)** to simulate five IT help desk incidents. Practiced ticket creation, incident lifecycle management, customer-visible comments, internal work notes, impact/urgency-based prioritization, resolution documentation, and escalation planning.

**All incidents and troubleshooting procedures are training simulations.** No real employee accounts, workstations, printers, or production networks were changed.

## Incident scenarios

| Scenario | Incident | Troubleshooting documented | Lab outcome |
|---|---|---|---|
| Employee account lockout | `INC0010003` | Identity verification, Active Directory account review, authorized unlock/password reset, login validation | Resolved for training |
| Internet connectivity failure | `INC0010006` | `ipconfig /all`, `ping`, `nslookup`, DHCP, gateway and DNS checks | Resolved for training |
| Microsoft Outlook crashes | `INC0010007` | Event Viewer, classic Outlook Safe Mode, COM add-ins, Office Quick Repair, profile checks | Resolution workflow documented |
| Printer unavailable | `INC0010008` | Print queue, Print Spooler service, printer connectivity, drivers, test page | Resolution workflow documented |
| Department-wide network outage | `INC0010010` | Impact assessment, infrastructure investigation, escalation and stakeholder communication | Left In Progress pending simulated restoration |

## Skills demonstrated
- **ITSM / ServiceNow:** incident intake, ticket tracking, status changes, work notes, resolution documentation
- **Help desk:** troubleshooting methodology, clear technical notes, customer communication
- **Networking:** TCP/IP, DHCP, DNS, default gateway, reachability tests
- **Windows support:** Event Viewer, Office troubleshooting, Windows services, printer support
- **Incident prioritization:** observed **Impact 2 – Medium + Urgency 1 – High = Priority 2 – High** for the simulated outage
- **Escalation:** documented when to involve the network infrastructure team and why not to close an unresolved outage

## Workflow
1. Create incident with caller, short description and customer-visible summary.
2. Review urgency and impact, and verify calculated priority.
3. Move **New → In Progress**.
4. Add **internal Work notes** with a structured investigation plan.
5. Record simulated resolution or document escalation and keep the incident open.
6. Capture evidence screenshots.

## Evidence
The project evidence package contains 11 screenshots in a `screenshots/` folder, including incident forms, status changes, and posted work notes. **Screenshots will be linked here after upload.** Some final resolution screenshots were not available in the export.

## Lessons learned
ServiceNow distinguishes customer-visible comments from internal technician work notes. High-impact incidents require appropriate prioritization, communication, and escalation. A ticket should not be closed simply because troubleshooting has started: restoration must be verified in real environments.

## Future improvements
- Add the remaining resolution and escalation screenshots.
- Reproduce selected troubleshooting procedures in a disposable Windows test VM and capture actual command results.
- Practice assignment group routing and SLA tracking in the developer instance.
