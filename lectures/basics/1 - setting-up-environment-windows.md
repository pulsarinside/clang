# Setting Up C Development Environment on Windows

## Prerequisites

Before setting up a C development environment on Windows, ensure you have the following prerequisites:

1. **Windows Operating System:** You should be running a Windows-based operating system (Windows 7, 8, 10, or later).

2. **Internet Connection:** A stable internet connection is required for downloading necessary tools.

## Steps

### 1. Install Windows Subsystem for Linux (WSL)

To make C development on Windows more convenient, you can set up the Windows Subsystem for Linux (WSL) and use it to install GCC and other development tools.

1. Open PowerShell as an administrator by searching for "PowerShell" in the Windows Start menu, right-clicking it, and selecting "Run as administrator."

2. Run the following command to enable the WSL feature:

   ```powershell
   dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart

Restart your computer when prompted.

Install WSL 2 by running the following command:

```powershell
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```
Download and install the WSL 2 Linux Kernel update package from [Microsoft's WSL 2 Kernel](https://aka.ms/wsl2kernel) page.

### Set WSL 2 as the default version by running this command:

```powershell
wsl --set-default-version 2
```
Install a Linux distribution from the Microsoft Store, such as Ubuntu, Debian, or CentOS. Launch the installed distribution and complete the initial setup (username/password).

### Install GCC in WSL
Open your installed Linux distribution (e.g., Ubuntu) from the Start menu or use the wsl command in PowerShell.

Update the package list and install GCC by running the following commands:

```bash
sudo apt update
sudo apt install gcc
```
Verify the installation by checking the GCC version:

```bash
gcc --version
```

### Setting Up a Text Editor or Integrated Development Environment (IDE)

Choose a text editor or IDE for writing and editing your C code. Some popular options include Visual Studio Code (VSCode) with C/C++ extensions, Code::Blocks, or Sublime Text. Install your preferred editor/IDE and configure it according to your preferences.

### Writing and Compiling C Programs

You are now ready to write and compile C programs using your preferred text editor or IDE. Create a C source code file (e.g., my_program.c) and use the following command in your WSL terminal to compile it:

```bash
gcc -o my_program my_program.c
```
Replace my_program with your desired output executable name and my_program.c with the name of your C source file.

### Running C Programs
After successful compilation, you can run your C program from the WSL terminal:

```bash
./my_program
```
Congratulations! You have successfully set up a C development environment on Windows using WSL and GCC. You can now start writing, compiling, and running C programs on your Windows machine.