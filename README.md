# Reset Remote Desktop Terminal Services (PowerShell)

PowerShell script to restart and reset Remote Desktop Services (Terminal Services) on Windows systems.

---

## Features

- Stops Remote Desktop related services
- Restarts Terminal Services safely
- Clears stuck RDP sessions
- Fixes common RDP issues:
  - Black screen
  - Frozen session
  - Stuck login
  - Session disconnects
  - Unresponsive Terminal Services

---

## Requirements

- Windows 10 / Windows 11 / Windows Server
- Administrator privileges
- PowerShell 5.1+

---

# Run the Script

## Step 1 — Open PowerShell as Administrator

- Press `Start`
- Search for `PowerShell`
- Right-click **Windows PowerShell**
- Click **Run as Administrator**

---

## Step 2 — Bypass PowerShell Execution Policy

Run the following command:

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force
```

---

## Step 3 — Navigate to Script Folder

Example:

```powershell
cd "C:\Scripts"
```

---

## Step 4 — Run the Script

```powershell
.\reset-remote-desktop-terminal-services.ps1
```

---

# One-Line Quick Run

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force
cd "C:\Scripts"
.\reset-remote-desktop-terminal-services.ps1
```

---

## Example

```powershell
PS C:\Scripts> .\reset-remote-desktop-terminal-services.ps1
```

---

## Common Issues Fixed

| Issue | Status |
|---|---|
| RDP black screen | ✅ |
| Frozen Remote Desktop | ✅ |
| Stuck login screen | ✅ |
| Session disconnects | ✅ |
| Terminal Services hanging | ✅ |

---

## Troubleshooting

### Script Execution Disabled

Error:

```text
running scripts is disabled on this system
```

Fix:

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force
```

---

### Access Denied

Run PowerShell as Administrator.

---

## GitHub Usage

Clone repository:

```bash
git clone https://github.com/yourusername/reset-rdp-terminal-services.git
```

Open PowerShell:

```powershell
cd reset-rdp-terminal-services
Set-ExecutionPolicy Bypass -Scope Process -Force
.\reset-remote-desktop-terminal-services.ps1
```

---

## Warning

Running this script may disconnect active RDP users.

Use carefully on production servers.

---

## License

MIT License
