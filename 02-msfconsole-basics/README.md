# ⚙️ msfconsole Basics

`msfconsole` is the primary command-line interface of the **Metasploit Framework**. It provides access to exploits, payloads, auxiliary modules, post-exploitation tools, and other framework features.

---

## 🚀 Launch msfconsole

> Make sure the PostgreSQL service is running before launching Metasploit.

```bash
sudo systemctl start postgresql
msfconsole
```

---

## 📌 Common Commands

| Command | Description |
|---------|-------------|
| `help` | Display all available commands |
| `version` | Show the installed Metasploit version |
| `banner` | Display a random Metasploit banner |
| `exit` | Exit msfconsole |
| `clear` | Clear the terminal screen |
| `history` | Show previously executed commands |
| `db_status` | Check the database connection status |

---

## 🔍 Searching Modules

```bash
search <keyword>
```

**Example:**
```bash
search smb
```

---

## 📂 Selecting a Module

```bash
use <module_path>
```

**Example:**
```bash
use exploit/windows/smb/ms17_010_eternalblue
```

---

## 📋 Display Information

```bash
info
```

Shows detailed information about the selected module.

---

## ⚙️ View Options

```bash
show options
```

Displays the required and optional parameters.

---

## 🎯 Set Options

```bash
set RHOSTS <target_ip>
set LHOST <your_ip>
set PAYLOAD <payload_name>
```

---

## 🚀 Run the Module

```bash
run
```

or

```bash
exploit
```

---

## 🔄 Background a Session

Press:

```text
Ctrl + Z
```

---

## 📌 View Active Sessions

```bash
sessions
```

Interact with a session:

```bash
sessions -i <session_id>
```

---

## ❌ Exit a Session

```bash
exit
```

or

```bash
background
```

to keep the session running.

---

## 💡 Tips

- Use `Tab` for auto-completion.
- Use `help <command>` to learn about a specific command.
- Run `show options` before executing a module.
- Verify the database connection with `db_status`.

> **Note:** Practice only in authorized environments such as TryHackMe, Hack The Box, or your own lab.
