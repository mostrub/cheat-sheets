---
description: web-based SSH access tool
---

# Shell In A Box

This tools allow you to access the server's shell securely through a web browser. Most modern browsers like Chrome, Firefox, Edge, and Safari should support these web-based SSH tools.

#### Setting Up Shell In A Box:

1.  **Install Shell In A Box**:

    {% code overflow="wrap" %}
    ```bash
    sudo apt update
    sudo apt install shellinabox
    ```
    {% endcode %}
2. **Configure Shell In A Box** (if needed):
   * The default configuration should work out of the box, but you can customize it by editing `/etc/default/shellinabox`.
   * For SSL configuration, you can specify your own certificate or let Shell In A Box generate a self-signed certificate.
3.  **Start the Service**:

    {% code overflow="wrap" %}
    ```bash
    sudo systemctl start shellinabox
    ```
    {% endcode %}
4. **Access Shell In A Box**:
   * Open your web browser and navigate to `http://your-server-ip:4200/`.
   * For secure HTTPS access, use `https://your-server-ip:4200/`.

### Security Considerations

* **Use HTTPS**: For both Shell In A Box and Guacamole, it's highly recommended to use HTTPS to secure your connections.
* **Firewall Configuration**: Make sure to configure your firewall to allow traffic on the ports used by these services.
* **Regular Updates**: Keep your server and these applications updated for security and stability.

#### Browser Support

Both Shell In A Box and Apache Guacamole should work on any modern web browser, including:

* Google Chrome
* Mozilla Firefox
* Microsoft Edge
* Apple Safari

These browsers support the web technologies used by Shell In A Box , ensuring compatibility and performance.

### Shell In A Box:

1. **Simplicity**:
   * Shell In A Box is simpler and more straightforward to set up and use. It's primarily focused on providing web-based SSH access.
2. **Resource Usage**:
   * Being a lighter application, it consumes fewer resources on the server.
3. **Functionality**:
   * It's mainly for accessing the shell/command-line interface of the server via a web browser.
4. **Best Suited For**:
   * Users who need quick and easy web-based access to a Unix shell.
5. **Security**:
   * Offers SSL encryption for secure access, though it's less feature-rich in terms of security compared to Guacamole.

#### Apache Guacamole:

1. **Feature-Rich**:
   * Guacamole provides a full remote desktop gateway. It supports VNC, RDP, and SSH protocols, allowing access to graphical desktops as well as terminal sessions.
2. **No Client Software Needed**:
   * Works entirely in the browser without needing any client software or plugins.
3. **Integration Capabilities**:
   * Integrates with LDAP, two-factor authentication, and can use MySQL, PostgreSQL, or SQL Server for database storage.
4. **Resource Usage**:
   * More resource-intensive due to its broader range of features and capabilities.
5. **Best Suited For**:
   * Users who require remote access to graphical desktop environments or need a more comprehensive remote access solution with support for multiple protocols.
6. **Security**:
   * Offers robust security features, including options for two-factor authentication and secure connections over various protocols.

### Reliability and Stability:

* Both are considered stable and reliable for their intended purposes. Shell In A Box is more focused and lightweight, whereas Guacamole offers a wider range of features but at the cost of increased complexity and resource usage.

#### Conclusion:

* If you need a simple, lightweight tool for accessing the shell of your server via a web browser, **Shell In A Box** is more suitable.
* If you require a comprehensive solution that supports multiple protocols (VNC, RDP, SSH) and need access to graphical desktop environments or advanced integration and security features, **Apache Guacamole** is the better choice.
