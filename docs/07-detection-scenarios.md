# Detection Scenarios

All scenarios are benign and lab-only.

- Enter an incorrect password a small number of times for a fictional account and detect failures.
- Create a fictional test account through normal admin tools and observe the event.
- Temporarily add a fictional test account to a lab admin group, observe, then remove it.
- Run harmless PowerShell process/service queries and observe telemetry.
- Against your own Linux VM, generate a small number of failed SSH authentications and observe logs.

Record expected event, actual event, detection, analyst decision, and cleanup.