# SOC Investigation Write-ups

A collection of hands-on SOC investigation write-ups focused on alert triage, log analysis, endpoint telemetry, threat intelligence, incident validation, containment, and MITRE ATT&CK mapping.

The repository is organized so that each investigation is self-contained: the write-up and all of its supporting screenshots live in the same folder.

## Investigations

| ID | Investigation | Main focus |
|---|---|---|
| [SOC168](writeups/SOC168-whoami-command-injection/README.md) | Whoami Command Detected in Request Body | Web command injection, SIEM triage, EDR correlation, response-size analysis, containment |
| [SOC342](writeups/SOC342-sharepoint-toolshell-rce/README.md) | SharePoint ToolShell — CVE-2025-53770 | SharePoint exploitation analysis, authentication bypass/RCE chain, process and PowerShell investigation |

## Repository Structure

```text
soc-investigation-writeups/
├── README.md
├── .gitignore
└── writeups/
    ├── SOC168-whoami-command-injection/
    │   ├── README.md
    │   └── assets/
    └── SOC342-sharepoint-toolshell-rce/
        ├── README.md
        └── assets/
```

## Investigation Workflow

The write-ups generally follow a repeatable SOC workflow:

1. Alert context and initial triage
2. Source/destination and asset validation
3. Threat-intelligence and reputation checks
4. SIEM/log investigation
5. Endpoint/EDR correlation
6. Exploitation validation and impact assessment
7. Incident verdict
8. Containment and escalation
9. MITRE ATT&CK mapping

## Topics Covered

- SOC alert triage
- SIEM and log analysis
- Web exploitation investigation
- Endpoint Detection and Response (EDR)
- Threat intelligence / IP reputation
- Incident response and containment
- MITRE ATT&CK mapping
- Command injection and remote code execution
- Microsoft SharePoint security investigations
