# Cybsec-Notes-Course-4

# Module 2

# 🐧 Common Linux Distributions in Cybersecurity

## 🔐 Kali Linux™

**Kali Linux™** is a **Debian-based**, open-source Linux distribution specifically designed for cybersecurity professionals.

### 🛠️ Key Features
- Pre-installed tools for:
  - **Penetration testing**
  - **Digital forensics**
- Frequently used in ethical hacking labs and red team operations
- CLI-focused but includes a GUI
- Popular in training and certification environments (e.g., OSCP)

> Penetration testing simulates attacks to identify vulnerabilities.  
> Digital forensics investigates and analyzes digital evidence after incidents.

---

## 🧑‍💻 Ubuntu

**Ubuntu** is one of the most **user-friendly** and widely adopted Linux distributions, including in the security industry.

### 🔍 Key Features
- Debian-derived
- Includes both a **CLI** and **GUI**
- Supports **common and security-focused packages** via APT
- Large community and extensive support documentation
- Frequently used in **cloud computing environments**

> Ubuntu is ideal for newcomers and widely used in enterprise cloud systems.

---

## 🦜 Parrot OS

**Parrot OS** is another **Debian-based** distribution tailored for cybersecurity tasks.

### 🔐 Key Features
- Includes tools for:
  - **Penetration testing**
  - **Digital forensics**
- User-friendly with a clean **GUI** and robust **CLI**
- Lighter footprint than Kali in some configurations

> Great for security professionals who want preloaded tools with a GUI-centric workflow.

---

## 🏢 Red Hat® Enterprise Linux® (RHEL)

**RHEL** is a **subscription-based**, **enterprise-grade** Linux distribution.

### 🧾 Key Features
- Designed for **business and enterprise environments**
- Offers **official support**, patches, and security updates
- Not free; geared toward organizations requiring stability and support
- Often found in corporate data centers

> Used in mission-critical applications and enterprise IT environments.

---

## 🌐 AlmaLinux

**AlmaLinux** is a **community-driven replacement** for CentOS, designed for stability and compatibility.

### 🔁 Key Features
- Binary-compatible with **RHEL**
- Fully open-source and free
- Intended as a drop-in replacement for **CentOS 8**
- Maintains support for legacy infrastructure and enterprise applications

> Ideal for organizations migrating from CentOS after its end-of-life.

---

## ✅ Key Takeaways

- **Kali Linux™, Ubuntu, Parrot, Red Hat, and AlmaLinux** are widely used in cybersecurity.
- Security analysts should be familiar with these distributions as they may encounter them in real-world environments.
- Some are designed for **penetration testing** (e.g., Kali, Parrot), others for **enterprise or server use** (e.g., Red Hat, AlmaLinux), and some serve as general-purpose distributions (e.g., Ubuntu).

# 📦 Introduction to Package Managers (Linux)

## 🧱 What is a Package?

A **package** is a collection of files and metadata required to install and run a piece of software. Some packages form complete applications, while others are dependencies (support files used by other packages).

> Example: A text editor might require several libraries (dependencies) for its GUI or text rendering.

---

## 🛠️ What is a Package Manager?

A **package manager** is a tool that:
- Installs, updates, removes, and manages packages
- Resolves and installs **dependencies**
- Helps keep systems secure by updating packages with **security patches and bug fixes**

> Always aim to use the latest package versions to maintain security and stability.

---

## 📁 Package File Formats

| Package Type     | Used By                    | File Extension     |
|------------------|----------------------------|--------------------|
| `.deb` (Debian)  | Debian, Ubuntu, Kali, Parrot | `package_version.deb` |
| `.rpm` (Red Hat) | Red Hat, CentOS, AlmaLinux | `package-version.rpm` |

---

## 🔧 Package Managers by Distribution

