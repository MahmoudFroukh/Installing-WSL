# Installing-WSL

### 🐧 What is WSL?
- WSL stands for Windows Subsystem for Linux.
- It lets you run a Linux environment directly on Windows without using a virtual machine.
- You can use Linux tools, commands, and applications alongside Windows apps.
- Supports running Ubuntu, Debian, Kali, Fedora, and more.
- There are two versions: WSL 1 (simpler) and WSL 2 (faster, full Linux kernel support).

## 💡 Why use WSL?
- WSL is great for developers, sysadmins, and IT professionals who need quick access to Linux tools in Windows.
- Perfect for learning Linux or testing scripts without leaving your Windows setup.
- Simplifies workflows that require both Windows and Linux tools.

## ⚖️ Benefits over dual-booting or VMs
- ✅ Easier setup — fewer steps than configuring a VM or dual-boot.
- ✅ No reboot needed — use Linux and Windows simultaneously.
- ✅ Faster startup — WSL launches in seconds.
- ✅ Low resource usage — no need to allocate RAM or disk like in VMs.
- ✅ File system integration — access Windows files from Linux and vice versa.


## 🧪 Basic WSL commands
- `wsl` – Launches your default Linux distro.
- `wsl -l` – Lists installed Linux distributions.
- `wsl --install -d <distro>` – Installs a specific Linux distro.
- `wsl -d <distro>` – Runs a specific distribution.
- `wsl --set-default-version 2` – Sets WSL 2 as the default.
- `wsl --update` – Updates the WSL kernel.
- `wsl --status` – Shows WSL version info and default distro.
- `wsl --terminate <distro>` - Shutsdown the specified distro.
- `wsl --shutdown` - Shuts down all running distros.

## 🛠️ Common first-time setup tips
- Set up a user account when prompted after first launch.
- Once the Linux instance is launched, run: <pre> ```sudo apt update && sudo apt upgrade -y ``` </pre>
- All Linux files will be located here: `/home/yourusername/`
- All Windows files will be located here: `/mnt/c/Users/yourname/`

## 🔹 What you'll need
- Windows Terminal
- Windows 10 or higher
- x64 or ARM64
- Enable virtualization in BIOS/UEFI

## 📝 Steps
- Open **PowerShell as Administrator** and run: <pre> ```wsl --install ``` </pre>
- Verify that WSL is installed: <pre> ```wsl --status ``` </pre>
- See all the available Linux distributions: <pre> ```wsl --list --online ``` </pre>
- Install one: <pre> ```wsl --install -d <distro>``` </pre>
- You may need to restart your machine
- Run: <pre> ```wsl.exe -d <distro>``` </pre>
  ![Running a distro](https://github.com/user-attachments/assets/ec593fd2-4ad3-4822-abc2-5135dda530a1)

