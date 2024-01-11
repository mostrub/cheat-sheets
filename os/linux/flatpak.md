---
description: >-
  Flatpak is a software utility for application virtualization, and package
  management for Linux desktops.  It provides a sandbox environment where users
  can run applications in isolation.
---

# Flatpak

1.  **Update Your System**:

    ```bash
    sudo apt update
    sudo apt upgrade
    ```
2.  **Install Flatpak**:

    ```bash
    sudo apt install flatpak
    ```
3.  **Add the Flathub Repository**: Flathub is a major repository for Flatpak apps.

    ```bash
    flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
    ```
4. **Restart Your System** (Optional): It's generally a good practice to restart your system after a major installation.

Using Flatpak:

* To install a Flatpak app: `flatpak install flathub [ApplicationID]`
* To run a Flatpak app: `flatpak run [ApplicationID]`
