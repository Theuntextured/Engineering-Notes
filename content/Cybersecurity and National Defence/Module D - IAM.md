# Access Control Definitions

## Core Security Functions
* **Access Control:** The process of granting or denying specific requests to obtain and use information or to enter physical facilities.
* **Authentication:** The verification that the credentials of a user or system entity are valid.
* **Authorization:** The granting of rights or permissions to a system entity, determining who is trusted for a specific purpose.
* **Auditing:** An independent review of system records to ensure compliance with policies and to detect security breaches. Internal audits are performed by employees to identify and mitigate risks, whereas external audits are conducted by independent professionals to build client and shareholder confidence.

## Access Control Framework
* **Security Mechanism:** The low-level software and hardware functions that enforce controls.
* **Security Policy:** The high-level rules that dictate what types of access are permitted and by whom.
* **Security Model:** The formal mathematical or logical representation of the security policy.
* **Entities:** 
  * **Subjects:** Active entities (like users or processes) capable of accessing objects.
  * **Objects:** Passive resources (like files or directories) containing or receiving information.
  * **Actions:** Operations a subject can perform, such as Read, Write, or Execute.

## Access Control Models
* **Discretionary Access Control (DAC):** Controls access based on the identity of the requestor and explicit rules. It allows the owner of an object to specify which users or groups can access it. Conceptually represented by an Access Matrix, it is practically implemented using Authorization Tables, Access Control Lists (ACLs), or Capability Lists.
* **Mandatory Access Control (MAC):** Controls access by comparing security labels (resource sensitivity) with security clearances (user eligibility). Users cannot alter these permissions on their own volition.
* **Role-Based Access Control (RBAC):** Controls access based on the organizational roles users assume, rather than individual identity. It utilizes role hierarchies to allow superior roles to inherit the access rights of subordinate roles. It also enforces constraints, such as mutually exclusive roles.
* **Attribute-Based Access Control (ABAC):** Controls access based on the attributes of the subject, the object, and environmental conditions (such as time of day or network security level). It is extremely flexible but carries a higher cost in complexity and performance.

---

# Security by Design

## Foundation
* **Security by Design:** Software must be designed from the foundation to be secure, enforcing the best security tactics through its architecture rather than retrofitting them later.

## Main Security Principles
* **Least Privilege:** An entity should only be given the absolute minimum privileges and resources required to complete a task, and only for the minimum necessary duration.
* **Separation of Duties:** Sensitive activities must depend on the satisfaction of multiple conditions (e.g., requiring two individuals with different keys), forcing attackers to collude to compromise the system.
* **Separation of Privilege:** A single privilege should be broken across multiple independent subjects so that multiple authorizations are required to perform an action.
* **Defense in Depth:** The application of multiple layers of protection, ensuring that if an outer layer is breached, subsequent layers continue to provide security.
* **Fail Secure:** If a system fails, it must default to a state that denies access, preventing unauthorized users from exploiting the outage.
* **Complete Mediation:** Every single access request must undergo a valid authorization procedure; this cannot be bypassed, even during system shutdown or maintenance.
* **Least Common Mechanism:** Systems should minimize the number of protection mechanisms shared among users to prevent unintentional data transfers or the creation of covert channels.
* **Psychological Acceptability:** Security interfaces must be intuitive and easy to use so that users do not have to interpret complex instructions.
* **Weakest Link:** A protection system is only as strong as its most fragile module.
* **Open Design:** Directly opposes "Security by Obscurity" by ensuring that architectural designs can remain secure even when their inner workings are publicly known.

## Zero Trust
* **Philosophy:** Abides by the mantra "Never Trust, Always Verify," utilizing least privilege and a default-deny posture.
* **Architecture:** Replaces broad network trust zones with microperimeters, ensuring full visibility and constant inspection.