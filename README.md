# minishell
A simple Unix shell implemented in C, mimicking basic shell behavior like bash. This project focuses on command parsing, execution, and basic shell features such as built-in commands, piping, and redirection.

Features:
- Execute commands with arguments.
- Built-in commands: cd, echo, exit, env, pwd, export, unset.
- Input/output redirection (>, <, >>, <<).
- Piping between commands (|).
- Signal handling (Ctrl+C, Ctrl+D, Ctrl+\).

Requirements:
- GCC or any C compiler
- Unix-like operating system (Linux, macOS)

How to Build:
Clone the repository and compile the code using:

`make`
This will create an executable called minishell.

How to Use:
Run the shell by executing:

`./minishell`
Then you can type commands as you would in a regular shell.

Example:
`ls -l | grep ".c" > output.txt`
Limitations:
- Does not support advanced shell features like job control or scripting
- Limited error handling
