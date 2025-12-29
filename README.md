Linux Workstation Setup
===
Ansible playbook that installs and configures software I use on my linux workstations (Fedora and Debian). 

> ⚠️ STILL WORK IN PROGRESS

Requirements
---
- Sudo access
- Python 3 installed
- Ansible installed

Installation
---
- Clone this repository with `git clone https://github.com/myckakamil/linux-workstation-playbook` and navigate to the repository directory `cd linux-workstation-playbook`
- Run playbook with `ansible-playbook main.yml --ask-become-pass` and enter sudo password

Included apps and tools
---
**Packages**:
- docker
- minikube
- vscodium
- neovim
- tmux
- ncdu
- python3-psutil
- tealdeer
- flatpak
- gnome-extensions-app
- steam
- fastfetch
- gnome-shell-extension-appindicator.noarch
- xdg-desktop-portal
- trash-cli

**Flatpaks**:
- Thunderbird
- Obsidian
- Spotify
- Slack
- Discord
- Bitwarden
- WinBox
- Flameshot

Removed packages
---
I don't like having duplicate apps or apps I don't use, so I decided to uninstall some packages that come preinstalled by default.
- Fedora Media Writer
- GNOME Tour
- GNOME System Monitor
- GNOME extensions installed from distribution package
    - Apps menu
    - Background logo
    - Launch new instance
    - Places menu
    - Window list
    - 'common' extensions
- GNOME Contacts
- GNOME Classic Session
- Showtime

Roadmap
---
- [ ] - Add Debian support (I haven't needed to reinstall my laptop with Debian for over 2 years, so I haven't found a reason to do this yet)
- [ ] - More in-depth configuration of VSCodium and Neovim
- [x] - Shortcuts configuration
- [x] - Installing and enabling GNOME extensions
- [ ] - System hardening
- [ ] - Set up Windows VM
- [ ] - Sync with my Nextcloud instance