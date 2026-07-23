# 🔄 Project Workflow

This document explains the complete workflow, architecture, and internal working of **SecureFile Encryptor**.

---

# 📖 Overview

SecureFile Encryptor is a desktop-based cybersecurity application that allows users to securely encrypt and decrypt files using the **Fernet symmetric encryption algorithm** from the Python Cryptography library.

The application ensures that only users with the correct secret key can restore encrypted files.

---

# 🎯 Project Objective

The objective of this project is to provide a simple, secure, and user-friendly desktop application for protecting sensitive files through encryption while demonstrating practical cryptography concepts.

---

# 🏗️ System Architecture

```text
                 +----------------------+
                 |      User            |
                 +----------+-----------+
                            |
                            ▼
                 +----------------------+
                 |  CustomTkinter GUI   |
                 +----------+-----------+
                            |
        +-------------------+-------------------+
        |                   |                   |
        ▼                   ▼                   ▼
+---------------+   +----------------+   +----------------+
| Key Manager   |   | File Utilities |   | Logging Module |
+-------+-------+   +--------+-------+   +----------------+
        |                     |
        ▼                     ▼
+---------------+     +----------------+
| Encryption    |     | Decryption     |
| (Fernet)      |     | (Fernet)       |
+-------+-------+     +--------+-------+
        |                      |
        ▼                      ▼
 encrypted/              decrypted/
```

---

# 📂 Module Workflow

## 1. Application Startup

* User launches the application.
* Required folders are verified or created.
* Logging is initialized.
* Existing encryption key is checked.

---

## 2. Key Management

The user can:

* Generate a new secret key.
* Load an existing key.
* Validate the key format.
* Store the key securely in:

```text
keys/secret.key
```

---

## 3. File Selection

The application allows users to browse and select any file from their system.

Supported examples include:

* Text documents
* PDFs
* Images
* Videos
* ZIP archives
* JSON files
* Office documents

The selected file's information is displayed, including:

* File name
* File size
* File type
* File path

---

## 4. Encryption Process

When the **Encrypt** button is clicked:

1. The selected file is opened in binary mode.
2. The secret key is loaded.
3. Fernet encrypts the file contents.
4. A timestamped filename is generated.
5. The encrypted file is saved in:

```text
encrypted/
```

Example:

```text
sample_text_20260723_103000.enc
```

A success message is displayed.

---

## 5. Encrypted File Verification

Encrypted files contain unreadable binary data.

Example:

```text
gAAAAABpJ...
```

This confirms that the original content has been successfully protected.

---

## 6. Decryption Process

When the **Decrypt** button is clicked:

1. The encrypted file is selected.
2. The secret key is loaded.
3. Fernet verifies the key.
4. The encrypted content is decrypted.
5. The original file is restored.
6. The restored file is saved inside:

```text
decrypted/
```

Example:

```text
sample_text_20260723_103000.txt
```

---

## 7. Integrity Verification

The decrypted file should exactly match the original file.

Verification methods include:

* Opening both files manually.
* Comparing file sizes.
* Byte-by-byte comparison using Python.

Expected result:

```text
Original File == Decrypted File
```

---

# 🔄 Complete Workflow Diagram

```text
Start
   │
   ▼
Launch Application
   │
   ▼
Generate or Load Secret Key
   │
   ▼
Browse File
   │
   ▼
Display File Information
   │
   ▼
Encrypt File
   │
   ▼
Save Encrypted File
   │
   ▼
Select Encrypted File
   │
   ▼
Decrypt File
   │
   ▼
Restore Original File
   │
   ▼
Verify Integrity
   │
   ▼
End
```

---

# 📁 Folder Usage

| Folder       | Purpose                           |
| ------------ | --------------------------------- |
| `keys/`      | Stores the generated secret key   |
| `encrypted/` | Stores encrypted output files     |
| `decrypted/` | Stores decrypted output files     |
| `samples/`   | Contains sample files for testing |
| `logs/`      | Stores application log files      |
| `assets/`    | Images, icons, and screenshots    |

---

# 🔐 Security Workflow

* Generate a secure Fernet key.
* Store the key separately from encrypted data.
* Encrypt file contents.
* Save encrypted output with timestamped filenames.
* Prevent decryption using invalid keys.
* Restore original data only with the correct key.
* Log application events and errors.

---

# 🧪 Testing Workflow

1. Generate a secret key.
2. Encrypt `sample_text.txt`.
3. Encrypt `sample_config.json`.
4. Verify encrypted files are unreadable.
5. Decrypt both encrypted files.
6. Compare decrypted files with the originals.
7. Confirm that all tests pass successfully.

---

# 📈 Future Improvements

* Password-based encryption.
* Folder encryption.
* Batch file encryption.
* Cloud storage integration.
* File hash verification (SHA-256).
* Multi-language support.
* Automatic updates.
* User authentication.
* Secure key backup and recovery.

---

# ✅ Conclusion

SecureFile Encryptor demonstrates how modern cryptographic techniques can be integrated into a desktop application to protect sensitive data. The project combines secure key management, robust encryption, intuitive user interface design, and cross-platform compatibility, making it a practical cybersecurity learning project and a strong portfolio piece.
