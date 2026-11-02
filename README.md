# Debian Machine Setup

### Automated Debian Linux Environment Configuration

A collection of Bash scripts and shell configuration files designed to simplify setting up a fresh Debian-based Linux system.

This project automates the installation of my preferred development tools, command-line utilities, and desktop applications while documenting my personal Zsh environment.

## Overview

Configuring a new Linux installation can involve repetitive package installation, system updates, and shell customization.

This repository brings those tasks together through a Bash installation script and a reusable Zsh configuration.

It reflects my interest in Linux system administration, automation, and creating efficient development environments.

## Features

- **System Updates:** Refreshes package lists and upgrades installed packages using APT.
- **Automated Software Installation:** Installs a curated collection of development, productivity, and multimedia applications.
- **Zsh Setup:** Attempts to configure Zsh as the default shell.
- **Oh My Zsh Integration:** Installs the Oh My Zsh framework.
- **Shell Enhancements:** Downloads syntax highlighting and autosuggestion plugins.
- **Personal Configuration:** Includes a `.zshrc` file with my preferred theme, plugins, and terminal greeting.
- **Privilege Checking:** Verifies that the installation script is executed with root privileges.

## Included Software

| Category | Applications |
|---|---|
| Development | Git, Emacs, Python 3, pip, Kate |
| Terminal & Shell | Zsh, Oh My Zsh, Terminator, fzf |
| System Monitoring | htop, Neofetch |
| Networking | SSH, curl, wget |
| File Management | Krusader, Midnight Commander |
| Web Browsing | w3m |
| Multimedia | VLC |
| Compatibility & Gaming | Wine, Lutris, PlayOnLinux |
| Terminal Utilities | cowsay |

## Repository Structure

**`install_apps.sh`**

The main Bash script responsible for system updates, package installation, and initial shell configuration.

**`.zshrc`**

My personal Zsh configuration, including the Robbyrussell theme, plugin settings, and a customized terminal greeting.

**`LICENSE`**

GNU General Public License version 3.

## Installation

Clone the repository:

```bash
git clone https://github.com/michaelsamhume/Debian-Machine-Setup.git
cd Debian-Machine-Setup
```

Review the installation script:

```bash
cat install_apps.sh
```

The script is designed to run with root privileges:

```bash
sudo bash install_apps.sh
```

**Important:** This is a personal configuration script, not a universally tested installer. It performs system-wide changes and downloads an external shell installation script. Review its commands before execution.

Package availability may vary by Debian release and configured repositories. The current script also requires improvements to ensure Zsh and Oh My Zsh are configured for the intended non-root user.

### Zsh Configuration

The repository includes my personal `.zshrc` configuration as a reference.

It uses the Robbyrussell theme and includes settings for syntax highlighting, autosuggestions, and a custom terminal greeting.

The configuration may need adjustments to plugin paths and dependencies before use on another system.

## Technologies

- Bash scripting
- Debian Linux
- APT package management
- Zsh
- Oh My Zsh
- Git
- Linux command-line utilities

## What I Learned

This project gave me practical experience with:

- Automating repetitive system administration tasks
- Linux package management
- Bash scripting and shell environments
- Configuring developer tools
- Managing system privileges
- Customizing and maintaining Linux installations

It also reinforced the value of reproducible development environments and reducing manual configuration.

## Future Improvements

Potential improvements include:

- More reliable configuration of the non-root user's shell
- Better error handling and package availability checks
- Idempotent installation procedures
- Automatic backup of existing shell configurations
- Optional software installation categories
- Support for additional Debian-based distributions

## Related Project

[Fedora Machine Setup](https://github.com/michaelsamhume/Fedora-Machine-Setup) — A similar automation project using Fedora's DNF package manager.

## License

Licensed under the GNU General Public License v3.0. See `LICENSE` for details.

## Author

**Michael Hume**

Computer Science | Software Engineering | Linux | Systems Programming

[GitHub Profile](https://github.com/michaelsamhume)
