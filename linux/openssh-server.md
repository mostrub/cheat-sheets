---
description: SSH Server to access a Unix/Linux based systems
---

# OpenSSH Server

1.  **Install OpenSSH Server**:

    ```bash
    sudo apt update
    sudo apt install openssh-server
    ```
2.  **Enable SSH Service**:

    ```bash
    sudo systemctl status ssh
    ```
3.  **Configure Firewall**:

    ```bash
    sudo ufw allow ssh
    ```

