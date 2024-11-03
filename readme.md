# ❄️ Arch Linux on WSL

This repository provides the necessary steps to download and install Arch Linux on Windows Subsystem for Linux (WSL) from GitHub.

## 📋 Requirements

1. 🖥️ **Windows 10/11** with WSL enabled.
2. 🛠️ **Git** installed on Windows.
3. ✅ **WSL** enabled on your system (either WSL 1 or WSL 2).

## 🚀 Installation Steps

### 1. Enable WSL on Windows

If WSL is not enabled on your system, open PowerShell as Administrator and run:

```bash
wsl --install
```

After installation, restart your computer if prompted. 🔄

### 2. Clone the Repository

Clone this repository to your local machine by running the following command in a terminal or PowerShell:

```bash
git clone https://github.com/who-icyy/archlinuxwsl.git
cd archlinux-wsl
```

### 3. Run the Installation Script

1. Open PowerShell or Command Prompt as Administrator. ⚡
2. Navigate to the cloned repository directory.
3. Run the installation script:

```bash
wsl --import ArchLinux <path> archlinux-wsl.tar.gz
# For example:
wsl --import ArchLinux C:\WSL\ArchLinux archlinux-wsl.tar.gz
```

This command installs Arch Linux from the provided `archlinux-wsl.tar.gz` file. 📦

### 4. Configure Arch Linux

Start your Arch Linux installation:

```bash
wsl -d ArchLinux
```

After entering the Arch Linux environment, set up your initial configuration by updating the package manager and installing essential packages:

```bash
sudo pacman -Syu
```

You can now customize and use your Arch Linux environment on WSL! 🎉

### 🌟 Optional: Setting Arch Linux as Default WSL Distribution

If you'd like to set Arch Linux as your default WSL distribution, run:

```bash
wsl --set-default ArchLinux
```

### 🔧 Additional Configuration (Optional)

1. Install commonly used tools:

   ```bash
   sudo pacman -S base-devel vim git
   ```

2. Set up additional configurations or packages as per your requirements.

## 🗑️ Uninstalling Arch Linux from WSL

To remove Arch Linux from WSL, run:

```powershell
wsl --unregister ArchLinux
```

This will delete the Arch Linux instance from WSL.

## ❓ Troubleshooting

If you encounter issues during installation, ensure that:

1. 🧰 WSL is enabled and updated on your system.
2. 🌐 You have a working internet connection.

## 📜 License

This project is licensed under the MIT License.

---

🎉 Enjoy using Arch Linux on WSL! 🎉
