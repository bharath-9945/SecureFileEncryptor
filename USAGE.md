# 📖 User Guide

This guide explains how to use **SecureFile Encryptor** to securely encrypt and decrypt files.

---

# 🚀 Starting the Application

After installing all dependencies, launch the application.

### Windows

```cmd
python main.py
```

or

```cmd
py main.py
```

### macOS / Linux

```bash
python3 main.py
```

---

# 🏠 Home Screen

After launching the application, you will see the main dashboard with the following options:

* 🔑 Generate Key
* 📂 Browse File
* 🔒 Encrypt File
* 🔓 Decrypt File
* 📁 Open Output Folder
* ⚙️ Settings
* ℹ️ About
* ❌ Exit

---

# 🔑 Generate a Secret Key

Before encrypting any file, a secret key must be generated.

### Steps

1. Open the application.
2. Click **Generate Key**.
3. The application creates a secure key.
4. The key is stored in:

```text
keys/secret.key
```

Expected Result:

```
✔ Secret Key Generated Successfully
```

> **Important:** Keep the secret key safe. Without it, encrypted files cannot be decrypted.

---

# 🔒 Encrypt a File

### Steps

1. Click **Browse File**.
2. Select any file.
3. Click **Encrypt**.
4. Wait for the encryption process to complete.

The encrypted file will be saved in:

```text
encrypted/
```

Example:

```text
encrypted/sample_text_20260723_143500.enc
```

Expected Result:

```
✔ File Encrypted Successfully
```

---

# 🔓 Decrypt a File

### Steps

1. Click **Browse File**.
2. Select an encrypted `.enc` file.
3. Click **Decrypt**.
4. Wait for the process to complete.

The decrypted file will be saved in:

```text
decrypted/
```

Example:

```text
decrypted/sample_text_20260723_143500.txt
```

Expected Result:

```
✔ File Decrypted Successfully
```

---

# 📂 Supported File Types

SecureFile Encryptor works with **any file type** because encryption is performed on raw binary data.

Examples:

* `.txt`
* `.pdf`
* `.docx`
* `.xlsx`
* `.pptx`
* `.jpg`
* `.png`
* `.gif`
* `.zip`
* `.rar`
* `.mp4`
* `.mp3`
* `.exe`
* `.json`
* `.csv`
* and many more.

---

# 🧪 Testing the Application

Follow these steps to verify that the application is working correctly.

### Test 1 – Generate Key

* Click **Generate Key**
* Verify that `keys/secret.key` is created.

---

### Test 2 – Encrypt Text File

Select:

```text
samples/sample_text.txt
```

Click:

```
Encrypt
```

Verify that a new encrypted file appears inside:

```text
encrypted/
```

---

### Test 3 – Encrypt JSON File

Select:

```text
samples/sample_config.json
```

Encrypt the file.

Confirm that another encrypted file is created.

---

### Test 4 – Verify Encryption

Open the encrypted file in a text editor.

The content should appear as unreadable encrypted data.

Example:

```text
gAAAAAB...
```

This confirms the file has been encrypted.

---

### Test 5 – Decrypt Files

Decrypt both encrypted files.

Verify that the decrypted files are created in:

```text
decrypted/
```

---

### Test 6 – Compare Files

Compare:

```text
Original File
```

with

```text
Decrypted File
```

Both files should be identical.

---

# 📊 Application Workflow

```text
Start Application
        │
        ▼
Generate / Load Secret Key
        │
        ▼
Browse File
        │
        ▼
Encrypt File
        │
        ▼
Save Encrypted File
        │
        ▼
Browse Encrypted File
        │
        ▼
Decrypt File
        │
        ▼
Save Restored File
        │
        ▼
Verify Integrity
        │
        ▼
Exit
```

---

# ⚠️ Best Practices

* Generate a new secret key only when needed.
* Store the secret key securely.
* Never share your secret key publicly.
* Keep backups of important encrypted files.
* Verify decrypted files before deleting originals.

---

# 📁 Output Directories

Generated Key

```text
keys/
```

Encrypted Files

```text
encrypted/
```

Decrypted Files

```text
decrypted/
```

Application Logs

```text
logs/
```

---

# 🛠 Troubleshooting

## Unable to Encrypt

* Ensure a secret key exists.
* Verify that the selected file is accessible.
* Check file permissions.

---

## Unable to Decrypt

Possible reasons:

* Incorrect secret key
* Corrupted encrypted file
* Invalid file selection

---

## Missing Dependencies

Reinstall dependencies:

```bash
pip install -r requirements.txt
```

---

# 📷 Screenshots

Add screenshots to:

```text
assets/screenshots/
```

Suggested screenshots:

* Home Screen
* Generate Key
* Encrypt File
* Decrypt File
* Settings
* About

---

# 🎉 Congratulations!

You have successfully learned how to use **SecureFile Encryptor** to securely encrypt and decrypt files while protecting sensitive information using modern cryptography.
