# Why Cybersecurity Exists
## Core Concepts & Definitions
* **Cybersecurity Core Convergence:** Despite different scopes (individual, organizational, national), all definitions of cybersecurity share three main goals: Ensuring Confidentiality, Integrity, and Availability (CIA triad), guaranteeing resilience, and reducing risk.
* **System Definition:** A set of interacting components (hardware, software, networks, data, people, and procedures) that depend on each other to deliver a service.
* **IT vs. OT (Crucial Distinction):**
  * **IT (Information Technology):** Manages data, computation, and communication (e.g., servers, cloud).
  * **OT (Operational Technology):** Controls physical processes (e.g., sensors, industrial controllers, actuators). 
  * *Exam Note:* Modern infrastructure merges IT and OT, meaning digital vulnerabilities now create physical, real-world consequences.

## The Cyberspace
* **Nature of Cyberspace:** A dynamic socio-technical environment shaped by human behavior, automation, and technical/legal rules.
* **Three Interrelated Layers:**
  1. Physical Network Layer.
  2. Logical Network Layer.
  3. Cyber-Persona Layer.
* **National Cyberspace:** The segment of the global network under a specific nation's legal and administrative jurisdiction, making security a matter of national sovereignty and law.

## Why Systems are Inherently Vulnerable
* **Complexity:** Modern software ecosystems (like OS kernels) contain tens of millions of lines of code. Because comprehensive formal verification is impossible, systems are inherently vulnerable. 
* **Pervasiveness:** The expansion of IoT, 5G, and Cloud computing means connectivity is embedded in physical systems everywhere, causing the attack surface to explode.

## Historical Evolution of Cyber Risk
* **1940s-60s (Isolated Computing):** Physical access was required; security assumptions were purely physical.
* **1948 (Stored-Program Concept):** Instructions became modifiable digital objects. Software flexibility enabled innovation but also introduced software exploitation.
* **1969 (Networking/ARPANET):** Connectivity destroyed the protection of physical distance, introducing remote attack paths.
* **1971 (Creeper & Reaper):** "Creeper" (first self-propagating program) proved code could move autonomously across networks. "Reaper" was the first defensive response, starting the co-evolution of attack and defense.
* **1990s (World Wide Web):** Mass adoption moved value and personal data online, shifting threats toward economically motivated cybercrime.

## The Strategic / EU Context
* **Coordination Problem:** Cybersecurity must be addressed across all layers simultaneously: Individual, Organizational, National, and International.
* **EU Market Limitations:** The European cybersecurity market is heavily fragmented, and companies struggle to scale globally. 
* **Underinvestment:** Severe underinvestment compared to the US leads to strategic dependency and reduced technological sovereignty for the EU.
---
# Systems Thinking & Risk

## Core Concepts
* **Danger:** An intrinsic property accountable to a factor that generates a harmful event; this exists even in the absence of malicious actors.
* **Threat:** Any circumstance or event with the potential to adversely impact assets; unlike danger, a threat introduces intention via a hostile agent.
* **Security:** The state of freedom from conditions that can cause the loss of assets with unacceptable consequences.
* **Asset:** Any tangible or intangible item of value; intangible assets (data, reputation) are often the primary targets of cyberattacks.

## Risk Management
* **Risk Definition:** Risk is the combination of the severity of an impact and the probability of its occurrence (Risk = Severity x Probability).
* **Risk Loop:** The operational loop consists of an Asset Inventory, identifying Threats/Risks, implementing Protection controls, and managing the Residual Risk.
* **Insurance:** Cyber insurance covers residual risk, not a lack of controls, and typically does not reimburse acts of war by state-related entities.

## Safety vs Security
* **Safety:** Ensures the system does not harm people or the environment, focusing on preventing failures caused by accidental, unintentional faults.
* **Security:** Ensures the system is protected from malicious, intentional actions by adversaries.
* **The Dilemma:** A system can be safe but insecure; therefore, systems require a joint "Safety & Security-by-Design" approach.

## Dependability & Resilience
* **Dependability:** A property allowing reliance on a system's services, comprising reliability, safety, security, and maintainability.
* **Resilience:** The ability of a system to prepare for adverse events, absorb disruption, recover within an acceptable time, and adapt to evolving threats.
---
# Security Properties & Crypto

## Data vs Information
* **Distinction:** Data refers to raw items; Information is the meaning inferred from data plus context.
* **Inference Attacks:** Attackers can learn sensitive information indirectly through statistical patterns or linkage, even if direct identifiers are hidden.

## The Extended CIA Triad
* **Confidentiality:** Preventing unauthorised disclosure of information.
* **Integrity:** Preventing unauthorised modification (Data Integrity) and ensuring the system operates without unimpaired manipulation (System Integrity).
* **Availability:** Ensuring timely and reliable access, measured by metrics like Uptime, MTBF (Mean Time Between Failures), and MTTR (Mean Time to Repair).
* **Authenticity:** Guaranteeing the message or source is genuine and credible.
* **Accountability:** The ability to uniquely trace actions to a specific entity, typically enforced via secure logging.
* **Non-repudiation:** Providing cryptographic evidence so an entity cannot falsely deny an action.

## Threats to CIA
* **Stealing:** Breaks confidentiality (e.g., sniffing).
* **Corrupting:** Breaks integrity (e.g., Man-in-the-Middle altering a transfer).
* **Inhibiting:** Breaks availability (e.g., DDoS or ransomware).
* **Forging:** Breaks authenticity (e.g., phishing or supply chain attacks).

