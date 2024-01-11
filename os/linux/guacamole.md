---
description: web-based SSH access tool
---

# Guacamole

These tools allow you to access the server's shell securely through a web browser. Most modern browsers like Chrome, Firefox, Edge, and Safari should support these web-based SSH tools.

#### Setting Up Apache Guacamole:

Apache Guacamole is a bit more complex to set up as it's a full remote desktop gateway. It requires a Tomcat server and a MySQL or PostgreSQL database.

1.  **Install Dependencies**:

    ```bash
    sudo apt update
    sudo apt install tomcat9 tomcat9-admin tomcat9-user
    sudo apt install guacd libguac-client-ssh0 libguac-client-vnc0 libguac-client-rdp0 guacamole
    sudo apt install libguac-client-vnc0 guacamole-tomcat
    ```
2. **Configure Guacamole**:
   * Edit the Guacamole configuration file (`/etc/guacamole/guacamole.properties`) to set up database connections and other settings.
3. **Deploy Guacamole Client**:
   * Deploy the Guacamole client to the Tomcat server.
4. **Start Services**:
   * Start or restart the Tomcat and Guacamole services.
5. **Access Guacamole Web Interface**:
   * Open your browser and navigate to `http://your-server-ip:8080/guacamole/`.
   * Log in using the credentials you set up during the configuration.

#### Security Considerations

* **Use HTTPS**: For both Shell In A Box and Guacamole, it's highly recommended to use HTTPS to secure your connections.
* **Firewall Configuration**: Make sure to configure your firewall to allow traffic on the ports used by these services.
* **Regular Updates**: Keep your server and these applications updated for security and stability.

#### Browser Support

Both Shell In A Box and Apache Guacamole should work on any modern web browser, including:

* Google Chrome
* Mozilla Firefox
* Microsoft Edge
* Apple Safari

These browsers support the web technologies used by Guacamole, ensuring compatibility and performance.

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
