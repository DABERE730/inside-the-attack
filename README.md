# inside-the-attack
Exploring real-world cyberattacks, attacker techniques, exploited vulnerabilities, threat detection, and defensive security through research and practical investigations.

Cyberattacks rarely happen without a reason. Behind every successful attack, there is usually an exploited weakness, a security gap, human error or an overlooked vulnerability.

This repository explores the techniques, behaviours and weaknesses behind common cyberattacks. It focuses on understanding the attacker's perspective while developing the analytical skills needed to identify, investigate and prevent malicious activities.

The goal is not just to understand what an attack is, but to understand how it works.

---

## 1. Inside a Phishing Attack

Phishing is a social engineering technique in which attackers use deceptive messages, websites or communications to trick individuals into revealing sensitive information or performing actions that compromise their security.

### How It Works

1. An attacker identifies a potential target.
2. A deceptive email or message is created.
3. The message is designed to appear legitimate.
4. The victim is encouraged to click a link, download an attachment or provide sensitive information.
5. The attacker may use the collected information to compromise an account or system.

### What Attackers Exploit
- Human trust.
- Fear and urgency.
- Lack of security awareness.
- Weak authentication practices.

### How Defenders Detect It
- Suspicious sender addresses.
- Unexpected attachments.
- Misleading URLs.
- Unusual login activities.
- Messages requesting sensitive information.

### Prevention
- Verify unexpected communications.
- Avoid suspicious links.
- Use Multi-Factor Authentication.
- Implement email security controls.
- Conduct security awareness training.

---

## 2. Inside a Brute-Force Attack

A brute-force attack involves systematically attempting different password combinations or credentials until the correct one is discovered.

### How It Works

An attacker uses automated tools or scripts to test multiple password combinations against an authentication system.

The effectiveness of this attack depends on factors such as password complexity, authentication controls and account lockout mechanisms.

### What Attackers Exploit
- Weak passwords.
- Reused credentials.
- Lack of rate limiting.
- Poor authentication configurations.
- Absence of Multi-Factor Authentication.

### How Defenders Detect It
- Repeated failed login attempts.
- Unusual authentication patterns.
- Multiple login attempts from suspicious sources.
- Unexpected account lockouts.

### Prevention
- Use strong, unique passwords.
- Implement MFA.
- Introduce login rate limiting.
- Monitor authentication logs.
- Apply account lockout policies carefully.

---

## 3. Inside a DDoS Attack

A Distributed Denial-of-Service (DDoS) attack attempts to make a service unavailable by overwhelming it with traffic or requests from multiple sources.

### How It Works

An attacker coordinates traffic from multiple devices or systems, often through a botnet, to overwhelm a target's resources.

The target may become slow, unstable or completely unavailable.

### What Attackers Exploit
- Limited server resources.
- Network bandwidth limitations.
- Weak traffic filtering.
- Insufficient infrastructure protection.

### How Defenders Detect It
- Sudden increases in traffic.
- Unusual traffic patterns.
- High resource consumption.
- Increased latency.
- Unexpected service interruptions.

### Prevention
- Use DDoS protection services.
- Implement traffic filtering.
- Configure rate limiting.
- Use load balancing.
- Monitor network traffic.

---

## 4. Inside a Man-in-the-Middle Attack

A Man-in-the-Middle (MitM) attack occurs when an attacker intercepts or potentially manipulates communication between two parties without their knowledge.

### How It Works

An attacker positions themselves between communicating systems and attempts to observe or modify information being exchanged.

This can happen through compromised networks, malicious access points or other interception techniques.

### What Attackers Exploit
- Unsecured network connections.
- Weak encryption.
- Certificate validation failures.
- Poor network security configurations.

### How Defenders Detect It
- Unexpected certificate warnings.
- Suspicious network behaviour.
- Unusual DNS activity.
- Unexpected changes in network routes.

### Prevention
- Use HTTPS.
- Avoid untrusted networks.
- Validate digital certificates.
- Use secure VPN connections where appropriate.
- Keep network devices updated.

---

## 5. Inside a Privilege Escalation Attack

Privilege escalation occurs when an attacker gains permissions beyond those originally assigned to their account.

There are two major categories:

**Vertical Privilege Escalation:** An attacker gains higher-level permissions, such as moving from a standard user account to administrator or root access.

**Horizontal Privilege Escalation:** An attacker gains access to another user's resources or account at a similar privilege level.

