# 🔐 SecureFile Encryptor

> A modern Python desktop application for secure file encryption and decryption using the **Cryptography (Fernet)** library and **CustomTkinter**.

---

## 📖 Table of Contents

* About
* Features
* Project Workflow
* Folder Structure
* Technologies Used
* Installation
* Usage
* Testing
* Screenshots
* Future Enhancements
* License
* Developer

---

# 🌟 About

SecureFile Encryptor is a cybersecurity desktop application developed using **Python**. The application securely encrypts and decrypts files using the **Fernet symmetric encryption algorithm** provided by the Cryptography library.

It provides an easy-to-use graphical interface for protecting sensitive files from unauthorized access while maintaining data confidentiality and integrity.

---

# ✨ Features

* 🔐 Secure File Encryption
* 🔓 Secure File Decryption
* 🔑 Secret Key Generation
* 📂 File Browser
* 📄 Supports Multiple File Types
* 🖥️ Modern CustomTkinter GUI
* 📊 Progress Bar
* 📝 Activity Logging
* ⚠️ Error Handling
* 📅 Timestamped Output Files
* 🛡️ Secure Key Management
* 🌙 Dark Theme
* 💻 Cross Platform Support

---

# 🔄 Project Workflow

```text
Start
   │
   ▼
Generate / Load Secret Key
   │
   ▼
Select File
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
End
```

---

# 📂 Project Structure

```text
SecureFileEncryptor/

├── main.py
├── gui.py
├── encryption.py
├── decryption.py
├── key_manager.py
├── file_utils.py
├── requirements.txt
├── README.md
├── LICENSE

├── assets/
├── keys/
├── encrypted/
├── decrypted/
├── samples/
└── logs/
```

---

# 🛠️ Technologies Used

| Technology            | Purpose                  |
| --------------------- | ------------------------ |
| Python 3.12+          | Programming Language     |
| CustomTkinter         | Desktop GUI              |
| Cryptography (Fernet) | File Encryption          |
| Logging               | Activity Logs            |
| OOP                   | Application Architecture |

---

# ⚙️ Installation

See:

📄 **docs/INSTALL.md**

---

# ▶️ Usage

See:

📄 **docs/USAGE.md**

---

# 🧪 Testing

Test the application using the following steps:

* Generate a Secret Key
* Encrypt sample_text.txt
* Encrypt sample_config.json
* Verify encrypted files are unreadable
* Decrypt both files
* Compare decrypted files with the originals

Expected Result:

✅ Original and decrypted files should be identical.

---

# 📷 Screenshots


Recommended screenshots:

* Home Screen
* Generate Key
* Encrypt File
* Decrypt File
* About Page

---

# 🚀 Future Enhancements

* Password-based Encryption
* Folder Encryption
* Multiple File Encryption
* Drag & Drop Improvements
* Cloud Storage Support
* AES-256 Password-Derived Keys
* File Integrity Verification
* User Authentication

---

# 📄 License

This project is licensed under the MIT License.

---

# 👨‍💻 Developer

**Bharath Kumar Reddy**

Cybersecurity Intern

Project:

**SecureFile Encryptor**

Intern ID:

**AB21**

---

⭐ If you found this project useful, please consider giving it a star on GitHub.
