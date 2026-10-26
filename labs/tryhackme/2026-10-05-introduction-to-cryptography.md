# Introduction to Cryptography

## Overview / Objective
Build a working understanding of the cryptographic mechanisms behind secure communication and password storage.

## Platform & date
| Platform | Room | Completed |
|---|---|---|
| TryHackMe | Introduction to Cryptography | 5 October 2026 |

## What I did / key steps
- Classical ciphers and substitution techniques
- Symmetric encryption and AES
- Practical exercises with **GPG** and **OpenSSL**
- Asymmetric encryption and RSA
- Diffie-Hellman key exchange
- Hashing and HMAC
- PKI and SSL/TLS certificates
- Password hashing, salts, rainbow tables and PBKDF2
- How HTTPS protects login credentials in transit

## Key concepts
How the pieces work together:

| Mechanism | Purpose |
|---|---|
| PKI / certificates | Identity verification |
| TLS | Secure session establishment |
| Symmetric encryption | Protecting session traffic |
| Salt + password hashing / KDF | Protecting passwords at rest |

## Findings / outcome
Room completed. The most useful takeaway was seeing how these mechanisms combine, rather than learning each one in isolation.

## Lessons learned
No single cryptographic primitive does everything. Identity, key exchange, bulk encryption and password storage each need the right tool.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7513010288930111488/)
