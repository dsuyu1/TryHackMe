# 1: Command Injection
"Command Injection" was the first lab I did with TryHackMe. It's an Easy lab that covers the basics of exploiting vulnerabilities using command injection.

To begin with, let’s first understand what command injection is. Command injection is the abuse of an application's behavior to execute commands on the operating system, using the same privileges that the application on a device is running with. For example, achieving command injection on a web server running as a user named joe will execute commands under this joe user - and therefore obtain any permissions that joe has.

Command injection is also often known as “Remote Code Execution” (RCE) because it allows an attacker to execute code remotely within an application. These vulnerabilities are often the most lucrative to an attacker because they allow the attacker to interact directly with the vulnerable system. For example, an attacker may read system or user files, data, and other similar items.

For example, being able to abuse an application to perform the command whoami to list what user account the application is running will be an example of command injection.
