# HACS100 Midterm Review

## 1. Intro to UNIX  
- **UNIX**: A family of operating systems.  
- **Connections**: Terminal emulation or secure shell (ssh, Windows Terminal, Putty, MobaXTerm).  
- **Prompt**: Indicates the shell is ready for commands.  
- **Components**:  
  - Unified file system  
  - Kernel  
  - Processes  
  - Shell  

---

## 2. Command Line Basics  
- **Shells**: BASH, C-shell, T-shell, etc., interpret typed commands.  
- **Commands**:  
  - `finger [loginID]`: Find user information  
  - `man [command]`: Open manual page for a command  
  - `exit`: Close shell  
  - `logout`: Close login shell  

---

## 3. Directories and Files  
- **Structure**: Tree-like with root `/`.  
- **Commands**:  
  - `pwd`: Print working directory  
  - `cd`: Change directory  
  - `ls`: List directory contents  
  - `mkdir` / `rmdir`: Create or remove directories  
  - `touch filename`: Create an empty file  
  - `rm filename`: Remove a file  
  - `cat filename`: Display file contents  

---

## 4. Text Editors (Vim & Nano)  
- **Vim Modes**: Insert, Command, and Last Line.  
  - `i`: Enter insert mode  
  - `u`: Undo in command mode  
  - `:wq`: Write and quit  
- **Nano**: No modes, simpler to use.  

---

## 5. Permissions  
- **Listing Permissions**: `ls -l`  
- **Changing Permissions**: `chmod`  
  - `u, g, o, a`: User, group, others, all  
  - `r, w, x`: Read, write, execute  

---

## 6. Variables  
- **Types**: Local (current shell), Global (available to child processes).  
- **Usage**:  
  - `myVar="value"`: Assign value  
  - `echo $myVar`: Access value  
- **Export**: `export MYVAR`  
- **Quoting**:  
  - Single: Literal  
  - Double: Interpret variables  
  - Back: Execute commands  

---

## 7. Wildcards  
- **Asterisk (*)**: Matches 0 or more characters.  
- **Question Mark (?)**: Matches exactly one character.  
- **Square Brackets ([ ])**: Match specific characters or ranges.  
- **Curly Braces ({ })**: Match one word from a list.  

---

## 8. Writing Shell Scripts  
- **Basics**: Commands stored in files and executed sequentially.  
- **Create & Run**:  
  - Use editors like `vim` to write scripts.  
  - `chmod +x scriptname`: Make executable.  
  - `./scriptname`: Run the script.  

---

## 9. Conditionals  
- **Comparisons**:  
  - Numeric: `-eq`, `-ne`, `-lt`, `-gt`  
  - String: `=`, `!=`  
  - File tests: `-e`, `-f`, `-d`, `-r`, `-w`, `-x`  
- **Structure**:  
  ```bash
  if [[ cond1 ]]; then
    statement1
  elif [[ cond2 ]]; then
    statement2
  else
    statement3
  fi