### 🐧 Debian-based (e.g., Ubuntu, Kali, Parrot)
- **Package Manager**: `dpkg`
- **Package Management Tool**: `APT` (Advanced Package Tool)
  - CLI command examples:
    ```bash
    sudo apt update           # Update package list
    sudo apt install nmap     # Install a package
    sudo apt remove nmap      # Remove a package
    ```

### 🏢 Red Hat-based (e.g., Red Hat, CentOS, AlmaLinux)
- **Package Manager**: `RPM`
- **Package Management Tool**: `YUM` (Yellowdog Updater, Modified)
  - CLI command examples:
    ```bash
    sudo yum update           # Update packages
    sudo yum install nmap     # Install a package
    sudo yum remove nmap      # Remove a package
    ```

---

## 🧠 Key Takeaways

- A **package** is software bundled for easy installation and use.
- **Package managers** and **management tools** simplify working with packages and their dependencies.
- **Debian-based** distros use `.deb` packages (`dpkg`, `apt`).
- **Red Hat-based** distros use `.rpm` packages (`rpm`, `yum`).
- Keeping packages updated is critical for system **security and performance**.

# 🧪 Qwiklabs: Resources for Completing Linux Labs

## 📌 Important Notice
> **Qwiklabs Age Requirement:**  
> Due to updated terms of service, Qwiklabs now requires users to be **18+**.  
> Learners under 18 can still complete the certificate by:
> - Reviewing Qwiklabs **instructions and exemplars**
> - Participating in **alternative hands-on activities**
> - Completing **graded assessments**

---

## 🧭 How to Use Qwiklabs

### 🔓 Launching a Lab
1. Navigate to a Coursera lab activity.
2. Click **Launch App** — a new tab with Qwiklabs instructions opens.
3. Click **Start Lab** to open a temporary terminal.
4. Instructions will appear on the right side of the screen.

> ⚠️ It may take a moment for the terminal to start.

### 🧰 Lab Control Dialog Box
- **Start Lab**: Begins the lab and timer.
- **End Lab**: Ends the lab and deletes resources.
- **Timer**: Shows how much time remains (e.g., 20 minutes).
- **Open Linux Console**: Opens terminal in a new browser window.

### 🔍 Checking Your Progress
Click the **Check my progress** button at the end of each task to:
- Get task completion feedback
- View helpful hints if the task is incomplete

---

## 🖱️ Navigation Tips & Shortcuts

### 📋 Copy/Paste in Terminal
- **Copy (CTRL + C)**: Works in instructions section.
- **Paste (CTRL + V)**: Works in the terminal after clicking inside it.
- **Allow clipboard access** when prompted by your browser for full functionality.

### 🧾 Code Blocks
- Click the **copy icon** (`📄`) in a code block to copy text.
- Paste into the terminal using **CTRL + V** once the terminal is active (flashing cursor block).

### 🧼 Clearing the Terminal
- Run `clear` or press **CTRL + L**.

---

## 🧭 Helpful Keyboard Shortcuts

| Shortcut       | Description                                          |
|----------------|------------------------------------------------------|
| `CTRL + C`     | Terminates current command in terminal               |
| `CTRL + V`     | Pastes text into terminal                            |
| `CTRL + A`     | Moves cursor to start of the line                    |
| `CTRL + E`     | Moves cursor to end of the line                      |
| `CTRL + L`     | Clears the terminal screen                           |
| `↑` / `↓`      | Scroll through command history                       |
| `←` / `→`      | Move left or right within a command                  |
| `Tab`          | Auto-completes commands or filenames                 |

---

## ✅ Finishing Your Lab

- When you're done: **Click `End Lab`**
- **Don’t end early**: Ending a lab deletes your progress and terminal access.

### 📈 Coursera Progress Tracking
If your lab completion isn’t showing:
- Refresh the Coursera page after finishing the lab
- Look for a ✅ green check mark

---

## 🧠 Key Takeaways
- Qwiklabs lets you **practice Linux commands interactively**
- Navigating Qwiklabs efficiently will help you get the most out of your labs
- Use **keyboard shortcuts** to work faster and smarter in the terminal

