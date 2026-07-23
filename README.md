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

Add screenshots inside:

```text
<img width="1280" height="775" alt="PHOTO-2026-07-23-09-43-32" src="https://github.com/user-attachments/assets/6178bf89-9e77-43a6-9219-93c94aec94c0" />
<img width="1280" height="771" alt="PHOTO-2026-07-23-09-44-32" src="https://github.com/user-attachments/assets/bc85d020-ad77-401d-8bea-c423ecf66c28" />
<img width="1280" height="754" alt="PHOTO-2026-07-23-09-45-45" src="https://github.com/user-attachments/assets/a4d4626f-66e9-44e5-9cd9-4e23e2778e30" />
```

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
