# Pre-class Setup: Installing Visual Studio Code

Before we begin our class, it is essential that you set up **Visual Studio Code (VS Code)** on your computer. VS Code is a lightweight but powerful source code editor available for both Windows and macOS, and it will be our primary tool for coding during this course.

Follow the instructions below to install VS Code and get your system ready for our class.

---

## Step 1: Install Visual Studio Code

### For Windows Users:
1. Open your web browser and navigate to the [Visual Studio Code Download Page](https://code.visualstudio.com/).
2. Click on the **Windows** download button.
3. Once the installer (`VSCodeSetup.exe`) has been downloaded, open it to start the installation process.
4. During installation, make sure to:
   - Check the option to **Add to PATH** (this allows you to run VS Code from the command line).
   - Optionally, check the **Install code command in PATH** option if you want to run the `code` command from a terminal.
5. Follow the prompts and finish the installation process.
6. Once installed, open **Visual Studio Code** from the Start Menu or by searching for "VS Code."

### For macOS Users:
1. Open your web browser and go to the [Visual Studio Code Download Page](https://code.visualstudio.com/).
2. Click on the **macOS** download button to get the `.dmg` installer.
3. After the download is complete, open the `.dmg` file and drag the **Visual Studio Code** application to your **Applications** folder.
4. To add VS Code to your system path so you can use it from the terminal:
   - Open VS Code.
   - Press **Cmd + Shift + P** to open the **Command Palette**.
   - Type and select **Shell Command: Install 'code' command in PATH**.
5. After this, you can open VS Code from the terminal by typing `code` followed by a directory or file.

---

## Step 2: Install Git (Required for Version Control)

We will use **Git** to manage and track changes in our projects. Install Git on your computer by following these steps:

### For Windows Users:
1. Download Git from [https://git-scm.com/download/win](https://git-scm.com/download/win).
2. Open the installer and follow the on-screen instructions.
3. Make sure to check the option **"Use Git from Git Bash only"** during installation if you only want to use Git with VS Code.
4. Once installed, open **Git Bash** to confirm Git is working by running:
   ```bash
   git --version
5. Ensure that Git is also integrated into VS Code by opening VS Code and going to the Source Control tab (located on the left sidebar).
### For macOS Users:
Git should already be installed by default on macOS. To confirm, open Terminal and run:
```
git --version
```
If Git is not installed, macOS will prompt you to install the Xcode Command Line Tools. Follow the prompts to install Git.
You can also download Git from https://git-scm.com/download/mac.

## Step 3: Install Extensions in VS Code
For Both Windows and macOS Users:
Once VS Code is installed, we will need to install several extensions that will make our coding environment more efficient:

Open VS Code.
Click on the Extensions icon in the sidebar (or press Ctrl + Shift + X on Windows or Cmd + Shift + X on macOS).
Search for the following extensions and click Install for each:
<br>Remote - SSH (to connect to remote servers using SSH).
<br>Python (if we are using Python in this course).
<br>GitLens (helps with Git version control).

## Step 4: Setting Up the Terminal in VS Code

### For Windows Users:
If you prefer using **Git Bash** within **VS Code** as your terminal, follow these steps:

1. Open **VS Code**.
2. Go to **File** > **Preferences** > **Settings**.
3. In the settings search bar, type **"Terminal"** and look for **Integrated > Default Profile**.
4. Set the default terminal profile to **Git Bash**.

### For macOS Users:
The default terminal in macOS is the **Bash** shell or **Zsh**, which can be used directly. However, if needed, you can still follow the same steps as above to adjust terminal settings.

---

## Step 5: Verify Your Setup

Once you’ve installed **VS Code** and **Git**, follow these steps to verify that everything is working correctly:

1. Open **VS Code**.
2. Press `Ctrl + \`` (backtick) on Windows or `Cmd + \`` (backtick) on macOS to open the integrated terminal.
3. Run the following commands to verify your installation:

   - **To check Git**:
     ```bash
     git --version
     ```

   - **To check if the `code` command is available**:
     ```bash
     code --version
     ```

If everything is set up correctly, you're ready to go for our class!

---

## Support

If you run into any issues while installing or setting up **VS Code**, feel free to reach out to the instructor for help or refer to the official [VS Code Documentation](https://code.visualstudio.com/docs).

---

# Cloning the Repository into VS Code

Before starting with the exercises, you need to clone the repository that contains the teaching material for this module.

## Steps to Clone the Repository:

1. **Open VS Code**.
2. **Open the Command Palette**:
   - Press `Ctrl + Shift + P` (Windows) or `Cmd + Shift + P` (macOS).
3. **Search for `Git: Clone`** and select it.
4. **Enter the repository URL**:
   - You will be prompted to enter the **GitHub repository URL**. Use the URL that the instructor provided (example below):
     ```bash
     https://github.com/apinya-j/HPC-Login-Practice-AMS-KKU.git
     ```
5. **Choose a folder** on your local machine where you want to clone the repository.
6. After the clone is complete, **open the cloned folder** in VS Code when prompted.

Now you are ready to proceed with the exercises in **Module 1**.