ctivity overview
In this lab activity, you used the Advanced Package Tool (APT) and sudo to install and uninstall applications in a Linux Bash shell.

While installing Linux applications can be a complex task, the APT package manager manages most of this complexity for you and allows you to quickly and reliably manage the applications in a Linux environment.

You used Suricata and tcpdump as an example. These are network security applications that can be used to capture and analyze network traffic.

The virtual machine you accessed in this lab has a Debian-based distribution of Linux running, and that works with the APT package manager. Using a virtual machine prevents damage to a system in the event its tools are used improperly. It also gives you the ability to revert to a previous state.

As a security analyst, it's likely you'll need to know how to install and manage applications on a Linux operating system. In this lab activity, you’ll learn how to do exactly that!

This exemplar is a walkthrough of the previous Qwiklab activity, including detailed instructions and solutions. You may use this exemplar if you were unable to complete the lab and/or you need extra guidance in competing lab tasks. You may also refer to this exemplar to prepare for the graded quiz in this module.

Scenario
Your role as a security analyst requires that you have the Suricata and tcpdump network security applications installed on your system.

In this scenario, you have to install, uninstall, and reinstall these applications on your Linux Bash shell. You also need to confirm that you’ve installed them correctly.

Here’s how you'll do this: First, you’ll confirm that APT is installed on your Linux Bash shell. Next, you’ll use APT to install the Suricata application and confirm that it is installed. Then, you’ll uninstall the Suricata application and confirm this as well. Next, you’ll install the tcpdump application and list the applications currently installed. Finally, you’ll reinstall the Suricata application and confirm that both applications are installed.

OK, it's time to learn how to install some applications!

Note: The lab starts with your user account, called analyst, already logged in to the Bash shell. This means you can start with the tasks as soon as you click the Start Lab button.

Task 1. Ensure that APT is installed
First, you’ll check that the APT application is installed so that you can use it to manage applications. The simplest way to do this is to run the apt command in the Bash shell and check the response.

The Bash shell is the command-line interpreter currently open on the left side of the screen. You’ll use the Bash shell by typing commands after the prompt. The prompt is represented by a dollar sign ($) followed by the input cursor.

Confirm that the APT package manager is installed in your Linux environment. To do this, type apt after the command-line prompt and press ENTER.

The command to complete this step:

1
apt
When installed, apt displays basic usage information when you run it. This includes the version information and a description of the tool:

123456789
apt 1.8.2.3 (amd64)
Usage: apt [options] command

apt is a commandline package manager and provides commands for
searching and managing as well as querying information about packages.
It provides the same functionality as the specialized APT tools,
like apt-get and apt-cache, but enables options more suitable for
interactive use by default.
...
APT is already installed by default in the Linux Bash shell in this lab because this is a Debian-based system. APT is also the recommended package manager for Debian. If you’re using another distribution, a different package manager, such as YUM, may be available instead.

Task 2. Install and uninstall the Suricata application
In this task, you must install Suricata, a network analysis tool used for intrusion detection, and verify that it installed correctly. Then, you’ll uninstall the application.

Use the APT package manager to install the Suricata application.

Type sudo apt install suricata after the command-line prompt and press ENTER.

The command to complete this step:

1
sudo apt install suricata
Note: The apt install and apt remove commands must be prefixed with the sudo command as elevated privileges are required to install and uninstall software in Linux.

The Suricata application can take a few minutes to install.

When you install an application with APT, the output displays details of all the software to be installed. This may include additional applications that depend on the new software. These additional applications are called the dependencies of the software to be installed.

When prompted to continue, press the ENTER key to respond with the default response. (In this case, the default response is Yes.)

Verify that Suricata is installed by running the newly installed application.

Type suricata after the command-line prompt and press ENTER.

The command to complete this step:

1
suricata
When Suricata is installed, version and usage information is listed:

