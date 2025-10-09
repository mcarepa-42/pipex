# 🛠 Pipex  
> *Explore UNIX pipes by implementing them in C.*

The **Pipex** project is part of the **42 curriculum** and focuses on understanding **UNIX pipes**, **process management**, and **I/O redirection** in C.  
It is inspired by how shell commands connect through pipes and how data flows between processes.

---

## 🪑 Project Goal
You must simulate shell command execution by connecting commands with **pipes**.  
Each command reads input from a file or previous command and outputs to a file or next command.  

The challenge is to:
- Properly handle **forks, execve, and pipes**.  
- Correctly manage **file descriptors** and **redirections**.  
- Prevent **memory leaks** and unexpected crashes.  
- Replicate shell behavior **exactly**, including chaining multiple commands.

---

## ⚙️ Technical Overview
- Written in **C**, following the **42 Norm**.  
- **Mandatory part:** Handle a single pipe connecting two commands:  
```bash
< file1 cmd1 | cmd2 > file2


