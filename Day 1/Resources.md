# Day 1 - Introduction
Hello guys! Welcome to the world of hacking and cyber security. 
First things first, lets talk about what motivates you towards this domain! Pretty black-green movie screens, commands going on...and boooom-"HACKED"!

### So, what is Infosec?
Information security (Infosec) is about protecting information and systems from unauthorized access or misuse. It’s about learning how systems work so you can defend them — and sometimes break them in **legal** environments (to learn xD).

### Some basics before we start...
These will help you in understanding things more quickly. Have a quick look:
1. **The Basics of Number Systems**
    Study number systems and their types [here](https://www.rapidtables.com/math/number/Numeral_system.html
).
2. **Explore ASCII Encoding**
Understand ASCII encoding [here](https://www.ascii-code.com/).
3. **Types of hacking**
For more motivation and ethics have a look on the types of hacking [here](https://www.geeksforgeeks.org/computer-networks/types-of-hacking/
).

---

## Linux
### Why Linux, why not Windows?

Linux is the preferred OS for most cybersecurity works, because in short it gives you control, flexibility, and the right environment to explore use tools and commands used to in this domain ( also the root access ;)  )— whereas Windows is more restrictive. To learn more on why linux is preferred, see [this](https://www.mygreatlearning.com/blog/linux-vs-windows/
) and [this articles](https://dev.to/arunammisetty/what-is-linux-and-why-do-hackers-use-it-47ln
).

### Installing Linux

There are multiple options such as Virtual Machine(VM), WSL, dual boot. But for now we will go on with VM. We are going on with Kali Linux as its specially made for hacking related stuffs!

See [this](https://youtu.be/sAMnXte56yY?si=ae0Z3wRXYb-lqORd
) video, it will help you on it.

### Core Linux Commands

Linux has a whole lot of commands to help you to do stuffs through the command prompt (CMD). Some have been listed... you need not remember these, you will be acquainted with these as you start to use linux.

The linux command [cheat sheet](https://www.reddit.com/media?url=https%3A%2F%2Fpreview.redd.it%2Fisnefnt32wn21.jpg%3Fauto%3Dwebp%26s%3Db6c48a27ab33a3d428b554d278eba617e35bf3a2).

Some are listed below, you can check details about them using the help menu or the man pages of the commands. Format:
<command name> -h or man <command name>.

For now just have a look.

**Navigation & Info**
```bash
pwd          # show current directory
ls        # list all files 
cd ..        # go up one directory
whoami       # current user
uname -a     # system info
```
**File ops**
```bash
cat file.txt            # view file
less file.txt           # paged view
cp src dest             # copy file
mv file1 file2          # move or rename
rm file                 # remove file
mkdir newdir            # make directory
touch file.txt          # create empty file or update timestamp
```
**Permissions & owners**
```bash
ls -l                   # view permissions and owner/group
chmod +x file.sh       # change permissions (rwxr-xr-x)
```
**Text tools (very handy)**
```bash
grep 'pattern' file     # search lines
find . -name '*.txt'    # find files by name
wc -l file              # count lines
sort file | uniq -c     # count unique lines
```
And many more..
"|" this is the pipe. You may learn more as you go ;).

#### Commads to  work with networking:

- ssh: remote shell
    ```
    Eg: ssh bandit0@bandit.labs.overthewire.org -p 2220
    ```
- scp: copy files over ssh
- nc (netcat): swiss army network tool
    ```
    Eg:
    nc -l -p 1234            # listen on port 1234
    echo "hello" | nc host 1234   # send data to host:port
    ```
    
---
## Over the wire Bandit:

Bandit is a fun way to learn Linux filesystems and commands. You would like to have a try on it. Try to do atleast till level 7 for the day... You may continue further( you should actually xD)

https://overthewire.org/wargames/bandit/

It will give you a structured way to use various commands of Linux. See the details given in each level and go on. 

**Note** : As this is a reputed resource to learn about linux commands, there are already a lot of writeups present on internet. But you should, try your best to solve every level on your own without looking at others solutions.

**Internet and manual pages are your go to place for any help!**

---
## CTFs:
### What are CTFs (Capture The Flag) and Subdomains?
CTFs (Capture the Flags) are infosec events where there are multiple infosec challenges related to various domains like rev , pwn , crypto , OSINT, forensics etc. are made available to participants where , which upon solving they find a text hidden by the problem maker called a flag. It’s not a country’s flag (xD) . These events can be held both online and on-site. Some of the famous CTFs are Insomni’hack, GoogleCTF, PlaidCTF, TCTF.

A typical CTF flag would look something like : **pclub{CTFs_ar3_fun!}**

- **Purpose:** Learn and practice cybersecurity skills in a safe, legal environment. 

**Why CTFs are useful for beginners:**
- Helps develop problem-solving skills.
- Builds familiarity with Linux commands, networking tools, and scripting.
- Encourages learning by doing, which builds intuition for cybersecurity tasks.

### Subdomains:
- Forensics
- Cryptography
- Web Exploitation
- Osint
- Reverse Engineering and Binary exploitation

Lets see you further...


