
# Learnathon: Infosec

## Day 4: Web Exploitation

Today we will be learning about web exploitation. As a prereq to getting into "web exploitation", understanding the most common web frameworks is a good way to indentify potential targets.

Its exploiting various dev or architectural related vulnerabilities that exists in web apps to gain unauthorized access to privileged resources.
You will be surprised that these vulnerabilties do exist in even the most popular apps you use everyday. 
[Ethical hackers](https://www.blackduck.com/glossary/what-is-ethical-hacking.html) exploit these and report them to respective companies as a part of [bug bounty programmes](https://www.hackerone.com/bug-bounty-programs). 


### Foundations

To get started with web exploitation, we need to know a little about how web actually works.
Here are some basics so you all don't end up copy-pasting payloads without any clue.

1. HTML/CSS/JS: You don't know need to become frontend devs, just know how these interact with each other. 
2. HTTP overview by MDN: [Link](https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/Overview)

**Tip**: Browser DevTools (Inspect → Elements, Network tab, Application tab) will be your microscope. Practice watching requests, cookies, and API calls before touching other tools.

### Website Security

1. Basics by PicoCTF: [Link](https://picoctf.org/learning_guides/Book-3-Web-Exploitation.pdf)
2. OWASP Top 10: [Link](https://owasp.org/www-project-top-ten/)
3. Good read: [Link](https://www.csc.ac.za/?page_id=148)
4. Portswigger's Web Security Academy: This contains various labs where you can learn and practice various techniques. [Link](https://portswigger.net/web-security) (Do labs related to OWASP top 10 here)
4. Modern web exploitation techniques by HTB: [Link](https://academy.hackthebox.com/course/preview/modern-web-exploitation-techniques)


You can also read writeups here: https://0xdf.gitlab.io/ to see how CTF players solve challenges.


### Practice and Learning sites

1. [XSS Game](https://xss-game.appspot.com/)
2. [Hacktricks.xyz](https://book.hacktricks.xyz/): This includes a lot of techniques, you can have a look at them and practice at your own pace.
3. OWASP Juice Shop / DVWA / bWAPP → Deliberately vulnerable apps you can install locally.

### Tools
[PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings)  
[Burp Suite](https://portswigger.net/burp)


But remember: Tools amplify skills, not replace them. First learn to work with DevTools + curl, then move to Burp, sqlmap, wfuzz, tqlmap etc.

There are many different types of tools available which you can use for different types of attacks and exploits, just a google search away :) 
You are expected to learn basics of web and basic types of vulnerabilities (namely OWASP top 10) before proceeding in the challenges.