123456
Suricata 4.1.2
USAGE: suricata [OPTIONS] [BPF FILTER]

    -c   : path to configuration file
    -T         : test configuration file (use with -c)
...
3. Use the APT package manager to uninstall Suricata.

Type sudo apt remove suricata after the command-line prompt and press ENTER. Press ENTER (Yes) when prompted to continue.

The command to complete this step:

1
sudo apt remove suricata
When prompted to continue, press the ENTER key to respond with the default response. (In this case, the default response is Yes.)

4. Verify that Suricata has been uninstalled by running the application command again.

Type suricata after the command-line prompt and press ENTER.

The command to complete this step:

1
suricata
If you have uninstalled Suricata, the output is an error message:

1
-bash: /usr/bin/suricata: No such file or directory
This message indicates that Suricata can't be found anymore.

Task 3. Install the tcpdump application
In this task, you must install the tcpdump application. This is a command-line tool that can be used to capture network traffic in a Linux Bash shell.

Use the APT package manager to install tcpdump.

Type sudo apt install tcpdump after the command-line prompt and press ENTER.

The command to complete this step:

1
sudo apt install tcpdump
Task 4. List the installed applications
Next, you need to confirm that you’ve installed the required applications. It's important to be able to validate that the correct applications are installed. Often you may want to check that the correct versions are installed as well.

1. Use the APT package manager to list all installed applications.

Type apt list --installed after the command-line prompt and press ENTER.

The command to complete this step:

1
apt list --installed
This produces a long list of applications because Linux has a lot of software installed by default.

2. Search through the list to find the tcpdump application you installed.

The Suricata application is not listed because you installed and then uninstalled that application:

123
...
tcpdump/oldstable,now 4.9.3-1~deb10u2 amd64 [installed]
...
Note: The specific version of tcpdump that you see displayed may be different from what is shown above.

Task 5. Reinstall the Suricata application
In this task, you must reinstall the Suricata application and verify that it has installed correctly.

1. Run the command to install the Suricata application.

Type sudo apt install suricata after the command-line prompt and press ENTER.

The command to complete this step:

1
sudo apt install suricata
When prompted to continue, press the ENTER key to respond with the default response. (In this case, the default response is Yes.)

2. Use the APT package manager to list the installed applications.

Type apt list --installed after the command-line prompt and press ENTER.

The command to complete this step:

1
apt list --installed
3. Search through the list to confirm that the Suricata application has been installed.

The output should include the following lines:

12345
...
suricata/oldstable,now 1:4.1.2-2+deb10u1 amd64 [installed]
...
tcpdump/oldstable,now 4.9.3-1~deb10u2 amd64 [installed]
...
Conclusion
Great work!

You now have practical experience with the APT package manager. You learned to

install applications,

uninstall applications, and

list installed applications.

Being able to manage installed applications in Linux is a key skill for any security analyst.


# 🐚 Understanding Different Types of Shells in Linux

## 💡 Why Shells Matter in Cybersecurity

Knowing how to work with Linux shells is a vital skill for cybersecurity professionals. Shells are used for a wide range of tasks—from running simple commands to automating complex operations. In this note, we'll review the concept of shells and introduce various types, including the one you'll use in this course.

---

## 🗣️ What Is a Shell?

A **shell** is a command-line interpreter. Think of it as a *translator* between you and the computer's operating system.

- When you type a command, the shell interprets it, sends it to the kernel, and displays the result.
- It's your primary tool for interacting with the system without a graphical interface.

---

## 🧵 Types of Linux Shells

There are several types of shells available on Linux systems. Each shell has its own features, syntax rules, and use cases.

| Shell                         | Description                                                                 |
|------------------------------|-----------------------------------------------------------------------------|
| **Bourne-Again Shell (bash)**| Default on most Linux distributions. Widely used and beginner-friendly.     |
| **C Shell (csh)**             | Syntax resembles the C programming language.                                |
| **Korn Shell (ksh)**          | Combines features of both Bourne shell and C shell.                         |
| **Enhanced C Shell (tcsh)**   | An improved version of C shell with auto-completion and other enhancements. |
| **Z Shell (zsh)**             | Feature-rich and user-customizable. Often preferred by power users.         |

