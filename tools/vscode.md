---
description: >-
  Visual Studio Code (VSCode) is a powerful, open-source code editor known for
  its flexibility and wide range of extensions, supporting various programming
  languages and development tasks.
---

# VSCode

## Visual Studio Code Cheat Sheet

### General Shortcuts

* **Open Command Palette**: `Ctrl+Shift+P` (Win/Linux), `Cmd+Shift+P` (Mac)
* **Quick Open File**: `Ctrl+P` (Win/Linux), `Cmd+P` (Mac)
* **Toggle Terminal**: `Ctrl+`` (Win/Linux),` Cmd+\`\` (Mac)
* **Toggle Sidebar**: `Ctrl+B` (Win/Linux), `Cmd+B` (Mac)
* **Open Settings**: `Ctrl+,` (Win/Linux), `Cmd+,` (Mac)

### Editing

* **Go to Line**: `Ctrl+G` (Win/Linux), `Cmd+G` (Mac)
* **Find**: `Ctrl+F` (Win/Linux), `Cmd+F` (Mac)
* **Replace**: `Ctrl+H` (Win/Linux), `Cmd+Option+F` (Mac)
* **Comment Line**: `Ctrl+/` (Win/Linux), `Cmd+/` (Mac)

### Code Navigation

* **Go to Definition**: `F12` (Win/Linux), `Cmd+Click` (Mac)
* **Open Preview**: `Ctrl+K V` (Win/Linux), `Cmd+K V` (Mac)
* **Toggle Problems**: `Ctrl+Shift+M` (Win/Linux), `Cmd+Shift+M` (Mac)

### Refactoring

* **Rename Symbol**: `F2` (Win/Linux/Mac)
* **Format Document**: `Shift+Alt+F` (Win/Linux), `Shift+Option+F` (Mac)
* **Show Refactoring Options**: `Ctrl+.` (Win/Linux), `Cmd+.` (Mac)

### Debugging

* **Start/Stop Debugging**: `F5` (Win/Linux/Mac)
* **Step Over**: `F10` (Win/Linux/Mac)
* **Step Into**: `F11` (Win/Linux/Mac)
* **Toggle Breakpoint**: `F9` (Win/Linux/Mac)

### Git Integration

* **Open Source Control**: `Ctrl+Shift+G` (Win/Linux), `Cmd+Shift+G` (Mac)
* **Commit Staged Changes**: `Ctrl+Enter` (Win/Linux), `Cmd+Enter` (Mac)
* **View Git History**: `GitLens` extension

### Extensions and Customization

* **Install Extensions**: `Ctrl+Shift+X` (Win/Linux), `Cmd+Shift+X` (Mac)
* **Choose Color Theme**: `Ctrl+K Ctrl+T` (Win/Linux), `Cmd+K Cmd+T` (Mac)

> Note: Keyboard shortcuts might vary based on keyboard layout and custom configurations.

**SSH Connectins from VSCode:**

1. **Install the Remote - SSH Extension** in VSCode on your PC.
2. **Open Command Palette in VSCode**:
   * Press `Ctrl + Shift + P` and type 'Remote-SSH: Connect to Host...'
3. **Enter the Ubuntu Server's IP Address**:
   * Format: `username@ip_address` (replace with your actual username and server's IP).
4. **Follow Prompts**:
   * Authenticate with your password or SSH key.

## VSCode Remote Development Cheat Sheet

### Setting Up Remote Development

* **Install 'Remote Development' Extension Pack**: `Ctrl+Shift+X` (Win/Linux), `Cmd+Shift+X` (Mac)
* **Open Command Palette**: `Ctrl+Shift+P` (Win/Linux), `Cmd+Shift+P` (Mac)
* **Choose Remote Option**:
  * For SSH: `Remote-SSH: Connect to Host...`
  * For Containers: `Remote-Containers: Open Folder in Container...`
  * For WSL: `Remote-WSL: New Window Using Distro...`

### Remote SSH

* **Connect to Host**: Enter `username@hostname` in input prompt
* **SSH Configuration File**: Edit SSH Configurations in `~/.ssh/config`

### Remote Containers

* **Open Folder in Container**: Use `Remote-Containers: Open Folder...`
* **Attach to Running Container**: `Remote-Containers: Attach to Running Container...`

### Working with WSL

* **Open a New WSL Window**: `Remote-WSL: New Window`
* **Open Current Project in WSL**: `Remote-WSL: Reopen Folder in WSL`

### Common Remote Operations

* **Install Extensions Remotely**: Extensions -> Install in SSH/Containers/WSL
* **Port Forwarding for Web Apps**: `Remote-SSH: Forward Port from Active Host`
* **Access Terminal of Remote Host**: Integrated terminal will default to remote shell
* **Edit Remote Config Files**: Directly edit files in the VSCode editor

### Tips for Efficient Remote Work

* **Keep Extensions Updated**: Ensure remote development extensions are up-to-date
* **Use Workspace Files**: To maintain consistent settings across environments
* **Leverage Source Control**: For seamless code sync between local and remote

> Note: Ensure proper network configurations and permissions for remote connections.

## Top 30 VSCode Shortcuts for Windows

### General Editing

1. **Ctrl + X**: Cut line (empty selection).
2. **Ctrl + C**: Copy line (empty selection).
3. **Alt + ↑ / ↓**: Move line up/down.
4. **Shift + Alt + ↓ / ↑**: Copy line up/down.
5. **Ctrl + Shift + K**: Delete line.
6. **Ctrl + Enter**: Insert line below.
7. **Ctrl + Shift + Enter**: Insert line above.
8. **Ctrl + Shift + \\**: Jump to matching bracket.
9. **Ctrl + ] / \[**: Indent/outdent line.
10. **Home / End**: Go to beginning/end of line.

### Navigation & Search

11. **Ctrl + P**: Quick open, go to file.
12. **Ctrl + G**: Go to line.
13. **Ctrl + T**: Show all symbols.
14. **Ctrl + F**: Find.
15. **Ctrl + H**: Replace.
16. **Ctrl + Shift + F**: Find in files.
17. **Ctrl + Shift + H**: Replace in files.

### Code Editing

18. **Ctrl + Space**: Trigger suggestion.
19. **Ctrl + Shift + Space**: Trigger parameter hints.
20. **Ctrl + Shift + I**: Format document.
21. **Ctrl + K**: Ctrl + F\*\*: Format selection.
22. **F12**: Go to definition.
23. **Alt + F12**: Peek definition.
24. **Ctrl + .**: Quick fix.

### Integrated Terminal

25. **Ctrl + \`**: Show integrated terminal.
26. **Ctrl + Shift + \`**: Create new terminal.
27. **Ctrl + Shift + 5**: Split terminal.

### Remote Development

28. **F1**, type "Remote-SSH": Connect to SSH Host...
29. **F1**, type "Remote-Containers": Reopen in Container.
30. **F1**, type "Remote-WSL": Reopen Folder in WSL.

> Note: These shortcuts can greatly enhance your productivity in VSCode on Windows.
