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

##🎯 Objective

The main objective of the project is to gain a deep understanding of:

How UNIX pipes and file descriptors work.

How to create and manage child processes using fork and execve.

How to handle errors, memory, and process synchronization safely.

In short, this project teaches you how to programmatically replicate shell behavior and manage inter-process communication — a core concept in systems programming and operating systems.
