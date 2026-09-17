# What is Shell?

A **shell** is a program that lets you interact with your computer by typing commands.

For example, instead of clicking folders and buttons, you can open a shell and type:

> cd Documents
> ls
> mkdir my-project

The shell reads those commands and asks the operating system to carry them out.

# What is the purpose of Shell?

The **purpose of a shell** is to provide a way for a user to **communicate with and control the operating system** using commands.

### Main purposes of a shell:

1. **Execute commands** — runs programs and system commands.
2. **Manage files and directories** — create, delete, copy, move, and rename files.
3. **Run programs** — start applications and scripts.
4. **Automate tasks** — use shell scripts to perform repetitive tasks automatically.
5. **Manage the system** — control processes, permissions, environment variables, etc.
6. **Connect commands** — combine commands using pipes (`|`) and redirection (`>`, `<`).

### Common shells

- **Bash** — very common on Linux and macOS
- **Zsh** — the default shell on modern macOS
- **PowerShell** — common on Windows
- **Fish** — designed to be more user-friendly

# Shell vs. terminal

They're related but different:

- **Terminal** = the application/window where you interact with the command line.
- **Shell** = the program inside the terminal that interprets your commands.

# BASH Shell

## What is BASH?

**BASH** stands for **Bourne Again SHell** created by Stephen Bourne.

It is a **command-line shell** used to communicate with an operating system, especially **Linux and Unix-like systems**.

### Key features of Bash

- Executes commands such as `ls`, `cd`, `mkdir`, and `cp`
- Allows users to manage files and directories
- Supports **shell scripting** for automation
- Supports variables, loops, conditions, and functions
- Allows commands to be connected using pipes (`|`)
- Can run programs and scripts

# What is a Script?

A **script** is a **file containing a series of commands or instructions that are executed automatically by an interpreter**.

# Structure of A BASH Script

### 1. Beginning

Contains the **shebang** and sometimes comments.

> #!/bin/bash

The shebang tells the system that the script should be executed using Bash.

### 2. Middle

Contains the **main commands and logic** of the script.

>name="John"
 echo "Hello $name"

This is where you perform tasks using variables, commands, conditions, and loops.

### 3. End

Contains the **final commands** and, optionally, an exit status.

> echo "Script completed"
  exit 0

`exit 0` indicates that the script completed successfully.
