# 📦 Modules

A **module** is a reusable component in the Metasploit Framework that performs a specific task, such as exploiting a vulnerability, scanning a target, generating a payload, or performing post-exploitation.

Metasploit organizes modules into different categories based on their functionality.

---

## 📂 Module Types

| Module Type | Description |
|-------------|-------------|
| **Exploit** | Takes advantage of a vulnerability on a target system. |
| **Auxiliary** | Performs scanning, enumeration, fuzzing, and other tasks without exploiting a vulnerability. |
| **Payload** | Executes code on the target after successful exploitation. |
| **Post** | Performs post-exploitation tasks such as gathering credentials, system information, and privilege escalation. |
| **Encoder** | Encodes payloads to help avoid simple detection or bad characters. |
| **NOP** | Generates No Operation (NOP) instructions used in payloads. |

---

## 📁 Module Path

Every module has a unique path.

**Example:**

```text
exploit/windows/smb/ms17_010_eternalblue
```

### Breakdown

| Part | Meaning |
|------|---------|
| `exploit` | Module type |
| `windows` | Target platform |
| `smb` | Target service/protocol |
| `ms17_010_eternalblue` | Module name |

---

## 🔍 Searching Modules

Search by keyword:

```bash
search smb
```

Search by module type:

```bash
search type:exploit
search type:auxiliary
search type:payload
search type:post
```

Search by platform:

```bash
search platform:windows
search platform:linux
```

Search by module name or vulnerability:

```bash
search ms17-010
```

---

## 📌 Module Information

Display detailed information about a module:

```bash
info exploit/windows/smb/ms17_010_eternalblue
```

or after selecting the module:

```bash
info
```

---

## 📥 Load a Module

```bash
use exploit/windows/smb/ms17_010_eternalblue
```

After loading, the prompt changes to indicate the selected module:

```text
msf6 exploit(windows/smb/ms17_010_eternalblue) >
```

---

> **Note:** Practice Metasploit modules only in authorized environments such as TryHackMe, Hack The Box, or your own lab.
