---
description: >-
  Nala is a front-end for libapt-pkg, aiming to provide a more user-friendly
  interface and faster package fetching with parallel downloading.
---

# Nala

1.  **Add Nala's Repository**:

    ```bash
    echo 'deb http://deb.nala.cat/ any main' | sudo tee /etc/apt/sources.list.d/nala.list
    ```
2.  **Add the Repository Key**:

    ```bash
    curl -sS 'https://deb.nala.cat/pubkey.gpg' | sudo gpg --dearmor | sudo tee /usr/share/keyrings/nala-archive-keyring.gpg
    ```
3.  **Update Your Package List**:

    ```bash
    sudo apt update
    ```
4.  **Install Nala**:

    ```bash
    sudo apt install nala
    ```

Using Nala:&#x20;

* To install a package: `nala install [package]`
* To remove a package: `nala remove [package]`
* For more commands: `nala --help`

