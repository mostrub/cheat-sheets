---
description: >-
  Remote Desktop Protocol. xRDP allows non-Windows systems to serve a graphical
  interface
---

# RDP with xRDP and XFCE

### xRDP and XFCE&#x20;

provides a solution to remotely access the graphical user interface of a Linux system from other operating systems like Windows. xRDP is an open-source implementation of the RDP server, which allows non-Microsoft operating systems, like Linux, to provide a fully functional remote desktop experience. XFCE is a lightweight and stable desktop environment for Unix-like operating systems, known for its speed and low resource usage. This combination is particularly beneficial for users who need a fast and efficient graphical interface over a remote

1.  **Install xRDP**:

    ```bash
    sudo apt install xrdp
    ```
2.  **Install XFCE** (for a lightweight GUI):

    ```bash
    sudo apt install xfce4 xfce4-goodies
    ```
3.  **Configure xRDP to Use XFCE**:

    ```bash
    echo xfce4-session >~/.xsession
    sudo systemctl restart xrdp
    ```
4.  **Open RDP Port in Firewall**:

    ```bash
    sudo ufw allow 3389/tcp
    ```
