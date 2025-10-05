# Binary Exploitation

First off, what's a  binary?

A binary is compiled code. When a programmer write code in a language say C, its not what the code is executed. It is compiled to binary, which consists of set of instructions called machine code, and then the binary is run. 
Binary exploitation is the art of finding and exploitaing a bug that survives the compilation step.


## Reverse engineering 

Reverse Engineering is figuring out how something works. It is yet another broad topic. It is required in Binary exploitation as most of the time we are only given a binary. We have to figure out how it works, before trying to attack it.

## Prerequisites

Before jumping into pwn (shorthand for binary exploitation), make sure you're confortable with
- Basics of C (arrays,strings, pointers)
- Fundamentals of assembly and CPU architecture
- Memory layout of C program.
- Basic Linux commands
- Use these resources before going further.
	- [How Assembly Functions Work- The Stack explained](https://www.youtube.com/watch?v=u_-oQx_4jvo)
	- [x86 Assembly Crash Course](https://www.youtube.com/watch?v=75gBFiFtAb8)
	- [Memory Layout of a C program](https://aticleworld.com/memory-layout-of-c-program/)
	- [LiveOverflow playlist](https://youtube.com/playlist?list=PLhixgUqwRTjxglIswKp9mpkfPNfHkzyeN&si=gST9Zj6WNopbb7kp)


## Tools
 - A disassembler - **GHIDRA** First thing we'll need is a tool that'll convert the machine code of binary back to Assembly ( and possibly try to get C code from Assembly). Ghidra is a powerful disassembler as well as decompiler . Follow the Ghidra installation from Pclub infosec roadmap then watch [this](https://www.youtube.com/watch?v=fTGTnrgjuGA&t=67s) .
 - A debugger - **GDB**, this is a defualt debugger packed along with GCC for decompiling binaries. However, to enhance GDB and make it easier to use and more powerful, we'll add a plugin on top of this. Install pwndbg from [here](https://pwndbg.re/pwndbg/latest/setup/). Use this [guide](https://www.youtube.com/watch?v=5judobmDBKI) to understand the basics command.
 - (Optional for now) **Pwntools** - Its a python library that makes write exploit scripts easier  by automating the booring part. [Github](https://github.com/Gallopsled/pwntools)


## Warmup
Now that you have the tools necessary for the job, head over to picoCTF and solve these [GDB baby steps](https://play.picoctf.org/practice?page=1&search=gdb%20baby%20step)  challenges then  [k3yg3n](https://crackmes.one/crackme/5da31ebc33c5d46f00e2c661) one from Crackme.

## Your First Binary Exploit 

The first bug, we'll understand is the Stack Buffer Overflow. It is vulnerability in which data can be written which exceeds the allocated space on stack and allows the attack to overwrite other data. 
- Watch [this](https://www.youtube.com/watch?v=T03idxny9jE) video from LiveOverFlow to watch how stack overflow happens. 
- Then head over to this [git repo](https://guyinatuxedo.github.io/04-bof_variable/csaw18_boi/index.html) and follow along with the writeups on with the tools you got.
Try to follow along with the tools you have to get hands-on practice.


# Further Resources
 To dive deeper into the world of low level, follow these resources
 
 - Nightmare Walkthrough
 - Pwn.college
 - LIve overflow
