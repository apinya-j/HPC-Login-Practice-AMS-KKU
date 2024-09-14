# Practical Skills in Using Server and HPC

## Overview
In this practical guide, you will learn how to log in to an HPC server using various methods, including:
- SSH (for macOS/Linux)
- PuTTY or X2Go (for Windows)
- Visual Studio Code (VS Code) with the Remote-SSH extension

By the end of this guide, you should be able to securely connect to an HPC server and begin running bioinformatics tasks.

### Step 1: Access via SSH from macOS/Linux
1. Open the **Terminal**.
2. Run the following command to log in:
```
ssh <username>@<HPC-server-address>
```
Note: Replace <username> with your actual username and <HPC-server-address> with the server address provided.  
3. You will be prompted for your password. Enter it to complete the login.  
4. Verify Login:
To confirm you have successfully logged in, type:
```
whoami
```
You should see your username as output.

### Step 2: SSH Access with SSH Key
In case of, username and password provided to you by the admin to access the HPC server.
Instructions:
1. Ensure that you have the following details provided by your admin:
Username: Your unique user identifier (e.g., student123).
Password: The password that was assigned to you by the admin.
HPC Server Address: The server’s domain name or IP address (e.g., hpc.example.com).

2. Log in to the HPC server using SSH:
Open Terminal (macOS/Linux) or Git Bash (Windows) on your system.
Run the following command, replacing <username> with the username provided by the admin and <HPC-server-address> with the server's address:
   ```
   ssh <username>@<HPC-server-address>
   ```

3. Enter your password
When prompted, input the password provided by the admin. Please note that the password will not appear as you type for security reasons.

4. Run the following command to verify your connection:
   ```
   whoami
   ```
The output should show your username.

### Step 3: SSH Access from Windows Using PuTTY or X2Go  
PuTTY or X2Go is a free SSH client for Windows users.  
Instructions:
1. Download and install PuTTY from PuTTY official website [here](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html).
   or X2Go [here](https://wiki.x2go.org/doku.php/download:start)
3. Open PuTTY or X2Go. In the Host Name field, enter the HPC server address: Make sure the Connection Type is set to SSH.
   ![How to set up new session of X2Go](https://github.com/user-attachments/assets/89b12150-259a-43fe-b68d-3b2eef2805ef)

5. Click Open. You will be prompted to enter your username and password.

### Step 4: Use Visual Studio Code with SSH Extension
Visual Studio Code offers an integrated environment to connect to remote servers using the Remote-SSH extension.
Instructions:
1. Install VS Code from [here](https://code.visualstudio.com/download)
2. Open VS Code and go to the Extensions tab on the left sidebar.
3. Search for Remote - SSH and click Install.

4. After installing the extension, press Ctrl + Shift + P (or Cmd + Shift + P on macOS) and type:
  ```bash
Remote-SSH: Connect to Host
```
![image](https://github.com/user-attachments/assets/407b0986-ed77-4453-b3a5-fea726fd40e7)

5. Enter your SSH command in the prompt:
  ```bash
ssh <username>@<HPC-server-address>
```
6. You will be prompted for your password or SSH key. After connecting, you can open folders, run terminal commands, and work directly on the HPC server through VS Code

### Troubleshooting
If you encounter issues while logging in:
<br>Double-check your username and HPC server address.
<br>Ensure that your firewall is not blocking SSH access.
<br>Make sure you have installed the correct tools (e.g., PuTTY, Git for Windows, or SSH keys).
<br>Contact the system administrator if you cannot log in after following the instructions.

