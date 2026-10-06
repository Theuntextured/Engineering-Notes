# The Human Factor

## Core Concepts
* **The Weakest Link:** No matter how strong the technical defenses (firewalls, encryption), humans remain the most vulnerable element in cybersecurity.
* **PEBKAC:** An acronym meaning "Problem Exists Between Keyboard And Chair," highlighting user error.
* **Social Engineering:** The art and science of manipulating people to release sensitive information, bypass security protocols, or authorize malicious actions. 
* **Primary Targets:** Attackers frequently target help desk, secretarial, and support staff.

## Psychological Vulnerabilities
* **Dual Process Theory (Wason & Evans, 1974):** Decision-making relies on two systems:
  * **System 1 (Intuitive):** Automatic, unconscious, fast, and emotional; it requires zero mental effort.
  * **System 2 (Analytical):** Conscious, rational, slow, and logical; it requires high cognitive effort and concentration.
* **Cognitive Biases:** Social engineers hack human behavior by exploiting cognitive biases (like obeying authority or reacting to high-pressure deadlines) to trigger a fast, compliant response from System 1 before the analytical System 2 can evaluate the threat.
---
# Phishing & Cyber Hygiene

## Cyber Hygiene
* **Definition:** The precautionary measures and best practices individuals and organizations adopt to keep sensitive data secure.

## Types of Phishing
* **Phishing:** Fraudulent communication designed to trick victims into providing credentials, clicking malicious links, or opening malware.
* **Spear Phishing:** Highly targeted phishing aimed at a specific individual, using gathered personal details to appear authentic.
* **Whaling:** Spear phishing specifically targeting high-ranking executives ("whales" like CEOs or CFOs) who have the authority to approve large wire transfers.
* **Business Email Compromise (BEC):** Attackers impersonate trusted contacts (colleagues, vendors) to deceive organizations into paying fake invoices or transferring funds; this often involves actual unauthorized access to the sender's email account.
* **Vishing:** Voice phishing, often using caller ID spoofing to impersonate trusted entities over the phone.
* **Smishing:** SMS/text-message phishing.
* **Typosquatting:** Registering domains that are common misspellings of legitimate sites (e.g., `rnicrosoft.com` instead of `microsoft.com`) to deceive users.

## Technical Exploits & Defenses
* **Microsoft DDE (Dynamic Data Exchange):** A legacy protocol that attackers exploit to execute embedded malicious code in Office documents without triggering the authorization prompts associated with macros.
* **XZ Backdoor Case:** A supply chain attack where a malicious contributor gained maintainer access and inserted a backdoor into a widely used compression tool (utilized in OpenSSH).
* **Defensive Tools:** 
  * **Virtual Machines (VMs):** Emulated computer systems; if the VM OS is compromised by a malicious file, the host OS remains safe.
  * **Sandboxes:** Isolated virtual environments used to safely execute and observe untrusted applications or files.
---
# Physical Attacks

## Physical Access
* **The Golden Rule:** Unrestricted physical access bypasses the strongest digital defenses (like encryption and 2FA); if an attacker physically holds the device, it is compromised.

## Attack Vectors
* **Baiting:** Leaving an infected physical device (like a USB drive) in a public or common area, relying on human curiosity to plug it in.
* **HID (Human Interface Device) Attacks:** Malicious USB devices (e.g., a programmable Teensy board) that emulate a keyboard to rapidly inject pre-configured keystrokes and drop payloads the moment they are plugged in.
* **Charging Risks:** Plugging directly into public USB charging ports can infect devices or allow attackers to infer user behavior via power consumption analysis; always use electrical outlets or data-blocking USB adapters.
* **Keyloggers:** Tools that secretly record keystrokes.
  * **Hardware:** Physical devices spliced into keyboard cables.
  * **Software:** Malicious hypervisors, kernel drivers, API hooks, or Form Grabbing (capturing web form data before submission).
* **Piggybacking / Shoulder Surfing:** Gaining access by closely following an authorized person through a secure door, or visually snooping on their screen (mitigated by privacy filters and screen locks).
* **Man-in-the-Video Attacks:** Intercepting and manipulating video output (e.g., using a malicious HDMI cable) to display spoofed URLs or phishing replicas to the user.

## Dumpster Diving & Sanitization
* **Dumpster Diving:** Scavenging disposed hardware or paper for sensitive data.
* **The Deletion Flaw:** When an OS "deletes" a file, it only marks the space as available; the actual data remains physically on the disk until overwritten.
* **Sanitization:** The process of permanently removing data so it cannot be recovered, mandated by regulations like the GDPR.
  * **Degaussing (Hardware):** Destroying the magnetic field of a hard drive, rendering it completely inoperable.
  * **Wiping/Shredding (Software):** Overwriting every bit or block of file data with new data.