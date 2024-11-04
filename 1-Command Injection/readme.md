<img src="https://assets.tryhackme.com/img/badges/introtowebsecurity.svg" length = 125, width = 125>

# 1: Command Injection
"Command Injection" was the first lab I did with TryHackMe. It's an Easy lab that covers the basics of exploiting vulnerabilities using command injection.
The lab itself consisted of trying different payloads to see what the vulnerable application would return. It almost felt like I was trying to brute-force the application,
as I had to try different payloads over and over again to try to get a response from the application. 

I could find what user the application was running as by inputting `;whoami` and to find the flag, I used the payload `;cat /home/tryhackme/flag.txt`. By the end of the lab, 
I learned that there are many variations of the same payload. Some had the `|` in front, and some had `$` in front. For this lab, the semicolon (`|`) worked. 

Command injection can be easily prevented via **input sanitization.** We check whether or not the input is valid. We can look for certain characteristics. For example, the input must be a number between 0 and 9. Otherwise, we will reject it.

### Summary
I learned:
- How to discover the command injection vulnerability
- How to test and exploit this vulnerability using payloads designed for different operating systems
- How to prevent this vulnerability in an application
- Applying my learning by performing command injection in a practical application
