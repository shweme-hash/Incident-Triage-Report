Incident Triage Report: Suspicious Third-Party Remote Access

Incident Type: Potential unauthorised access and data exfiltration

Severity: High – provisional assessment

Status: Under investigation

Environment: Simulated corporate environment

1. Initial Observation

A third-party vendor account established a remote connection to a legacy file server outside the approved maintenance scope. Subsequent activity indicated possible unauthorised access to sensitive customer information.

2. Incident Timeline

Time| Observed Activity

08:14| Vendor account successfully logs in

08:17| Account connects to LEGACY-FS01

08:21| Approximately 2,400 customer archive files accessed

08:27| archive-tool.exe executed under the vendor account

08:31| Approximately 1.8 GB outbound data transfer detected

08:36| Remote session closes

3. Evidence Collected

- Unfamiliar remote login activity.
- Access to a large volume of customer archive files.
- Execution of an archive utility.
- Significant outbound network traffic.
- Remote session termination following the suspicious activity.

4. Potential Impact

Possible exposure or unauthorised extraction of sensitive customer information. The extent of data exposure and whether the transferred information contained customer records remain unconfirmed.

5. Immediate Response

- Escalate the incident to the SOC supervisor.
- Preserve authentication, endpoint, firewall and file-server logs.
- Verify whether the vendor account and remote session were authorised.
- Investigate the source and destination of the outbound transfer.
- Request an authorised containment assessment.
- Establish the scope of potentially affected information.

6. Current Status

Under investigation. The initial findings indicate suspicious third-party access and possible data exfiltration. The initial access method, responsible party and full impact have not yet been established.

7. Lessons Learned

Organisations should implement multi-factor authentication, least-privilege access, vendor account reviews, network segmentation and continuous monitoring of third-party remote connections.
