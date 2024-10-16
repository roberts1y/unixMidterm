# Midterm Review: Introduction to UNIX and Shell Programming

## **Key UNIX Concepts**
- **UNIX**: A family of operating systems with a unified file system, kernel, processes, and shell.
- **Connecting to Virtual Machine**:
  * Use `ssh`, Windows Terminal, or PuTTY/MobaXTerm.
- **Shells Available**:
  * BASH, C-shell, T-shell, etc.  
  * **Usage**: Interpret typed commands and run them.

## **Command Line Basics**
- **Useful Commands**:
  * `finger [loginID]`: Find user info.
  * `man [command]`: Open manual page.
  * `pwd`: Print working directory.
  * `ls`: List directory contents.
  * `mkdir` / `rmdir`: Create or remove directories.
  * `rm filename`: Remove a file.
- **Vim Editor Basics**:
  * **Modes**: Insert, Command, Last line.
  * Commands:
    * `i`: Enter Insert mode.
    * `Esc`: Return to Command mode.
    * `:wq`: Save and quit.
- **Nano Editor Basics**: No modes.  
  * `CTRL + O`: Save, `CTRL + X`: Exit.

## **Permissions and Directory Management**
- **File and Directory Permissions**:
  * `chmod` to change permissions.
  * Read (r), Write (w), Execute (x).
- **Permissions Application**:
  * Files: Controls reading, editing, and executing.
  * Directories: Controls listing contents and access.
- **Octal Notation for Permissions**:
  * User: 4 (read), 2 (write), 1 (execute).

## **Shell Variables**
- **Variable Types**:
  * Local (restricted to shell) and Global/Exported (available to child processes).
- **Creating Variables**:
  * `myVar="value"`  
  * Access: `echo $myVar`
  * Exporting: `export MYVAR`

## **Wildcards and Scripts**
- **Wildcards**:
  * `*`: Matches 0+ characters.
  * `?`: Matches 1 character.
  * `[abc]`: Matches one character from set.
  * `{word1,word2}`: Matches listed words.
- **Shell Scripts**:
  * Store and execute commands sequentially.
  * Start a script:  
    ```bash
    ./scriptname
    chmod +x scriptname
    ```
  * First line: `#!/bin/bash`

## **Conditionals and Loops**
- **Conditionals**:
  * `if`, `elif`, `else` structures.
  * Comparisons: `-eq`, `-ne`, `-lt`, `-gt`.
- **While Loop Example**:
  ```bash
  num=0  
  while [[ $num -lt 3 ]]; do
    echo $num
    num=$(( num + 1 ))
  done
