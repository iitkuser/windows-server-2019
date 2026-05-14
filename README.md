# Reset Remote Desktop Terminal Services (PowerShell)

PowerShell script to restart and reset Remote Desktop Services (Terminal Services) on Windows systems.

---

## Features

- Stops Remote Desktop related services
- Restarts Terminal Services safely
- Clears stuck RDP sessions
- Helps fix:
  - Black screen on RDP
  - Frozen Remote Desktop sessions
  - Disconnected session issues
  - Terminal Services not responding

---

## Requirements

- Windows Server / Windows 10 / Windows 11
- Administrator privileges
- PowerShell 5.1 or later

---

## File


reset-remote-desktop-terminal-services.ps1
Run the Script
Step 1 — Open PowerShell as Administrator

Start Menu → Search PowerShell → Right Click → Run as Administrator

Step 2 — Allow Script Execution (If Blocked)

Run:

Set-ExecutionPolicy RemoteSigned -Scope Process

Press:

Y

when prompted.

Step 3 — Run the Script

Navigate to the script folder:

cd "C:\Path\To\Script"

Run:

.\reset-remote-desktop-terminal-services.ps1
Example
PS C:\Scripts> .\reset-remote-desktop-terminal-services.ps1
Common Fixes
Problem	Fixed
RDP black screen	✅
Session disconnected	✅
RDP stuck on loading	✅
Terminal Services frozen	✅
Multiple ghost sessions	✅
Important Notes
Running this script may disconnect active RDP users.
Always test in a non-production environment first.
Administrator access is required.
Troubleshooting
PowerShell script execution disabled

Error:

running scripts is disabled on this system

Fix:

Set-ExecutionPolicy RemoteSigned -Scope Process
Access Denied

Make sure PowerShell is opened as:

Run as Administrator
GitHub Usage

Clone repository:

git clone https://github.com/yourusername/reset-rdp-terminal-services.git

Enter folder:

cd reset-rdp-terminal-services

Run script:

.\reset-remote-desktop-terminal-services.ps1
License

MIT License

Author

Created for Windows Remote Desktop troubleshooting and automation.
