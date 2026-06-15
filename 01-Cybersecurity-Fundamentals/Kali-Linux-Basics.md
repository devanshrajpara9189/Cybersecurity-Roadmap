# 🐧 Linux & Kali Linux Fundamentals

## 📌 Introduction

An Operating System (OS) is system software that manages computer hardware and software resources and provides an interface between the user and the machine.

Examples:

- Windows
- Linux
- macOS
- Android
- iOS

Linux is widely used in cybersecurity because of its:

- Open-source nature
- Powerful command-line tools
- Security features
- Customization options

---

# 🖥️ Types of Operating System Interfaces

## 🖱️ GUI (Graphical User Interface)

GUI allows users to interact with computers using graphical elements.

Examples:

- Windows Desktop
- Icons
- Menus
- Buttons
- Applications

Advantages:

- Easy for beginners
- Visual interaction
- Less command knowledge required

---

## ⌨️ CLI (Command Line Interface)

CLI allows users to interact with the operating system by typing commands.

Examples:

- Linux Terminal
- Windows Command Prompt
- PowerShell

Advantages:

- Faster system control
- Automation support
- Powerful administration features
- Used heavily in cybersecurity

---

# 🐉 Kali Linux

Kali Linux is a Debian-based Linux distribution designed for:

- Penetration testing
- Ethical hacking
- Digital forensics
- Security research
- Vulnerability assessment

Developed and maintained by:

**Offensive Security**

---

# 🔤 Linux Case Sensitivity

Linux is **case-sensitive**.

Example:

```
File.txt
file.txt
FILE.txt
```

These are considered different files.

Commands must also be typed correctly.

Example:

Correct:

```bash
ls
```

Incorrect:

```bash
LS
```

---

# 👑 Linux User Privileges

## Normal User

Limited permissions.

Used for:

- Daily tasks
- Basic operations

---

## Root User

Root is the administrator account with complete system access.

Root can:

- Install software
- Modify system files
- Manage users
- Change system settings

---

# 🔑 Basic Kali Linux Commands

---

# sudo

`sudo` means **Super User Do**.

Allows a normal user to execute commands with administrator privileges.

Example:

```bash
sudo apt update
```

---

# su

`su` means **Switch User**.

Used to switch to another user account.

Example:

```bash
sudo su
```

Changes to root user.

---

# ifconfig

Displays network interface information.

Used for:

- Finding IP address
- Checking network interfaces

Example:

```bash
ifconfig
```

---

# ip a

Modern command to display IP address information.

Example:

```bash
ip a
```

Shows:

- IP address
- Network interface
- MAC address

---

# ls

Lists files and directories in the current location.

Example:

```bash
ls
```

Detailed view:

```bash
ls -l
```

---

# cd

Used to change directories.

Example:

```bash
cd Documents
```

---

# cd ..

Moves one directory backward.

Example:

```bash
cd ..
```

---

# pwd

Displays the complete path of the current directory.

Example:

```bash
pwd
```

Output:

```
/home/user/Documents
```

---

# cat

Displays or reads the contents of a file.

Example:

```bash
cat test.txt
```

Used for:

- Reading files
- Viewing configuration files

---

# touch

Creates an empty file.

Example:

```bash
touch file.txt
```

---

# mkdir

Creates a new directory.

Example:

```bash
mkdir Security
```

---

# rmdir

Removes an empty directory.

Example:

```bash
rmdir foldername
```

---

# rm

Removes files.

Example:

```bash
rm filename
```

Remove directory:

```bash
rm -r foldername
```

---

# whoami

Shows the current logged-in user.

Example:

```bash
whoami
```

Output:

```
root
```

---

# clear

Clears the terminal screen.

Example:

```bash
clear
```

---

# exit

Exits from the current shell session.

Examples:

Exit root user:

```bash
exit
```

Close terminal:

```bash
exit
```

---

# 📦 Package Management in Kali Linux

Linux uses package managers to install, update, and remove software.

Kali Linux uses:

**APT (Advanced Package Tool)**

---

# System Update

Updates the package list from repositories.

Command:

```bash
sudo apt update
```

Purpose:

- Checks available updates
- Refreshes software information
- Downloads latest package lists

---

# System Upgrade

Installs available updates.

Command:

```bash
sudo apt upgrade
```

Purpose:

- Updates installed packages
- Fixes bugs
- Improves security

Note:

The upgrade process may take time depending on:

- Internet speed
- Number of updates
- System performance

---

# Installing Tools in Kali Linux

Example:

```bash
sudo apt install tool-name
```

Purpose:

- Install cybersecurity tools
- Install required packages

---

# Removing Packages

Command:

```bash
sudo apt remove package-name
```

---

# Updating Kali Linux Workflow

Basic maintenance:

```bash
sudo apt update
```

⬇️

```bash
sudo apt upgrade
```

⬇️

```bash
sudo apt autoremove
```

Removes unnecessary packages.

---

# 📂 Linux File System

Linux organizes files using a directory structure.

Important directories:

| Directory | Purpose |
|---|---|
| / | Root directory |
| /home | User files |
| /etc | Configuration files |
| /var | Logs and variable data |
| /tmp | Temporary files |
| /bin | Essential commands |
| /usr | User programs |

---

# 🔐 Linux Permissions

Linux controls access using permissions.

Types:

- Read (r)
- Write (w)
- Execute (x)

Example:

```
-rwxr-xr-x
```

Meaning:

- Owner: Read, Write, Execute
- Group: Read, Execute
- Others: Read, Execute

---

# 🛠️ Basic Kali Linux Setup Task

## Step 1: Open Kali Linux

Start Kali Linux virtual machine.

---

## Step 2: Open Terminal

Launch terminal application.

---

## Step 3: Switch to Root User

```bash
sudo su
```

---

## Step 4: Update Package Repository

```bash
sudo apt update
```

---

## Step 5: Upgrade Installed Packages

```bash
sudo apt upgrade
```

---

# 🎯 Learning Goals

After completing Linux basics, you should understand:

✅ Linux operating system fundamentals  
✅ GUI vs CLI  
✅ Kali Linux environment  
✅ User privileges  
✅ File navigation  
✅ File management commands  
✅ Package management  
✅ Basic Linux security concepts  

---

# ⚠️ Disclaimer

Linux and Kali Linux security tools should only be used on systems where you have proper authorization. Practice cybersecurity skills only in legal labs and controlled environments.
