# SOC Architecture

Build an isolated defensive lab with a SIEM/log server, Windows endpoint, Linux server, telemetry, and analyst interface. Data flow: endpoint event -> collector -> SIEM -> detection -> triage -> investigation -> response -> report. Generate events only on systems you own/are authorized to test.