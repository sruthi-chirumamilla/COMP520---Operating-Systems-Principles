# COMP520---Operating-Systems-Principles

# ProjectA Explanation
The code writes "Hello World" to the screen by accessing video memory at address 0xb800. It iterates through the string, writing characters and color attributes to consecutive memory locations. The 'putInMemory' function writes characters and attributes, incrementing the memory offset. The code forms the phrase "Hello World" in white text on a black background before entering an infinite loop.

To verify the code, run these commands in the terminal chmod + x compileOS.sh and ./compileOS.sh. If you’re done without any error, then run the java -jar simulator.jar 

# ProjectB Explanation
The main function reads user input, prints messages to the screen, and demonstrates reading a sector from a disk. It relies on handleInterrupt21 to handle various interrupt-driven functions, such as printing and reading strings, and sector reading. The code also defines functions for printing characters and new lines and handles backspace during string input. 

To verify the code, run these commands in the terminal chmod + x compileOS.sh and ./compileOS.sh. If you’re done without any error, then run the java -jar simulator.jar 
