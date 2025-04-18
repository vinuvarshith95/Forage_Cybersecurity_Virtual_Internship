## Task 2 – Response

### 1. What kind of attack has happened and why do you think so?

This was a **phishing attack** that likely escalated into a **ransomware** incident.

- The initial email, disguised as a message from HR, directed employees to a fake portal. This is a common phishing tactic used to steal login credentials.
- The presence of an error page after credential submission strongly indicates **credential harvesting**.
- Later reports of issues opening file shares and Word documents are **classic signs of ransomware**, where files are either encrypted or corrupted.

---

### 2. As a cyber security analyst, what are the next steps to take?

- **Alert the incident response team** and activate the response plan.
- **Disconnect compromised systems** from the network to prevent lateral spread.
- **Notify all employees** about the phishing email and instruct them not to interact with it.
- **Check logs and email filters** to trace affected users and how the email bypassed defenses.
- Begin **threat hunting** to detect any malicious payloads or indicators of compromise (IOCs).
- **Reset passwords** for potentially affected user accounts.
- **Inform management and legal/compliance** teams if sensitive data may be impacted.

---

### 3. How would you contain, resolve, and recover from this incident?

#### Containment
- Isolate infected systems immediately.
- Block access to the phishing domain at the firewall or DNS level.
- Suspend or reset accounts suspected of being compromised.

#### Resolution
- Perform full malware scans and forensic investigation.
- Remove any discovered malware or backdoors.
- Reimage infected systems if necessary.
- Apply missing security patches and update antivirus/EDR tools.

#### Recovery
- Restore files and systems from **verified clean backups**.
- Gradually reconnect restored systems to the network.
- Monitor systems closely for any reinfection or anomalies.
- Verify full system functionality before marking the incident as resolved.

---

### 4. What activities should be performed post-incident?

- Conduct a **post-incident review** to evaluate response effectiveness.
- Update the **incident response plan** based on lessons learned.
- Document the incident thoroughly in a **formal report**.
- Deliver **targeted security training** to help employees recognize phishing attempts.
- Review and enhance **technical controls** such as MFA, email filtering, and endpoint protection.
- Test and validate **backup and disaster recovery processes** to ensure future readiness.
