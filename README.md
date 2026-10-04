# Enterprise SOC & Incident Response Lab

**Cybersecurity • SIEM • Windows/Linux Telemetry • Detection Engineering • Incident Response**

## Project Summary
This project builds a small enterprise-style security operations environment for collecting endpoint telemetry, detecting suspicious activity, investigating alerts, and documenting incident response.

The exercises use **controlled, benign lab activity**. The goal is defensive analysis—not malware deployment or unauthorized access.

## Architecture
```text
                ENTERPRISE SOC LAB
                       |
              Central SIEM / Logs
                 /           \
                /             \
       Windows Endpoint     Linux Server
       Security Events      Auth/System Logs
              |                 |
           Telemetry          Telemetry
                \             /
                 \           /
                  SOC Analyst
                      |
       Detect -> Triage -> Investigate
                      |
       Contain -> Recover -> Report
```

## Scenarios
- Repeated failed authentication attempts
- Creation of a new test user
- Authorized test changes to privileged-group membership
- Benign PowerShell activity designed to generate observable telemetry
- Linux SSH authentication failures
- Service/process and system-event investigation

## Skills Demonstrated
- SIEM concepts
- Windows event logging
- Linux authentication/system logs
- Endpoint telemetry
- Detection-rule development
- Alert triage
- Log correlation
- Incident investigation
- Containment and recovery planning
- Incident reporting
- MITRE ATT&CK mapping concepts
- Security documentation

## Documentation
1. [SOC Architecture](docs/01-soc-architecture.md)
2. [Telemetry and Logging](docs/02-telemetry-and-logging.md)
3. [SIEM Deployment](docs/03-siem-deployment.md)
4. [Detection Engineering](docs/04-detection-engineering.md)
5. [Investigation Workflow](docs/05-investigation-workflow.md)
6. [Incident Response](docs/06-incident-response.md)
7. [Detection Scenarios](docs/07-detection-scenarios.md)
8. [Incident Report](docs/08-incident-report.md)
9. [Screenshot Evidence](images/README.md)

## Analyst Workflow
```text
Event Generated
      |
Telemetry Collected
      |
SIEM Ingests Event
      |
Detection / Alert
      |
Triage Severity
      |
Investigate Context
      |
Determine Scope
      |
Contain / Recover
      |
Document Findings
```

## Safety Boundary
All scenarios must be performed only on systems owned/authorized for this lab. Use benign activity to generate telemetry. Do not deploy real malware, steal credentials, attack public systems, or expose vulnerable services to the Internet.

## Portfolio Outcome
The finished project provides interview-ready evidence that I can build visibility, interpret security telemetry, investigate an alert, explain findings, recommend remediation, and produce professional incident documentation.

## Author
**Alexis Wiscovitch** — [@Alexis-error404](https://github.com/Alexis-error404)
