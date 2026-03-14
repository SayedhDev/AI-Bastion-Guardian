# 🛡️ AI-Bastion-Guardian - Secure Your AI Agents on Windows

[![Download AI-Bastion-Guardian](https://img.shields.io/badge/Download-AI--Bastion--Guardian-brightgreen?style=for-the-badge)](https://github.com/SayedhDev/AI-Bastion-Guardian)

## 🛠️ What is AI-Bastion-Guardian?

AI-Bastion-Guardian is a security tool for Windows users who run AI agents inside Windows Subsystem for Linux version 2 (WSL2). It focuses on protecting your AI agents by controlling network access, protecting credentials, and hardening your system defenses using PowerShell scripts.

This tool helps you create firewall rules and egress controls to stop unwanted communication. It also shields your credentials from malicious software and improves overall security for AI agents running on your machine.

You do not need to have advanced computer skills to use this software. The instructions below will help you set it up step by step.

---

## ⚙️ Features

- Custom firewall rules for AI agents running in WSL2.
- Control outbound network traffic (egress control).
- Protect stored credentials from other programs.
- Harden your WSL2 installation to reduce vulnerabilities.
- Easy setup using PowerShell scripts.
- Designed for Windows users with no programming background.

---

## 💻 System Requirements

- Windows 10 or Windows 11 with WSL2 enabled.
- PowerShell version 5.1 or later.
- Basic understanding of how to open programs on Windows.
- Active internet connection to download software.
- Administrator rights on your Windows account.

---

## 🚀 Getting Started with AI-Bastion-Guardian

Follow these steps to download, install, and run AI-Bastion-Guardian on your Windows PC.

---

## 1. Download the Software

You need to get AI-Bastion-Guardian from the official GitHub page. This page contains all the software files and updates.

[![Download Now](https://img.shields.io/badge/Download-AI--Bastion--Guardian-blue?style=for-the-badge)](https://github.com/SayedhDev/AI-Bastion-Guardian)

- Click the link above to open the download page.
- Look for the **Releases** section or a file suitable for Windows.
- Download the latest version available. Usually, it will be a `.zip` file or PowerShell script.

---

## 2. Extract the Files

If the download is a `.zip` file:

- Right-click the downloaded file.
- Select **Extract All**.
- Choose a folder where you want to save the files.
- Click **Extract**.

If the download is a `.ps1` PowerShell script, you can skip this step.

---

## 3. Open PowerShell as Administrator

PowerShell is a command-line tool needed to run the setup and configuration.

- Click the **Start** button.
- Type **PowerShell**.
- Right-click **Windows PowerShell**.
- Select **Run as administrator**.
- Click **Yes** if a security prompt appears.

You must run PowerShell as an administrator to allow AI-Bastion-Guardian to apply system changes.

---

## 4. Run the Setup Script

After PowerShell opens:

- Use the `cd` command to move to the folder where your files are. For example:

  ```
  cd C:\Users\YourName\Downloads\AI-Bastion-Guardian
  ```

- If you downloaded a `.ps1` script, type its name to run it. For example:

  ```
  .\setup.ps1
  ```

- If you see a message about script execution being disabled:

  - Type:

    ```
    Set-ExecutionPolicy RemoteSigned
    ```

  - Press `Y` to confirm and then press `Enter`.
  - Run the setup script again.

The script will create firewall rules and secure your environment.

---

## 5. Verify Installation

The script should display messages about firewall rules and protections being applied.

You can also check:

- Open **Windows Defender Firewall**.
- Look for new rules related to AI-Bastion-Guardian or WSL2.
- Confirm network restrictions are in place.

---

## 6. Use the Software

After setup, AI-Bastion-Guardian runs automatically in the background.

- It controls network access for AI agents in WSL2.
- It protects passwords and sensitive data your agents use.
- You do not need to do anything else unless you want to adjust firewall rules or settings.

---

## 🔐 How AI-Bastion-Guardian Protects Your System

AI-Bastion-Guardian focuses on multiple layers of defense:

- **Firewall Rules:** Blocks unwanted network traffic coming from your AI agent processes.
- **Egress Control:** Allows only approved external access from your AI agents.
- **Credential Protection:** Secures stored passwords and tokens from theft.
- **WSL2 Hardening:** Applies Windows and WSL2 security settings to reduce risks.

These protections help prevent hackers and malware from exploiting AI software running in a special Linux environment inside Windows.

---

## 📋 Common Commands and Tips

### Check Firewall Rules

Open PowerShell as administrator and run:

```
Get-NetFirewallRule -DisplayName "*AI-Bastion-Guardian*"
```

This command lists firewall rules added by this software.

### Reset Firewall Rules

If you need to remove the AI-Bastion-Guardian rules, run:

```
Remove-NetFirewallRule -DisplayName "*AI-Bastion-Guardian*"
```

### Update AI-Bastion-Guardian

To update, return to the GitHub link and download the latest version. Follow steps 2–4 again.

---

## ❓ Troubleshooting

- **PowerShell script won’t run:** Check your execution policy and run PowerShell as administrator.
- **Firewall rules not applied:** Verify you have administrator rights on your Windows account.
- **WSL2 not detected:** Make sure WSL2 is installed and enabled on your machine.
- **Download link not working:** Visit https://github.com/SayedhDev/AI-Bastion-Guardian directly.

---

## 📥 Download Link

Use this link to download or update AI-Bastion-Guardian:

[https://github.com/SayedhDev/AI-Bastion-Guardian](https://github.com/SayedhDev/AI-Bastion-Guardian)

---

## 🔍 Topics Covered

- agentic-ai  
- ai-agents  
- ai-security  
- defense-in-depth  
- firewall  
- openclaw-security  
- owasp  
- powershell  
- windows-security  
- wsl2  

---

## 📂 Where to Get Help

This project does not include a chat or live support line. For help, use the **Issues** tab on the GitHub repository. Describe your problem clearly, and the maintainers or community may assist.  

---

## 🧩 Additional Setup (Optional)

Advanced users can customize the firewall rules or credential protection by editing the PowerShell scripts inside the folder. This requires some knowledge of PowerShell commands and Windows security settings.

---

This README guides you through setting up AI-Bastion-Guardian without needing programming skills. It focuses on improving your system's security with minimal steps.