# Module 2: Introduction to Linux and Basic HPC Commands (Using Local Computer with VS Code)

## Objective
In this module, students will practice basic **Linux commands** for file management and navigation on their local computer using **VS Code**. We will also simulate some **High-Performance Computing (HPC)** concepts through VS Code’s integrated terminal. Before starting, you will need to clone the repository that contains all the required files and instructions for this module.

---

## 1. Cloning the Repository into VS Code

Before starting with the exercises, you need to clone the repository that contains the teaching material for this module.

### Steps to Clone the Repository:

1. **Open VS Code**.
2. **Open the Command Palette**:
   - Press `Ctrl + Shift + P` (Windows) or `Cmd + Shift + P` (macOS).
3. **Search for `Git: Clone`** and select it.
4. **Enter the repository URL**:
   - You will be prompted to enter the **GitHub repository URL**. Use the URL that the instructor provided (example below):
     ```bash
     https://github.com/yourusername/linux-hpc-training.git
     ```
5. **Choose a folder** on your local machine where you want to clone the repository.
6. After the clone is complete, **open the cloned folder** in VS Code when prompted.

Now you are ready to proceed with the exercises in **Module 2**.

---

## 2. Basic Linux Commands in VS Code

You will be using **VS Code’s integrated terminal** to practice these commands on your **local computer**.

### a. File and Directory Management

1. **Open the integrated terminal in VS Code**: SKIP THIS step
   - Press `Ctrl + \`` (backtick) on Windows or `Cmd + \`` on macOS.

2. **Check your current directory**:
   - Use the `pwd` command to print the current working directory:
     ```bash
     pwd
     ```
   - The output should show the path where the repository is cloned.

3. **List files and directories**:
   - Use the `ls` command to list the files and directories in your current location:
     ```bash
     ls -l
     ```
   - You should see the files that were cloned from the repository.

4. **Create a new directory**:
   - Use `mkdir` to create a new directory called `practice` inside your cloned repository:
     ```bash
     mkdir practice
     ```

5. **Navigate into the new directory**:
   - Use `cd` to change directories into the `practice` folder:
     ```bash
     cd practice
     ```

6. **Create a new file**:
   - Use the `touch` command to create an empty file called `myfile.txt`:
     ```bash
     touch myfile.txt
     ```

7. **Edit a file**:
   - Open the newly created `myfile.txt` directly in VS Code:
     ```bash
     code myfile.txt
     ```
   - Add some text to the file and save it.

8. **Move or rename a file**:
   - Use the `mv` command to move or rename `myfile.txt`:
     ```bash
     mv myfile.txt mynewfile.txt
     ```

9. **Delete a file**:
   - Use the `rm` command to remove the file:
     ```bash
     rm mynewfile.txt
     ```
10. **Copy a file from your local machine to the server**
Transfer files using SCP (Secure Copy Protocol), a command that allows them to securely move files between their local machine and the server.
```bash
     scp -i /path/to/your-key.pem /local/path/to/file <username>@<server-IP>:/home/<username>/practice/
```
11. After copying the file, verify its existence on the server or your local machine using the ls command:

12. Check disk space usage:
```bash
     df -h
```
13. Check running processes:
```bash
     top
```
---

## 3. Simulating Basic HPC Commands (Locally) >SKIP This Step<

Although you are working on your local computer, we can simulate some HPC-related commands and workflows.

### a. Simulating Job Scheduling (SLURM)

Since you are not on an actual HPC cluster, the following commands will simulate the **SLURM** commands used in real HPC environments:

1. **View available resources** (simulating the `sinfo` command):
   ```bash
   echo "Available nodes: 2, CPUs: 64, GPUs: 8"
   ```
2. Simulate submitting a job:
Use the `sbatch` command to simulate submitting a job. This command creates a simple shell script and "submits" it:
```bash
echo -e "#!/bin/bash\n\necho Hello, HPC!" > myjobscript.sh
sbatch myjobscript.sh
```
3. Check the status of the job (simulating `squeue`):

Use the following command to simulate checking the status of your job:
bash
```bash
echo "Checking job status... Job ID: 101, Status: Running"
```

4. Cancel a job (simulating scancel):

You can simulate cancelling a job using the following command:
```bash
echo "Job 101 has been cancelled"
```
# Practical Exercises

## Exercise 1: File Management

1. Log into the server (simulated in your local machine using VS Code).
2. Create a directory called `linux_practice`:
   ```bash
   mkdir linux_practice
   ```
3. Inside the `linux_practice` directory, create a text file called exercise.txt:
```bash   
touch exercise.txt
```
4. Add your full name to `exercise.txt`
```
echo "My name is [Your Name] and my favorite programming language is [Language]" > exercise.txt
```
5. Copy the file to another location, rename it to `backup.txt`, and delete the original:
```
cp exercise.txt backup.txt
rm exercise.txt
```
6. List all files in the directory to verify your work:
```
ls -l
```
# Exercise 2: Basic HPC Simulation
Task 1: File Transfer and Management:
1. Transfer a text file from your local machine to the server using SCP.
2. On the server, create a directory structure:
```
   project/
    data/
    scripts/
    results/
```
3. Move the transferred file: "file to be transered" to the data/ folder and rename it to dataset1.txt.


## Submission Instructions:
Complete the exercises and write your answers to the quiz in a file called `quiz_answers.<your full name>.txt`.
Submit your quiz_answers.txt file via the [Onedrive)](https://khonkaenuniversity-my.sharepoint.com/:f:/g/personal/apinjus_kku_ac_th/EqZaaIfr-8JCi7_Mf0xi5bAB0VDQUl10ycl8tny3KxJfdg?e=iXFeyU).

## Support
If you run into any issues during this module, feel free to reach out to the instructor or teaching assistant for help. You can also refer to the official Linux or HPC documentation for further assistance.

Thank you for setting up your environment ahead of time!
