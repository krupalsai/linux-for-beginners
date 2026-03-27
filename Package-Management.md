# 📦 Package Management in Linux

## What is a Package Manager?

A package manager automatically installs, updates, and removes software.
Think of it as an **App Store for Linux** — but free!

---

## APT (Ubuntu / Debian)

```bash
sudo apt update                     # Refresh package list
sudo apt upgrade                    # Upgrade all packages
sudo apt install vim                # Install a package
sudo apt remove vim                 # Remove a package
sudo apt autoremove                 # Remove unused packages
apt search firefox                  # Search for a package
apt show vim                        # Show package details
```

---

## DNF / YUM (Fedora / RHEL / CentOS)

```bash
sudo dnf update                     # Update all
sudo dnf install vim                # Install
sudo dnf remove vim                 # Remove
sudo dnf search vim                 # Search
```

---

## Pacman (Arch Linux / Manjaro)

```bash
sudo pacman -Syu                    # Update system
sudo pacman -S vim                  # Install
sudo pacman -R vim                  # Remove
sudo pacman -Ss vim                 # Search
```

---

## Snap (Universal Packages)

```bash
sudo snap install code              # Install VS Code
sudo snap list                      # List installed snaps
sudo snap remove code               # Remove
```

---

## Installing from Source (advanced)

```bash
./configure
make
sudo make install
```

> ⚠️ Prefer your distro's package manager over manual installs when possible.

---
Next → [Resources.md](Resources.md)
