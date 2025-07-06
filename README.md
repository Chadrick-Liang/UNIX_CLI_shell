# Welcome to CSEShell by CL01 Team 1 🐚

CSEShell is a custom-built UNIX command-line shell created by CL01 Team 1! This shell mimics the behaviour of common terminal environments, supporting essential built-in commands (cd, help, exit), dynamic environment control and execution of external programs. We also developed system utilities (file search, dynamic library inspection and daemon processes) to showcase OS-level programming in C. CSEShell is built to handle the navigation of directories, managing environment variables and more with efficiency. 

## How to compile & Run shell 

Requirements: Linux environment

Steps to compile & run CSEShell:
-  Open your terminal and navigate to the project directory
  - Optional: clean previous builds (if necessary) using command `make clean`
- Compile the shell and all system programs using command `make`
- Start the shell using command `./cseshell`

## Built-in Functions 

BLABLABLABLABLA

## Additional Features
1. Character ASCII Art 
  - Accessible through commands: `batman`, `cyclops`, `squidward`
  - Example: ‘batman’ outputs Batman in ASCII Art 
  - Adds fun and visually engaging elements to the shell, breaking the monotony of plain text interactions
```bash
batman
```

2. Basic Calculator
  - Accessible through the `calc` command
  - Example: `calc 1+1` outputs 2
  - Be sure to type your equation without any trailing spaces
  - This feature allows users to perform simple arithmetic operations directly within the terminal, including addition, subtraction, multiplication, division.
  - It also includes basic error handling
  - Example: Returns `inf` (which stands for infinity) when a number is divided by zero 

From there, you can execute built-in commands and any of the included system programs (e.g., `find`, `ld`, `ldr`).

## System Programs

- `find.c` - Searches for files in a directory.
- `ld.c` - List the contents of the curent directory.
- `ldr.c` - List the contents of the current directory recursively.

Each program can be executed from the CSEShell once it is running. This starter code only allows the shell to execute a command once before exiting because `execv` replace the entire process' address space. Students need to fix this and allow the shell to prompt for more commands in Programming Assignment 1.

## Files Directory

The `files/` directory contains various text, PDF, and image files for testing the functionality of the CSEShell and its system programs.

## Makefile

The Makefile contains rules for compiling the shell and system programs. You can clean the build by running:

```bash
make clean
```

## Source Directory

Contains all the necessary source code for the shell and system programs. It is divided into the shell implementation (`shell.c`, `shell.h`) and system programs (`system_programs/`).
