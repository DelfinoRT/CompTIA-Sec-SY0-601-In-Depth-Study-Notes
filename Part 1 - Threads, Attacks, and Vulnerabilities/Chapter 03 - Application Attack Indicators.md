# CompTIA SY0-501 Security+ Study Notes

## Part 1 - Threads, Attacks, and Vulnerabilities  
### Chapter 03 - Application Attack Indicators 


🟢 **Privilege Escalation**  
Most attacks begin at a privilege level associated with an ordinary user. From this level, the attacker exploits vulnerabilities that enable them to achive root or admin level access. This step is called privilege escalation.  
The act of exploiting a bug, a design flaw, or a configuration oversight in an operating system or software application to gain elevated access to resources that are normally protected from an application or user.  
A method to limit the attack surface of this attack is to reduce the processes and services that run in elevated mode.  

🟢 **Cross-Site Scripting**  
This is one of the most common attack methodologies.   
The cause of the vulnerability is weak user input validation. If input is not validated properly, an attacker can include a script in the inputs and have it rendered as part of the web process.  
Input validation (data validation) is used to prevent XSS attacks.  
There are different types of XSS attacks:  
  * Non-persistent XSS attack: The injected script is not persisted or stored but rather is immediately executed and passed back via the web server.
  * Persisten XSS attack: The script is permanently stored on the web server or some back-end storage, this allows the script to be used against others who access the system.
  * DOM-based XSS attack: The script is executed in the browser via the Document Object Model (DOM) process as opposed to the web server.

Common uses:
  * Theft of authentication information from a web application
  * Session hijacking
  * Deploying hostile content
  * Changing user settings, including feature users
  * Impersonating a user
  * Phishing or stealing sensitive information  

🟢 **Injection Attacks**  
Most attacks begin at a privilege level associated with an ordinary user. From this level, the attacker exploits vulnerabilities that enable them to achive root or admin level access. This step is called privilege escalation.  
The act of exploiting a bug, a design flaw, or a configuration oversight in an operating system or software application to gain elevated access to resources that are normally protected from an application or user.  
A method to limit the attack surface of this attack is to reduce the processes and services that run in elevated mode.  
