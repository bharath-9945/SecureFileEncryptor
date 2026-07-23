# Security Policy

## Overview

The security of **SecureFile Encryptor** is a top priority. This document explains how to responsibly report security vulnerabilities and outlines the project's security practices.

---

# Supported Versions

The following versions currently receive security updates.

| Version | Supported |
| ------- | --------- |
| 1.0.x   | ✅ Yes     |
| < 1.0   | ❌ No      |

---

# Reporting a Security Vulnerability

If you discover a security vulnerability, **please do not create a public GitHub Issue**.

Instead:

1. Prepare a detailed description of the vulnerability.
2. Include steps to reproduce the issue.
3. Describe the potential impact.
4. If possible, suggest a mitigation or fix.
5. Contact the project maintainer privately.

Please include:

* Operating System
* Python Version
* Project Version
* Error Logs (if available)
* Screenshots (if applicable)

We aim to acknowledge vulnerability reports within **5 business days** and investigate them as quickly as possible.

---

# Responsible Disclosure

We appreciate responsible disclosure of security issues.

Please:

* Allow reasonable time for investigation before publicly disclosing the issue.
* Avoid sharing proof-of-concept exploits that could harm users.
* Provide enough information to reproduce the issue.

---

# Security Best Practices

To use SecureFile Encryptor safely:

* Keep your **secret key** confidential.
* Never upload your `secret.key` file to GitHub or other public repositories.
* Back up your secret key in a secure location.
* Verify the source of files before encrypting or decrypting them.
* Regularly update Python and project dependencies.
* Use a virtual environment for development.

---

# Current Security Features

SecureFile Encryptor includes:

* Fernet-based authenticated encryption
* Secure runtime key generation
* Separate key storage
* Timestamped output filenames
* Invalid key detection during decryption
* Exception handling to prevent application crashes
* Logging for troubleshooting
* Cross-platform compatibility

---

# Known Limitations

* The application uses symmetric encryption, so the same key is required for encryption and decryption.
* Loss of the secret key will make encrypted files unrecoverable.
* Users are responsible for securely storing and backing up their keys.

---

# Future Security Improvements

Planned enhancements include:

* Password-derived key generation
* SHA-256 file integrity verification
* Digital signatures
* Secure key backup and recovery
* Multi-factor authentication for key access
* Batch encryption with integrity checks

---

# Dependency Security

Keep dependencies updated:

```bash
pip install --upgrade -r requirements.txt
```

You can also check for outdated packages:

```bash
pip list --outdated
```

---

# Contact

If you believe you have found a security issue, please contact the project maintainer privately before making the issue public.

Thank you for helping improve the security of **SecureFile Encryptor**.
