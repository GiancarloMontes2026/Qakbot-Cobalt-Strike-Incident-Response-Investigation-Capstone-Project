# Qakbot & Cobalt Strike Incident Response Investigation

## Overview

This project documents a team-based Blue Team cybersecurity investigation completed as the capstone project for CodePath's CYB102 Intermediate Cybersecurity program.

The investigation analyzed a simulated Qakbot (QBot) malware infection that resulted in Cobalt Strike activity within a compromised environment. The project followed the incident from the initial phishing attack through network traffic analysis, IOC identification, threat intelligence, impact assessment, incident triage, and remediation planning.

The objective was to apply a structured incident response methodology to determine how the compromise occurred, identify malicious activity, evaluate its potential impact, and recommend actions to contain and remediate the threat.

## Investigation Scenario

The attack originated from a phishing email containing a malicious attachment.

The malicious document initiated Qakbot, which operated as a loader for additional Cobalt Strike activity. Network traffic and associated artifacts were analyzed to reconstruct the attack and identify indicators associated with the compromise.

The investigation examined the potential for:

- Command and Control (C2) communication
- Credential theft
- Persistence
- Privilege escalation
- Lateral movement
- Data exfiltration
- Additional malware deployment
- Ransomware deployment

## Tools & Technologies

- Wireshark
- VirusTotal
- AbuseIPDB
- MITRE ATT&CK
- PCAP Analysis
- SHA-256 Hash Analysis
- Network Traffic Analysis
- Threat Intelligence
- IOC Analysis
- Incident Response
- Malware Analysis
- Phishing Analysis

## Network Traffic Analysis

Wireshark was used to analyze packet capture (PCAP) data associated with the incident.

Multiple traffic streams and protocols were examined, including:

- DNS
- TCP
- HTTP
- SMB
- SMTP
- POP
- IMAP

The investigation searched for suspicious network behavior and communications associated with Qakbot and Cobalt Strike.

HTTP traffic analysis helped identify suspicious domains, IP addresses, downloaded files, and other potential Indicators of Compromise.

## Indicators of Compromise

The investigation identified and analyzed multiple types of IOCs, including:

- Malicious file hashes
- IP addresses
- Suspicious domains
- Malicious URLs
- Email attachments
- Downloaded malware
- Network communications

Files and indicators discovered during network analysis were investigated further using threat intelligence sources.

VirusTotal was used to analyze suspicious files and hashes and identify malware associated with Qakbot.

## Threat Intelligence

Threat intelligence analysis was performed using:

- VirusTotal
- AbuseIPDB
- Wireshark
- MITRE ATT&CK

The investigation examined Qakbot and Cobalt Strike tactics, techniques, and procedures (TTPs) and connected observed behavior to known adversary techniques.

MITRE ATT&CK techniques examined included areas such as:

- Command and Scripting Interpreter
- PowerShell
- Registry Modification
- Credential Access
- System Information Discovery
- Persistence
- Privilege Escalation
- Application Layer Protocols
- Web Protocols

## Impact Analysis & Incident Triage

My primary contribution to the group investigation focused on Impact Analysis and Triage.

The incident was assessed as high severity because a successful Qakbot/Cobalt Strike compromise could enable persistent access, command-and-control communication, credential compromise, lateral movement, data exfiltration, and additional malware or ransomware deployment.

The triage process considered:

- Detection of unusual network activity
- Identification of potentially compromised systems
- Determination of incident scope
- Severity classification
- Containment and eradication priorities
- Stakeholder communication
- Password resets
- Multi-factor authentication
- Malware removal
- Forensic analysis
- Incident documentation
- Post-incident review

## Incident Response Recommendations

Recommended response actions included isolating affected systems to prevent additional spread, removing or quarantining malicious files, blocking identified malicious infrastructure, reviewing system logs, performing forensic analysis, updating security tools, patching vulnerabilities, and monitoring the environment for reinfection.

## Attack Investigation Workflow

The project followed a Blue Team investigation workflow:

**Phishing Email → Malicious Attachment → Qakbot Infection → Cobalt Strike Activity → Network Analysis → IOC Identification → Threat Intelligence → Impact Assessment → Incident Triage → Containment & Remediation**

## Skills Demonstrated

**Incident Response • SOC Analysis • Malware Investigation • Qakbot • Cobalt Strike • Wireshark • PCAP Analysis • Network Traffic Analysis • Threat Intelligence • IOC Analysis • VirusTotal • AbuseIPDB • MITRE ATT&CK • Phishing Analysis • Incident Triage • Impact Analysis • Threat Detection • Remediation • Blue Team Operations**

## Key Takeaways

This capstone strengthened my understanding of how multiple cybersecurity disciplines work together during a real-world-style incident investigation.

The project required moving beyond identifying individual malicious indicators and examining the larger attack chain. Network evidence, malware indicators, threat intelligence, attacker techniques, and potential organizational impact were combined to determine the severity of the incident and appropriate response actions.

My primary contribution focused on assessing the potential impact of the Qakbot and Cobalt Strike compromise and developing an incident triage approach for detection, scoping, containment, eradication, recovery, documentation, and post-incident review.

The project strengthened practical skills applicable to SOC Analyst, Cybersecurity Analyst, Incident Response, and Threat Intelligence roles.

## Team Project

This project was completed collaboratively as part of the CodePath CYB102 Intermediate Cybersecurity Group Capstone.

My primary responsibility was **Impact Analysis and Incident Triage**, while the overall team investigation covered monitoring sources, asset identification, threat intelligence, IOC analysis, remediation, and case management.

## Disclaimer

This project was completed in an authorized educational environment for cybersecurity training purposes. The analysis was conducted using provided/sample datasets and was intended solely for defensive security education.
