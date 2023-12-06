# COMP520---Operating-Systems-Principles

# ProjectA Explanation (kernel.c)
The code writes "Hello World" to the screen by accessing video memory at address 0xb800. It iterates through the string, writing characters and color attributes to consecutive memory locations. The 'putInMemory' function writes characters and attributes, incrementing the memory offset. The code forms the phrase "Hello World" in white text on a black background before entering an infinite loop. It's important to note that the provided description does not include all the code and may reference additional functions that are not explicitly mentioned.

To verify the code, run these commands in the terminal chmod + x compileOS.sh and ./compileOS.sh. If you’re done without any error, then run the java -jar simulator.jar 

# ProjectB Explanation (kernel.c)
The main function reads user input, prints messages to the screen, and demonstrates reading a sector from a disk. It relies on handleInterrupt21 to handle various interrupt-driven functions, such as printing and reading strings, and sector reading. The code also defines functions for printing characters and new lines and handles backspace during string input. It's important to note that the provided description does not include all the code and may reference additional functions that are not explicitly mentioned.

To verify the code, run these commands in the terminal chmod + x compileOS.sh and ./compileOS.sh. If you’re done without any error, then run the java -jar simulator.jar 

# ProjectC Explanation (kernel.c and shell.c)
The kernel initializes an interrupt vector table, reads a file named "message" into a buffer, and prints its content. If the file is not found, it launches a simple shell. The kernel includes functions for file system operations, I/O functions, and program execution. The termination function in the kernel executes a program named "shell" to return to the command prompt. 

The shell, defined in shell.c, enters a perpetual loop, accepting user input and interpreting commands. It supports commands like "type" to display file content and "exec" to execute programs. If the shell encounters unrecognized commands, it prints appropriate error messages. In summary, this code interacts with hardware through interrupt calls, and the file system and shell provide basic functionality for a simple operating system environment. It's important to note that the provided description does not include all the code and may reference additional functions that are not explicitly mentioned.

To verify the code, run these commands in the terminal chmod + x compileOS.sh and ./compileOS.sh. If you’re done without any error, then run the java -jar simulator.jar 
