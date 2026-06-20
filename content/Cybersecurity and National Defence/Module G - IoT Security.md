## IoT Fundamentals
* **Definition:** ITU-T Y.2060 defines IoT as a global infrastructure connecting physical and virtual things via interoperable communication technologies.
* **Components:** An IoT device typically requires a microcontroller (for computing), sensors/actuators (for interacting with the physical environment), network connectivity, and a unique identifier.
* **Connection Dimension:** IoT adds the "Any Thing connection" dimension, complementing traditional "Any Time" and "Any Place" network paradigms.

## Architecture & Security Framework
* **ITU-T Reference Model:** Consists of four primary layers: Device layer, Network layer, Service/Application support layer, and IoT Applications. Management and security functions operate across all four levels.
* **Security Framework Layers:** Smart Objects (edge devices), Fog Network, Core Network, and Data Center/Cloud.
* **Cross-Layer Security Capabilities:**
  * **Role-Based Access Control (RBAC):** Allocates access rights to specific roles rather than individual users, widely adopted for managing IoT device access.
  * **Tamper Resistance & Detection:** Crucial at the smart object and fog network layers because these devices are physically located outside secured enterprise perimeters.
  * **IPSec (Internet Protocol Security):** Ensures data confidentiality and integrity as it travels between architectural layers.

## IoT Security Challenges & Threats
* **Device Homogeneity:** Many IoT devices share identical hardware and connectivity methods; consequently, a single vulnerability can compromise millions of devices simultaneously.
* **Lifecycle Issues:** IoT devices have long operational lives, often outlasting manufacturer support ("orphaned" devices), and lack convenient mechanisms for software upgrades.
* **Operational Blind Spots:** Devices lack transparency (users cannot monitor internal processes) and fail to provide alerts when security breaches occur.
* **Primary Threats:** Cyber attacks (using IoT to access broader enterprise networks), data breaches, and physical device failures (e.g., compromised heating systems causing burst pipes).

## Security Countermeasures
* **Lightweight Cryptography:** Cryptographic methods specifically optimized for resource-constrained devices (like sensors and RFID tags) to provide end-to-end encryption at the application layer.
* **Password Limitations:** Passwords are becoming less viable in IoT because constrained devices struggle with password processing, and passwords hinder automated machine-to-machine communication.
* **Hardware Protections:**
  * **Trusted Execution Environment (TEE):** Hardware security extensions within CPUs that create a shielded "Secure World" isolated from the standard OS.
  * **Secure Element:** A tamper-proof hardware module acting as a root of trust that securely stores data and manages the device's lifecycle.
  * **Hardware Crypto Processors & HSMs:** Dedicated physical chips/devices for cryptographic operations that ensure decrypted data never leaves the protected environment or gets exposed on standard buses.
* **Blockchain:** A decentralized database of chronologically ordered blocks and transactions; integrating it with IoT prevents unauthorized alterations and ensures robust data integrity and auditability.
* **Data Erasure:** Software or hardware techniques that overwrite existing storage with binary data to ensure complete sanitization and prevent recovery.