# 🛠️ Developer Tool Setup Guide

This guide covers installation of essential development tools for **Windows** and **macOS**.

---

## 🪟 Windows Tools Installation (Using Chocolatey)

👉 First, install Chocolatey from the official guide:  
[https://chocolatey.org/docs/installation](https://chocolatey.org/docs/installation)

Then, run these commands in **Command Prompt (Admin)** or **PowerShell (Admin)**:

```bash
choco install virtualbox --version=7.1.4 -y
choco install vagrant --version=2.4.3 -y
choco install git -y
choco install corretto17jdk -y
choco install maven -y
choco install awscli -y
choco install intellijidea-community -y
choco install vscode -y
choco install sublimetext3 -y
```

---

## 🍎 macOS Tools Installation (Using Homebrew)

👉 First, install Homebrew from the official guide:  
[https://brew.sh/](https://brew.sh/)

---

### 📝 Add Curl Config (Important Step)

Create a `.curlrc` file in your home directory with the following content:

```bash
echo -k > ~/.curlrc
cat ~/.curlrc  # Verify the content
```

---

### 🔧 Install Tools via Terminal

> ⚠️ Note: `virtualbox` does **not** work on M1/M2 Macs. Skip it if using Apple Silicon.

```bash
brew install --cask virtualbox 
brew install --cask vagrant
brew install --cask vagrant-manager
brew install git
brew install openjdk@17
sudo ln -sfn $(brew --prefix)/opt/openjdk@17/libexec/openjdk.jdk /Library/Java/JavaVirtualMachines/openjdk.jdk
exec zsh -l
brew install maven
brew install --cask visual-studio-code
brew install --cask intellij-idea
brew install --cask intellij-idea-ce
brew install --cask sublime-text
brew install awscli
```

---

## ✅ Done!

You are now ready to start developing on your fully configured environment 🚀