## Cryptographic Mechanisms
* **Symmetric Cryptography:** Uses one shared secret key for encryption and decryption; efficient and used for bulk data.
* **Asymmetric Cryptography:** Uses a public key and a private key pair; encrypting with a public key ensures confidentiality, while signing with a private key ensures integrity, authenticity, and non-repudiation.
* **Hash Functions:** Produce a fixed-length digest from a message; detects accidental changes but cannot protect against active attackers alone.
* **Message Authentication Codes (MACs):** Use a shared secret key alongside a hash to provide authenticated integrity.
* **Access Control:** The primary mechanism that operationalises these properties using a Policy Decision Point (PDP) and a Policy Enforcement Point (PEP).
---
# Information Protection

## Dimensions of Protection
* **Privacy:** Protects the individual's fundamental rights and private sphere, focusing on the person, not just the data.
* **Data Protection:** The legal and governance framework (e.g., GDPR) that creates enforceable rules for processing personal data.
* **Secrecy:** An institutional regime that protects sensitive state or organisational information to prevent strategic harm.

## GDPR & Compliance
* **Core Duties:** Requires a lawful basis, data minimisation, purpose limitation, and transparency.
* **Accountability:** Organisations must demonstrably prove their compliance with regulations.
* **Data Breach:** A security incident resulting in the accidental or unlawful destruction, loss, modification, or unauthorised disclosure of personal data.

## Technical Mechanisms
* **Encryption:** Protects data confidentiality at rest and in transit, but does not regulate how data is used once decrypted (encryption is not privacy).
* **Anonymisation:** Irreversibly removes identifiability; if done effectively, the data falls outside GDPR jurisdiction.
* **Pseudonymisation:** Replaces identifiers with tokens; it is reversible with additional info, meaning the data remains under GDPR but risk is reduced.
* **Logging:** A detective control that records events to support accountability and forensics.

## Secrecy & National Defence
* **Classification:** Categorises information severity (e.g., Restricted, Confidential, Secret, Top Secret).
* **Need-to-Know Principle:** Having clearance is not unlimited access; distribution is constrained strictly by operational necessity.
---
# Cyber Attacks & Threat Actors

## The Threat Chain (Explaining Exposure)
* **Weakness:** A general flaw in design, implementation, or configuration (categorised by CWE - Common Weakness Enumeration).
* **Vulnerability:** An exploitable instance of a weakness within a specific environment (categorised by CVE - Common Vulnerabilities and Exposures).
* **Exploit:** The technical artifact or method used to take advantage of a vulnerability to launch an attack.

## The Cyber Kill Chain (Explaining Execution)
* **Reconnaissance:** Gathering passive and active intelligence about the target.
* **Weaponisation:** Preparing the malicious payload (e.g., crafting a malware document).
* **Delivery:** Transmitting the payload to the victim (e.g., via phishing emails).
* **Exploitation:** Triggering the vulnerability to execute code on the target's system.
* **Installation:** Establishing a persistent presence or backdoor on the system.
* **Command and Control (C2):** Establishing a remote connection for the attacker to manage the compromised host.
* **Actions on Objectives:** Executing the final goal, such as data exfiltration or sabotage.

## Threat Actors
* **State-Sponsored (APTs):** Highly resourced entities targeting strategic intelligence, espionage, and operational disruption.
* **Cybercriminals:** Profit-driven actors who increasingly rely on Crime-as-a-Service to scale operations with low marginal costs.
* **Hacktivists:** Ideologically motivated groups focusing on visibility, defacement, and communicative disruption.

## Cyberspace Asymmetry
* **The Defender's Dilemma:** Attackers only need one viable path and can choose their timing, while defenders must secure all assets constantly and operate under legal constraints.
---
# Adversary Behaviour & MITRE ATT&CK

## Limitations of Sequential Models
* **Non-Linearity:** Real-world attackers pivot, repeat steps, and reuse techniques; they do not always follow a strict linear progression like the Kill Chain.
* **Requirement:** Defenders require a behavioural ontology to understand what the adversary is doing, not just where they are in a sequence.

## MITRE ATT&CK Framework
* **Tactics:** Represent the adversary's immediate objective (the "why"), such as Privilege Escalation or Lateral Movement.
* **Techniques:** Represent the reusable behavioural methods used to achieve the objective (the "how"), such as OS Credential Dumping.
* **Procedures:** Represent the concrete, campaign-specific implementation of a technique (e.g., dumping LSASS memory using a specific tool).

## Defensive Mapping & Coverage
* **Observability:** A technique is only defensible if it leaves an artifact that generates telemetry.
* **Detection:** Not mere logging, but the analytical interpretation of telemetry to infer an attack.
* **Coverage Dimensions:** Must be measured across Visibility (collecting telemetry), Detection (identifying the technique), and Mitigation (reducing impact).
* **Residual Risk:** Represents the adversary behaviour that remains unobserved, undetected, or insufficiently mitigated.

## Case Study: Stuxnet
* **Impact:** Proved that IT compromise can be transformed into OT manipulation, leading to strategic physical sabotage.
* **Air-Gapping:** Demonstrated that air-gapped environments reduce exposure but do not eliminate attack paths, as the malware was delivered via an infected USB drive.