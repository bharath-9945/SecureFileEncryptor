# ❓ Frequently Asked Questions (FAQ)

This document answers common questions about **SecureFile Encryptor**.

---

# General Questions

## 1. What is SecureFile Encryptor?

SecureFile Encryptor is a Python-based desktop application that securely encrypts and decrypts files using the **Cryptography (Fernet)** library. It helps protect sensitive data from unauthorized access.

---

## 2. Why was this project developed?

The project was developed as a cybersecurity learning project to demonstrate practical implementation of modern cryptography, secure file handling, and desktop application development.

---

## 3. Which encryption algorithm is used?

The application uses **Fernet**, which provides authenticated symmetric encryption using AES-128 in CBC mode with HMAC authentication.

---

## 4. Which programming language is used?

Python 3.12+

---

## 5. Which GUI framework is used?

CustomTkinter (with Tkinter compatibility where applicable).

---

# Security Questions

## 6. Is my data secure?

Yes. Files are encrypted using the Fernet algorithm, making them unreadable without the correct secret key.

---

## 7. Is the secret key hardcoded?

No. A new key is generated at runtime and stored separately in the `keys/` directory.

---

## 8. What happens if I lose the secret key?

Encrypted files cannot be decrypted without the correct key. Keep your key backed up securely.

---

## 9. Can I use the same key for multiple files?

Yes. One generated key can encrypt and decrypt multiple files.

---

## 10. Can someone read an encrypted file?

No. Encrypted files contain unreadable ciphertext and require the correct key to restore the original content.

---

# Usage Questions

## 11. What file types are supported?

The application supports any file type because it encrypts the raw binary content, including:

* TXT
* PDF
* DOCX
* XLSX
* PPTX
* JPG
* PNG
* ZIP
* JSON
* MP4
* MP3
* and many others.

---

## 12. Where are encrypted files stored?

```text
encrypted/
```

---

## 13. Where are decrypted files stored?

```text
decrypted/
```

---

## 14. Where is the secret key stored?

```text
keys/secret.key
```

---

## 15. Does the application overwrite files?

No. Timestamped filenames are generated to avoid overwriting existing files.

---

# Installation Questions

## 16. Which operating systems are supported?

* Windows
* macOS
* Linux

---

## 17. What Python version is required?

Python 3.12 or later.

---

## 18. Which dependencies are required?

* cryptography
* customtkinter
* tkinterdnd2

---

## 19. How do I install dependencies?

```bash
pip install -r requirements.txt
```

---

## 20. How do I start the application?

Windows:

```bash
python main.py
```

macOS/Linux:

```bash
python3 main.py
```

---

# Troubleshooting

## 21. Why can't I decrypt my file?

Possible reasons include:

* Incorrect secret key
* Corrupted encrypted file
* Wrong file selected

---

## 22. Why is my encrypted file unreadable?

This is expected. Encryption converts readable data into ciphertext to protect it.

---

## 23. What should I do if the application doesn't start?

* Verify your Python installation.
* Install all required dependencies.
* Ensure you're running `main.py` from the project directory.

---

## 24. How can I verify encryption worked?

Encrypt a sample file, then decrypt it using the same key. The decrypted file should match the original exactly.

---

## 25. Can this project be extended?

Yes. Possible enhancements include:

* Password-based encryption
* Folder encryption
* Batch processing
* Cloud integration
* User authentication
* File integrity verification
* Digital signatures
* Multi-language support

---

# Need More Help?

If you encounter any issues:

1. Review the installation guide.
2. Check the application logs.
3. Open a GitHub Issue with details about your environment and the error.

Thank you for using **SecureFile Encryptor**!
