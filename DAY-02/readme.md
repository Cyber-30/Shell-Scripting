# Commenting

**Commenting** means adding notes or explanations to your Bash script that are **not executed by the shell**.

In Bash, a comment starts with the **`#` symbol**.

### Single-line comment

" # This is a comment "

echo "Hello"

Bash ignores the line beginning with `#`.

### Comment after a command

echo "Hello"  # Display Hello on the screen

Everything after `#` on that line is treated as a comment.

### Why use comments?

Comments help you:

- Explain what the code does
- Make scripts easier to understand
- Remind yourself what a section does
- Make debugging and maintenance easier

# #!/bin/bash

**`#!/bin/bash` is not treated as an ordinary comment when it appears at the very beginning of an executable script.**

It is called a **shebang** (or hashbang).

> #!/bin/bash

### What happens?

- `#!` → tells the operating system **which interpreter to use**
- `/bin/bash` → specifies that **Bash** should interpret the script

For example:

> #!/bin/bash
  echo "Hello"

If you run:

> ./script.sh

the operating system sees the shebang and effectively says:

> “Use `/bin/bash` to run this script.”

### But why does it start with `#`?

Because the `#!` line has **special meaning to the operating system** when it is the **first line of an executable script**.

If Bash itself reads that line, Bash treats it like a comment and doesn't execute it.

So:

**`#` → normally a comment**  
**`#!` at the beginning → shebang, specifies the interpreter**

That's why this:

> #!/bin/bash

is commonly placed at the **beginning of every Bash script**.

# 5 pieces of information we use to make our script professional:

1. Author: Alex
2. Date of creation: 00 Mon Year
3. Date of script was last modified: 00 Mon Year
4. Description: Short description
5. Script Usage: backup script

# Example 

Make a script that you can easily backup all the files in your home directory.
Also consider this script will be very useful for others in the organization.
Make sure the script is professionally formatted before sharing it

>  Author: Alex
   Date of creation: 00 Mon Year
   Date of script was last modified: 00 Mon Year
   Description: Short description
   Script Usage: backup script
   tar -cvf ~/directory/my_backup"$(date +%d-%m-%y_%H-%M-%S)".tar ~/* 2> /dev/null
   exit 0 