**Prompt Differences**  
- `bash`, `ksh` → `$` prompt  
- `zsh`, `csh` → `%` prompt

---

## 🧰 Bash: The Default and Preferred Shell

- **Bash** is the default shell for most Linux distributions.
- It’s beginner-friendly and supports scripting, job control, and command history.
- Bash is **heavily used in cybersecurity** because of its versatility and wide adoption.
- In this course, you'll primarily be working with **bash**.

---

## 📝 Key Takeaways

- Shells are crucial for interacting with Linux systems.
- They act as a bridge between the user and the kernel.
- There are several shell types—each with its strengths.
- **Bash** is the most commonly used shell, especially in cybersecurity.

# 🖥️ Input and Output in the Bash Shell

## 🔍 Activity Overview

Previously, you explored how the Bash shell helps you communicate with a computer’s operating system. In this activity, you'll dive deeper by examining how the shell receives **input** and returns **output** or **error messages**.

You'll work with:

- `echo` for text output
- `expr` for basic calculations
- `clear` to clean the shell screen

This foundational knowledge is essential for any cybersecurity professional working in a Linux environment.

---

## 🧪 Scenario

As a security analyst, you’ll often need to:

- Input commands into the shell  
- Interpret the output or identify errors  

In this activity, you'll simulate real-world tasks like echoing messages and calculating alert metrics.

---

## 🛠️ Task 1: Generate Output with the `echo` Command

The `echo` command outputs a string of text to the terminal.

### 1. Basic Output

#bash
echo hello

# 📁 Filesystem Hierarchy Standard (FHS) & Linux Command Guide

## 🔗 Filesystem Hierarchy Standard (FHS)

### Root Directory `/`
- The top-level directory in Linux.
- All other directories branch from here.

### Standard FHS Directories

| Directory | Description |
|----------|-------------|
| /home  | Contains personal directories for users. |
| /bin   | Stores essential binary/executable files. |
| /etc   | System configuration files. |
| /tmp   | Temporary files (accessible by all users). |
| /mnt   | Mount point for external storage like USBs. |

---

## 🧭 Understanding Paths

### Absolute Path
- Starts from the root /.
- Example: /home/analyst/projects

### Relative Path
- Based on current working directory.
- Symbols:
  - . = current directory
  - .. = parent directory
- Example: ../projects

### Tilde `~`
- Represents the user's home directory.
- Example: ~/logs = /home/username/logs

---

## 📂 Navigation Commands

| Command | Description | Example |
|---------|-------------|---------|
| pwd | Print working directory (absolute path). | /home/analyst |
| ls | List contents of directory. | ls, ls projects, ls /home/analyst |
| cd | Change directory. | cd .., cd /home/analyst/logs |

> 💡 Use whoami to print your current username.

---

## 📄 Reading File Content

| Command | Description | Example |
|---------|-------------|---------|
| cat | View full file contents. | cat updates.txt |
| head | View first 10 lines. | head updates.txt |
| head -n 5 | View first 5 lines. | head -n 5 updates.txt |
| tail | View last 10 lines. | tail updates.txt |
| less | Paginated view of file contents. | less updates.txt |

### `less` Keyboard Controls

| Key | Action |
|-----|--------|
| Space | Next page |
| b | Previous page |
| ↓ / ↑ | Move one line |
| q | Quit less |

---

## 🛡️ Key Takeaways for Security Analysts

- Navigate the Linux filesystem confidently.
- Understand the difference between absolute and relative paths.
- Master essential navigation (`pwd`, `ls`, `cd`) and file reading commands (`cat`, `head`, `tail`, `less`).
- Use commands efficiently to access logs, configs, and other critical files.

---
