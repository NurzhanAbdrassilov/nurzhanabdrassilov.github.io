---
title: Secure File Sharing System
layout: single
excerpt:
  Designed and implemented an end-to-end encrypted file sharing system with access control, rollback protection, and cryptographic integrity, built in Go.
collection: projects
---

- Designed and implemented a secure, end-to-end encrypted file sharing system supporting multiple users, file storage, and access revocation
- Built a stateless key-value storage interface with client-side encryption, integrity protection, and password-based user authentication
- Enabled fine-grained access control through secure key distribution and sharing between users
- Implemented append, load, and delete operations resilient to rollback and replay attacks
- Developed revocation mechanisms that preserve authorized access while blocking revoked users
- Applied cryptographic primitives including symmetric/asymmetric encryption, HMACs, KDFs, and digital signatures in a threat-model-aware system
- Built entirely in Go as part of UC Berkeley’s CS161 (Computer Security)