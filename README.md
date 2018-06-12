# AES256 Implementation written entirely in Assembly
FASM-Enabled Intel x86 Assembly code, intended for usage in real-mode operating systems.


**This code has only been tested on VirtualBox, and the actual implementation of the algorithm has not been extensively tested itself. USE AT YOUR OWN DISCRETION!**

## Compiling
I assembled the `implementation.asm` with Flat Assembler (https://flatassembler.net/ ) on Windows 10, with no Makefile. The programs that I used were:

* flat assembler 1.71.39
* HxD 1.7.7.0
* VirtualBox 5.2.2

Instead of writing a linker script, for some reason I manually copied the assembled version of implementation.asm into the first sector of a file I created called floppy.img with HxD upon each build. Then, I ran it in VirtualBox to see the result. No debugging tools were used.

While this code should work in Protected and Long Mode, I have not tested it under such running conditions yet.
