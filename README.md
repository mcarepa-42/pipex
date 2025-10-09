# 42 Projects: Philosophers & Pipex

---

## 🧠 Philosophers
> *“I never thought philosophy would be so deadly.”*

The **Philosophers** project is part of the **42 curriculum**, exploring **multithreading**, **synchronization**, and **concurrency** in C.  
It is inspired by the classic *Dining Philosophers Problem*, which teaches resource sharing and concurrency control.

### 🪑 Project Goal
Simulate a group of philosophers sitting around a table with a bowl of spaghetti.  
Each philosopher alternates between **eating**, **sleeping**, and **thinking**, but must pick up **two forks** to eat — one on each side.

**Objectives:**
- Prevent **deadlocks**.
- Avoid **data races**.
- Ensure no philosopher **starves**.
- Accurately log philosopher states.

### ⚙️ Technical Overview
- Written in **C**, following the **42 Norm**.
- **Mandatory part:** Uses **threads** and **mutexes**.
- **Bonus part:** Uses **processes** and **semaphores**.
- State logs:
  - Taking forks
  - Eating
  - Sleeping
  - Thinking
  - Dying

---

## 🛠 Pipex
> *Explore UNIX pipes by implementing them in C.*

The **Pipex** project (42 curriculum) teaches **UNIX pipes** and **process handling**.  
The goal is to replicate shell behavior by connecting commands with **pipes** and handling file input/output.

### 🪑 Project Goal
Your program should simulate the following shell command:

```bash
< file1 cmd1 | cmd2 > file2

