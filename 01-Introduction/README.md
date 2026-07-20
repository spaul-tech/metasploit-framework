# 🚀 Metasploit Framework

Welcome to my **Metasploit Framework** documentation repository.

This repository contains my notes, commands, modules, installation steps, and hands-on labs while learning the Metasploit Framework
for penetration testing and ethical hacking. It serves as a structured reference built through practice in authorized lab environments.

> ⚠️ **Disclaimer:** This repository is for educational purposes only. All testing is performed in authorized lab environments.

---

# 📥 Installation

> **Note:** Metasploit comes **pre-installed on Kali Linux**.

### 1. Update the system
```bash
sudo apt update && sudo apt upgrade -y
```

### 2. Install Metasploit (if not installed)
```bash
sudo apt install metasploit-framework -y
```

### 3. Start the PostgreSQL service
```bash
sudo systemctl start postgresql
```

### 4. Initialize the database
```bash
sudo msfdb init
```

### 5. Launch Metasploit
```bash
msfconsole
```

### 6. Verify the database connection
```bash
db_status
```

**Expected output:**
```text
[*] Connected to msf. Connection type: postgresql.
```
