# Introduction to Cryptography (Symmetric)

## Core Principles
* **Kerckhoffs's Principle:** The security of a system must rely entirely on the secrecy of the keys, not the secrecy of the algorithm. This completely invalidates "Security Through Obscurity".
* **Randomness:** Modern cryptography relies on pseudo-random generators that use deterministic processes and an initial entropy seed to create sequences that are statistically indistinguishable from true randomness.

## Symmetric Cryptography
* **Mechanism:** Uses a single shared secret key for both encryption and decryption. It is computationally lightweight, making it ideal for encrypting large volumes of data.
* **Vulnerability:** The primary theoretical attack is brute force (exhausting all $2^n$ possibilities). Keys must be regularly refreshed because both time and heavy usage provide cryptanalysts with more data to break the cipher.
* **Stream Ciphers:** Encrypt data bit-by-bit or byte-by-byte by applying an XOR operation against a generated pseudo-random sequence (e.g., ChaCha20, RC4).
* **Block Ciphers:** Encrypt data in fixed-size blocks (e.g., modern algorithms like AES use 128-bit blocks). If the data is not a multiple of the block size, padding is required.
  * **ECB (Electronic Code Book):** Highly insecure for long messages. Because identical plaintext blocks always produce identical ciphertext blocks, patterns remain visible.
  * **CBC (Cipher Block Chaining):** Secure mode that links blocks. Each plaintext block is XORed with the previous ciphertext block ($C_i = enc(K, P_i \oplus C_{i-1})$), requiring an Initialization Vector (IV) for the first block.

## Integrity and Authentication
* **Hash Functions:** Fast algorithms that generate a fixed-length, irreversible, and collision-resistant "digest" of a message of any size. SHA-2 (e.g., SHA-256) and SHA-3 (Keccak) are modern standards; MD5 and SHA-1 are obsolete.
* **Message Authentication Codes (MACs):** Keyed digests (like HMAC) that combine a hash function with a shared secret key to simultaneously prove data integrity and authenticate the sender.
* **Authenticated Encryption with Associated Data (AEAD):** Uses a single algorithm and key to simultaneously encrypt data for privacy and generate an authentication tag (e.g., GCM mode, widely used in TLS).
---
# Asymmetric Cryptography & Applications

## Limitations of Symmetric Crypto
* **Key Distribution:** For $N$ users to communicate securely, the system requires $N \times (N-1)/2$ symmetric keys, creating a severe logistical scaling problem.

## Asymmetric Cryptography
* **Mechanism:** Generates mathematically linked key pairs. The Private Key is kept secret; the Public Key is distributed freely to everyone. Operations performed by one key can only be undone by its pair.
* **Use Cases:** It is computationally heavy, so it is not used for bulk data. It is primarily used to securely distribute small symmetric keys and to create digital signatures.
  * **Confidentiality:** Encrypting a message with the recipient's public key ensures only their private key can read it.
  * **Authentication:** Encrypting a hash digest with the sender's private key creates a digital signature that anyone can verify using the sender's public key.

## Core Asymmetric Algorithms
* **RSA:** Relies on the mathematical difficulty of prime factorization. The public key is $(n,e)$ and the private key is $(n,d)$. Encryption is $C = P^e \pmod n$ and decryption is $P = C^d \pmod n$. A minimum of 2048 bits is currently required for adequate security.
* **Diffie-Hellman (DH):** A key agreement protocol allowing two parties to securely generate a shared symmetric key over an insecure channel. It is highly vulnerable to Man-in-the-Middle attacks if the parties do not authenticate each other first.
* **Elliptic Curve Cryptography (ECC):** Uses 2D curve operations instead of modular arithmetic. It offers the same level of security as RSA but requires significantly shorter keys (roughly 1/10th the size), resulting in much faster execution.

## Passwords and Key Derivation
* **Key Derivation Functions (KDF):** Humans use weak, predictable passwords. A KDF generates a strong pseudo-random cryptographic key from a password by adding a "salt" and running thousands of iterations (e.g., PBKDF2) to aggressively slow down brute-force attacks.

## Quantum Threat & PQC
* **The Quantum Threat:** Quantum computers running Shor's algorithm will solve factorization and discrete logarithms exponentially faster, rendering RSA, DSA, and ECC instantly obsolete. Symmetric crypto is less affected; Grover's algorithm effectively halves the key length, which is easily mitigated by simply doubling the key size.
* **Post-Quantum Cryptography (PQC):** NIST is standardizing new algorithms based on incredibly complex mathematical problems (e.g., lattice-based cryptography like ML-KEM and ML-DSA) that are resistant to quantum computing.

## PKI and Electronic Documents
* **Digital Certificates (X.509):** A data structure that cryptographically binds a public key to an entity's identity, digitally signed by a trusted Certification Authority (CA).
* **Revocation:** If compromised, certificates are revoked before expiration. Relying parties check validity using a CRL (Certificate Revocation List) or OCSP (On-line Certificate Status Protocol).
* **Electronic Documents:** Signatures can be enveloping, enveloped, or detached.
  * **Time-Stamping Authority (TSA):** Provides cryptographic proof that data existed before a specific date and time.
  * **Qualified Electronic Signature (QES):** A high-security signature backed by a Qualified Certificate and secure hardware devices, carrying the exact same legal weight as a handwritten signature.