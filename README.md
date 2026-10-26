# Linux Mini Shell Implementation in C

## 📌 Project Overview

The **Linux Mini Shell** is a command-line interpreter developed using C to understand Linux system programming and process management. It executes built-in and external commands and supports features such as pipes, signal handling, and basic job control.

## ✨ Features

- **Command Execution:** Executes external commands using `fork()` and `execvp()`.
- **Built-in Commands:** Supports commands such as `cd`, `pwd`, and `exit`.
- **Environment Information:** Supports `echo $$`, `echo $?`, and `echo $SHELL`.
- **Pipelines:** Executes commands connected using the pipe (`|`) operator.
- **Signal Handling:** Handles signals such as `SIGINT`, `SIGTSTP`, and `SIGCHLD`.
- **Job Control:** Provides basic foreground and background job management using `jobs`, `fg`, and `bg`.
- **Custom Prompt:** Supports prompt customization through `PS1`.
- **Job Tracking:** Uses linked lists to maintain job information.
- **Terminal Output:** Supports colored terminal output.

## 🛠️ Technologies Used

- **Programming Language:** C
- **Operating System:** Linux (Ubuntu)
- **Compiler:** GCC
- **System Calls:** `fork()`, `execvp()`, `waitpid()`
- **Concepts:** Process management, signals, pipes, file descriptors, and linked lists
- **Build Tool:** Makefile

## 📂 Project Structure

```text
Linux-Mini-Shell/
├── main.c
├── builtin.c
├── external.c
├── signal.c
├── minishell.h
├── mini.txt
└── Makefile
```

*Note: Update the filenames above if your actual project structure differs.*

## ⚙️ Installation and Execution

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd Linux-Mini-Shell
```

### 2. Compile the Project

```bash
make
```

### 3. Run the Shell

```bash
./MINISHELL.exe
```

### 4. Clean Build Files

```bash
make clean
```

## 💻 Example Commands

```bash
pwd
ls
echo $$
echo $?
ls | wc
sleep 20
```

## 📚 Key Learnings

- Understood process creation and program execution using POSIX system calls.
- Learned how to implement command pipelines using pipes and file descriptors.
- Gained experience in signal handling and basic job control.
- Practiced organizing C programs using header files, modular programming, and Makefiles.
- Improved debugging skills in a Linux development environment.

## 🚀 Future Improvements

- Improve command parsing and error handling.
- Add support for input and output redirection.
- Expand support for shell features and environment variables.
- Improve background process management.

## 👨‍💻 Author

**Yogeswara Reddy Gajulapalli**