### What Attackers Exploit
- Misconfigured permissions.
- Vulnerable software.
- Weak access controls.
- Excessive privileges.
- Insecure system configurations.

### How Defenders Detect It
- Unexpected privilege changes.
- Suspicious administrative activities.
- Unusual process execution.
- Unauthorized access to protected resources.

### Prevention
- Apply least privilege.
- Patch vulnerable systems.
- Monitor privileged accounts.
- Audit permissions regularly.
- Secure administrative credentials.

---

## 6. Inside a DNS Attack

The Domain Name System (DNS) translates human-readable domain names into IP addresses.

DNS attacks target this process to redirect users, disrupt services or manipulate the information used to locate systems.

### Common DNS Attacks

- DNS Spoofing.
- DNS Cache Poisoning.
- DNS Tunnelling.
- DNS Amplification.

### What Attackers Exploit
- Weak DNS configurations.
- Vulnerable DNS infrastructure.
- Poor monitoring.
- Inadequate DNS security controls.

### How Defenders Detect It
- Unexpected DNS responses.
- Unusual DNS queries.
- Suspicious domain requests.
- Abnormal DNS traffic patterns.

### Prevention
- Use trusted DNS resolvers.
- Implement DNSSEC where appropriate.
- Monitor DNS traffic.
- Secure DNS server configurations.
- Investigate suspicious domain activity.

---

## 7. Inside a Malware Infection

Malware is malicious software designed to disrupt operations, steal information, gain unauthorized access or perform other harmful activities.

### Common Types of Malware

**Trojan:** Malicious software disguised as legitimate software.

**Ransomware:** Malware that encrypts or otherwise restricts access to data and demands payment.

**Spyware:** Software designed to secretly monitor activities or collect information.

**Worm:** Malware capable of spreading between systems without requiring the same user-driven execution as many other malware types.

**Rootkit:** Malicious software designed to conceal activity and maintain privileged access.

### How Defenders Investigate Malware
- Examine suspicious files.
- Analyse file hashes.
- Monitor unusual processes.
- Investigate network connections.
- Review endpoint security alerts.

### Prevention
- Maintain updated systems.
- Use reputable endpoint protection.
- Avoid untrusted downloads.
- Restrict unnecessary permissions.
- Maintain secure backups.

---

## 8. Inside an Account Takeover

Account takeover occurs when an attacker gains unauthorized control of another person's account.

### Common Methods
- Credential theft.
- Phishing.
- Password reuse.
- Credential stuffing.
- Session hijacking.

### Warning Signs
- Unexpected login notifications.
- Password reset requests.
- Unfamiliar devices or locations.
- Changes to account settings.
- Unrecognized transactions or activities.

### Prevention
- Enable MFA.
- Use unique passwords.
- Secure recovery methods.
- Monitor account activity.
- Revoke suspicious sessions.

---

## 9. The Defender's Perspective

Understanding how attacks work is only one side of cybersecurity.

The other side involves identifying suspicious behaviour, investigating evidence, understanding potential impact and responding appropriately.

### Important Defensive Activities

**Log Analysis:** Reviewing system and application logs to identify unusual activities.

**Network Monitoring:** Observing network traffic for suspicious communication patterns.

**Endpoint Monitoring:** Monitoring devices for unusual processes, file changes and other potentially malicious behaviour.

**Vulnerability Management:** Identifying weaknesses, assessing their severity and recommending remediation.

**Incident Response:** Following structured procedures to investigate, contain and recover from security incidents.

---

## 10. Security Investigation Framework

For each investigation documented in this repository, I will use the following approach:

1. **Identify:** Determine the suspicious activity or security concern.
2. **Understand:** Establish how the attack works.
3. **Investigate:** Examine available evidence, logs and system behaviour.
4. **Analyse:** Identify the exploited weakness and potential impact.
5. **Detect:** Determine how defenders can recognise the activity.
6. **Mitigate:** Recommend controls to reduce the risk.
7. **Document:** Record findings, observations and lessons learned.

---

## 11. Practical Investigations

This section will contain hands-on security investigations and controlled demonstrations.

Planned investigations include:

- Analysing suspicious network traffic using Wireshark.
- Investigating authentication failures.
- Examining Linux system logs.
- Exploring vulnerability detection using OpenVAS.
- Monitoring endpoint activities using Wazuh.
- Analysing suspicious files in a controlled environment.
- Investigating network scanning activities.

All practical testing will be conducted in authorised environments.

