# COMP520---Operating-Systems-Principles

# ProjectA Explanation (kernel.c)
The code writes "Hello World" to the screen by accessing video memory at address 0xb800. It iterates through the string, writing characters and color attributes to consecutive memory locations. The 'putInMemory' function writes characters and attributes, incrementing the memory offset. The code forms the phrase "Hello World" in white text on a black background before entering an infinite loop. 

It's important to note that the provided description does not include all the code and may reference additional functions that are not explicitly mentioned.

To verify the code, run these commands in the terminal chmod + x compileOS.sh and ./compileOS.sh. If you’re done without any error, then run the java -jar simulator.jar 

# ProjectB Explanation (kernel.c)
The main function reads user input, prints messages to the screen, and demonstrates reading a sector from a disk. It relies on handleInterrupt21 to handle various interrupt-driven functions, such as printing and reading strings, and sector reading. The code also defines functions for printing characters and new lines and handles backspace during string input. 

It's important to note that the provided description does not include all the code and may reference additional functions that are not explicitly mentioned.

To verify the code, run these commands in the terminal chmod + x compileOS.sh and ./compileOS.sh. If you’re done without any error, then run the java -jar simulator.jar 

# ProjectC Explanation (kernel.c and shell.c)
The kernel initializes an interrupt vector table, reads a file named "message" into a buffer, and prints its content. If the file is not found, it launches a simple shell. The kernel includes functions for file system operations, I/O functions, and program execution. The termination function in the kernel executes a program named "shell" to return to the command prompt. 

The shell, defined in shell.c, enters a perpetual loop, accepting user input and interpreting commands. It supports commands like "type" to display file content and "exec" to execute programs. If the shell encounters unrecognized commands, it prints appropriate error messages. In summary, this code interacts with hardware through interrupt calls, and the file system and shell provide basic functionality for a simple operating system environment. 

It's important to note that the provided description does not include all the code and may reference additional functions that are not explicitly mentioned.

To verify the code, run these commands in the terminal chmod + x compileOS.sh and ./compileOS.sh. If you’re done without any error, then run the java -jar simulator.jar 

# ProjectD Explanation (kernel.c and shell.c)
kernel.c: This file serves as the core of an operating system kernel. It encompasses low-level operations like character printing, string reading, and sector-level file operations. The kernel initializes a simple shell by making use of the makeInterrupt21 function. It also provides fundamental functionalities such as executing programs, handling interrupts, and managing the file system. Notably, the handleInterrupt21 function acts as a system call dispatcher, routing different functionalities based on the value of the ax register. The kernel's role is to facilitate essential operations required for a basic operating system.

shell.c: The shell program operates within the environment established by the kernel. It engages users in a command-line interface, perpetually awaiting input. The isCommand function helps identify and interpret user commands. Supported commands include "type" for displaying file content, "exec" for executing programs, "dir" for listing directory contents, "del" for deleting files, "copy" for copying files, and "create" for creating files. The shell utilizes system calls to communicate with the underlying kernel, enabling users to interact with the file system and execute various operations. Overall, shell.c provides a user-friendly interface for interacting with the rudimentary operating system. 

It's important to note that the provided description does not include all the code and may reference additional functions that are not explicitly mentioned.

To verify the code, run these commands in the terminal chmod + x compileOS.sh and ./compileOS.sh. If you’re done without any error, then run the java -jar simulator.jar 


# ProjectE Explanation (kernel.c and shell.c)
The kernel (kernel.c) orchestrates fundamental OS functionalities, featuring a process management system capable of executing, terminating, and waiting on processes. It maintains an array to track active processes, their stack pointers, and processes currently waiting on others. The kernel supports interrupt handling, including a custom interrupt 21h for system calls and a timer interrupt (int 0x08) for basic time-sharing among processes. The file-related operations include reading and writing sectors, reading files, executing programs, terminating processes, deleting files, and managing process states. A process scheduler within the timer interrupt allocates processor time to active processes, updating their stack pointers and ensuring smooth execution.

The shell (shell.c) serves as the user interface for interacting with the kernel. It supports a set of commands, including "type" for displaying file contents, "exec" and "execb" for executing programs, "dir" for listing files, "del" for deleting files, "copy" for copying files, "create" for creating new files, and "kill" for terminating specific processes. The shell continually awaits user input, interprets commands, and invokes corresponding kernel functionalities to perform file operations or manage processes. This combined system demonstrates a simplified but functional operating environment with the ability to handle basic file operations and process management through a command-line interface.

It's important to note that the provided description does not include all the code and may reference additional functions that are not explicitly mentioned.

To verify the code, run these commands in the terminal chmod + x compileOS.sh and ./compileOS.sh. If you’re done without any error, then run the java -jar simulator.jar 














