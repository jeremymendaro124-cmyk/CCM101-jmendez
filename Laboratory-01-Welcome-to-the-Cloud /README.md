# Linux Laboratory Activities

## Mission Overview

This laboratory activity focuses on developing practical skills in Linux system administration and command-line operations. Throughout the laboratory activities, I will learn how to navigate the Linux environment, manage files and directories, create and manage user accounts, and use Bash commands.

This repository will contain the laboratory activities completed throughout the semester and will serve as a record of my learning and progress.

## Objectives

The objectives of this laboratory are to:

* Learn the basic Linux command-line interface.
* Understand and use Bash commands.
* Create and manage Linux user accounts.
* Configure user home directories and Bash shells.
* Manage user permissions and sudo access.
* Navigate and manage files and directories.
* Identify system information such as the username, working directory, and hostname.
* Develop practical Linux system administration skills.

## Activities Performed

The following activities were performed during the laboratory:

1. Navigated the Linux terminal using Bash commands.
2. Created a new Linux user account.
3. Created a home directory for the new user.
4. Configured the Bash shell for the new user.
5. Set a password for the new user.
6. Added the new user to the `sudo` group.
7. Logged in to the newly created user account.
8. Checked and recorded the current username.
9. Checked and recorded the current working directory.
10. Checked and recorded the hostname of the Linux system.
11. Captured a screenshot showing the required system information.

## Linux Commands Used

| Command    | Purpose                                          |
| ---------- | ------------------------------------------------ |
| `sudo`     | Executes commands with administrator privileges. |
| `useradd`  | Creates a new Linux user account.                |
| `passwd`   | Sets or changes a user's password.               |
| `usermod`  | Modifies an existing user account.               |
| `su`       | Switches to another user account.                |
| `whoami`   | Displays the current username.                   |
| `pwd`      | Displays the current working directory.          |
| `hostname` | Displays the hostname of the computer.           |
| `echo`     | Displays text or command output in the terminal. |

### Commands Used in the Activity

```bash
sudo useradd -m -s /bin/bash jmendez
sudo passwd jmendez
sudo usermod -aG sudo jmendez
su - jmendez
whoami
pwd
hostname
```

To display all required information in one screen:

```bash
echo "Current Username: $(whoami)"
echo "Current Working Directory: $(pwd)"
echo "Hostname: $(hostname)"
```

## Skills Learned

Through this laboratory activity, I learned how to:

* Use the Linux Bash terminal.
* Create and manage user accounts.
* Set and manage user passwords.
* Configure a user's home directory and shell.
* Assign sudo privileges.
* Switch between Linux user accounts.
* Check basic system information.
* Understand the purpose of common Linux commands.
* Follow proper procedures when performing system administration tasks.
* Document laboratory activities using GitHub and Markdown.

