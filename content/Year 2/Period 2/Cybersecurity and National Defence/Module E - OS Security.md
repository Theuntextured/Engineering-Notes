## Foundational Security Principles
* **Least Privilege:** Users and processes must only have the absolute minimum permissions essential for their specific roles. This improves system stability, security, and deployment simplicity.
* **Access Control:** Regulates whether an active subject (user/process) can interact with a passive object (file/system memory). 

## Protection Systems & Matrices
* **Protection System:** Comprises a protection state (who can do what) and transition operations that modify that state.
* **Access Control Matrix:** A table defining protection domains. Rows represent subjects, columns represent objects, and cells define access rights.
  * **ACL (Access Control List):** Corresponds to a *column* in the matrix, detailing every subject permitted to access a specific object.
  * **Capability:** Corresponds to a *row* in the matrix, listing all objects a specific subject can access.

## Access Control Models
* **Discretionary Access Control (DAC):** The resource owner decides who can access it; untrusted processes can alter the protection state. Used in Windows, Linux, and macOS.
* **Mandatory Access Control (MAC):** Only authorized administrators can modify permissions via trusted software, using strict security labels for subjects and objects. Used in highly sensitive environments like the military.
* **Role-Based Access Control (RBAC):** Permissions are assigned to roles based on organizational competency and authority, not to individual users directly.

## The Reference Monitor
* **Definition:** The foundational mechanism that enforces access control by evaluating every request.
* **Three Elements:**
  * **Interface:** Intercepts requests and triggers hooks.
  * **Authorization Module:** Translates process identities/objects into labels and queries the policy store.
  * **Policy Store:** Central repository managing protection states and evaluating authorization queries.

## Secure OS Requirements & Isolation
* **Secure OS Guarantees:** Must feature Complete Mediation (evaluating every sensitive operation), Tamperproof design (protected from untrusted software), and be Verifiable (compact enough for comprehensive testing).
* **Isolation Types:** Systems enforce separation via Physical (dedicated hardware), Temporal (separate execution times), Logical (abstracted workspaces), and Cryptographic (encryption) isolation.
* **Security Kernel:** The core component (hardware and software) that brings the reference monitor concept to life to enforce protocols.

## Security in Specific Operating Systems
* **UNIX:** Uses protection rings, allocates unique address spaces for processes, and treats all persistent system resources as files. The Trusted Computing Base (TCB) includes the kernel and 'root' processes.
* **Windows:** Uses a DAC model similar to UNIX but is highly extensible. It manages a broader range of object types via Active Directory and uses highly granular, flexible ACLs instead of simple mode bits.
* **Android:** Apps run in secure, isolated sandboxes and each app is assigned a unique user identity. It enforces MAC using Security-Enhanced Linux (SELinux) and ensures system integrity through a cryptographic Verified Boot Mechanism.