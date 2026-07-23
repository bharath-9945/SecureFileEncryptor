# ⚙️ Installation Guide

This guide explains how to install and run **SecureFile Encryptor** on **Windows**, **macOS**, and **Linux**.

---

# 📋 System Requirements

Before installing, ensure your system meets the following requirements:

* Python 3.12 or later
* pip (Python Package Manager)
* Git
* Internet connection (for downloading dependencies)

---

# 🪟 Windows Installation

## Step 1: Install Python

Download the latest version of Python from:

https://www.python.org/downloads/

During installation, make sure to enable:

* ✅ Add Python to PATH

Verify the installation:

```cmd
python --version
```

or

```cmd
py --version
```

Expected Output:

```text
Python 3.12.x
```

---

## Step 2: Install Git

Download Git from:

https://git-scm.com/downloads

Verify installation:

```cmd
git --version
```

---

## Step 3: Clone the Repository

```cmd
git clone https://github.com/YOUR_USERNAME/SecureFileEncryptor.git
```

---

## Step 4: Navigate to the Project

```cmd
cd SecureFileEncryptor
```

---

## Step 5: Create a Virtual Environment (Recommended)

```cmd
python -m venv venv
```

---

## Step 6: Activate the Virtual Environment

### Command Prompt

```cmd
venv\Scripts\activate
```

### PowerShell

```powershell
.\venv\Scripts\Activate.ps1
```

If PowerShell blocks activation:

```powershell
Set-ExecutionPolicy -Scope Process RemoteSigned
```

Then activate again.

---

## Step 7: Install Required Packages

```cmd
pip install -r requirements.txt
```

---

## Step 8: Run the Application

```cmd
python main.py
```

---

# 🍎 macOS Installation

## Step 1: Install Homebrew (If Not Installed)

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

---

## Step 2: Install Python

```bash
brew install python
```

Verify installation:

```bash
python3 --version
```

---

## Step 3: Install Git

```bash
brew install git
```

Verify:

```bash
git --version
```

---

## Step 4: Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/SecureFileEncryptor.git
```

---

## Step 5: Navigate to the Project

```bash
cd SecureFileEncryptor
```

---

## Step 6: Create a Virtual Environment

```bash
python3 -m venv venv
```

---

## Step 7: Activate the Environment

```bash
source venv/bin/activate
```

---

## Step 8: Upgrade pip

```bash
python3 -m pip install --upgrade pip
```

---

## Step 9: Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Step 10: Run the Application

```bash
python3 main.py
```

---

# 🐧 Linux Installation (Ubuntu/Debian)

## Step 1: Update Packages

```bash
sudo apt update
```

---

## Step 2: Install Required Software

```bash
sudo apt install python3 python3-pip python3-venv python3-tk git -y
```

---

## Step 3: Verify Installation

```bash
python3 --version
```

```bash
pip3 --version
```

```bash
git --version
```

---

## Step 4: Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/SecureFileEncryptor.git
```

---

## Step 5: Navigate to the Project

```bash
cd SecureFileEncryptor
```

---

## Step 6: Create a Virtual Environment

```bash
python3 -m venv venv
```

---

## Step 7: Activate the Virtual Environment

```bash
source venv/bin/activate
```

---

## Step 8: Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Step 9: Run the Application

```bash
python3 main.py
```

---

# 📦 Required Python Packages

These packages are automatically installed from **requirements.txt**.

```
cryptography
customtkinter
tkinterdnd2
```

---

# 🔍 Verify Installation

If everything is installed correctly, the application should launch successfully with:

* Modern GUI
* Sidebar Navigation
* Generate Key Button
* Encrypt Button
* Decrypt Button

---

# ❗ Troubleshooting

## Python Not Found

Windows

```cmd
python --version
```

If not found, reinstall Python and enable **Add Python to PATH**.

---

## Git Not Found

```bash
git --version
```

Install Git from:

https://git-scm.com/

---

## Missing Dependency

```bash
pip install -r requirements.txt
```

---

## Virtual Environment Issues

Deactivate:

```bash
deactivate
```

Delete the existing environment and create a new one:

Windows

```cmd
rmdir /s /q venv
```

Linux/macOS

```bash
rm -rf venv
```

Create a new environment:

```bash
python -m venv venv
```

or

```bash
python3 -m venv venv
```

---

# 🎉 Installation Complete

Your SecureFile Encryptor application is now ready to use.

