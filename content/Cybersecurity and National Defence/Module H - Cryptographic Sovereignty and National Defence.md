## Cryptography as a State Capability
* **The Three Pillars:** Cryptography at the state level involves defensive capabilities (protecting state secrets), offensive capabilities (breaking adversary secrets), and sovereign capabilities (avoiding blind dependence on uncontrollable algorithms or suppliers).
* **Code-Makers vs. Code-Breakers:** Cryptography is an evolutionary arms race driven by mathematics, computing machines, intelligence organizations, and political pressure.
* **The Intelligence Paradox:** A cryptanalytic breakthrough is a strategic asset, but revealing that capability publicly prompts the adversary to change their system and erase the advantage.
* **The Secret Frontier:** The classified domain of cryptography is often years or decades ahead of public academic research.

## Historical Case Studies
* **Mary Stuart & The Babington Plot:** Excessive trust in a weak cipher caused conspirators to write explicitly. British intelligence intercepted, decrypted, and forged additions to the letters to map the conspiracy, proving that weak cryptography can be worse than no encryption at all.
* **The Zimmermann Telegram:** During WWI, Germany relied on vulnerable, third-party diplomatic cables to propose an alliance to Mexico. British intelligence decrypted the message but faced the dilemma of using the intelligence to influence US policy versus risking the exposure of their codebreaking capabilities.
* **Crypto AG:** A Swiss encryption supplier was secretly acquired by the CIA and West German BND. They sold manipulated cryptographic products to dozens of foreign governments for decades, demonstrating that a compromised supplier scales vulnerabilities globally.
* **Enigma & Bletchley Park:** Polish cryptanalysts first modeled the German Enigma machine mathematically and exploited procedural weaknesses. British intelligence scaled this at Bletchley Park using Alan Turing's "Bombe" machines and guessed plaintext fragments called "cribs". To protect the source, the Allies had to use the resulting "Ultra" intelligence indirectly, avoiding actions that were too perfect.
* **GCHQ's Secret Public-Key Discovery:** British intelligence researchers (Ellis, Cocks, and Williamson) secretly invented public-key cryptography years before the public Diffie-Hellman and RSA breakthroughs. The secrecy preserved their intelligence advantage but cost them public recognition and patent opportunities.

## The Crypto Wars & Decentralization
* **Phil Zimmermann and PGP:** In 1991, Zimmermann released Pretty Good Privacy (PGP), combining fast symmetric ciphers with RSA public-key encryption to bring strong cryptography to ordinary citizens.
* **Export Controls:** The US government treated strong cryptographic software as a munition, placing it under export control to preserve surveillance capabilities. This policy created fragmented security, such as weaker export-grade browsers for foreign users and architectural constraints in early hardware like TPM 1.2.
* **Exceptional Access (Key Escrow):** The state attempted to mandate systems like the Clipper chip, which offered strong encryption but split the keys between escrow authorities for lawful government access. It failed due to a lack of public and international trust. Modern debates (like Apple vs. government unlock orders or EU client-side scanning proposals) are continuations of this same conflict.

## Standardization & Sovereignty
* **DES to AES:** The Data Encryption Standard (DES) suffered from a lack of public trust due to opaque NSA involvement and a controversial 56-bit key length. The Advanced Encryption Standard (AES) rebuilt trust through a transparent, open international competition.
* **National Standards:** States may reject foreign trust ecosystems. China developed its own "ShangMi" (SM) commercial cryptographic standards (e.g., SM2, SM3, SM4) to ensure technological sovereignty and protect national infrastructure from foreign algorithms.