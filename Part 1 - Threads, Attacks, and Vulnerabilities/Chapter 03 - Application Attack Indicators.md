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
  * **Non-persistent XSS attack**: The injected script is not persisted or stored but rather is immediately executed and passed back via the web server.
  * **Persisten XSS attack**: The script is permanently stored on the web server or some back-end storage, this allows the script to be used against others who access the system.
  * **DOM-based XSS attack**: The script is executed in the browser via the Document Object Model (DOM) process as opposed to the web server.

Common uses:
  * Theft of authentication information from a web application
  * Session hijacking
  * Deploying hostile content
  * Changing user settings, including feature users
  * Impersonating a user
  * Phishing or stealing sensitive information  

## **Injection Attacks**  

This happens when untrusted (unvalidated) inputs or unauthorized code are “injected” into an application and interpreted as part of a query or command. The result is an alteration of the software, redirecting it for a nefarious purpose.

🟢 **SQL Injection**  (Structured Query Language)  

Is a form of code injection aimed at any SQL-based database. 
An example of this attack is where the function takes the user-provided inputs for username and password and substitutes them in a **where** clause of a SQL statement with the express purpose of changing the **where** clause into one that gives a false answer to the query.  
The addition of **or** clauses, with an **always true** statement and the beginning of a comment line to block the trialing single quptes, alters the SQL statement to one in which the **where** clause is rendered inoperable, this might lead to a data breach if the **where** clause is altered to return records.  

Stored procedures are precompiled methods implemented within the database engine and act as a secure coding mechanism to isolate user input from the actual SQL statements being executed, this is one way to defend agains SQL injection.  

🟢 **DLL Injection**  (Dynamic-Link-Library)  

A DLL is a piece of code that can add functionality to a program through the inclusion of library routines linked at runtime.  
DLL injection is the process of adding to a program a DLL that has a specific functon vulnerability that can be capitalized upon by the attacker.  

🟢 **LDAP Injection**  (Lightweight Directory Access Protocol)  

LDAP injection can be used to execute arbritrary commands in a directory system when an application constructs an LDAP request based on user input.  
This technique is used to exploit web applications which could reveal sensitive user information or modify information stored in the LDAP directory.  

🟢 **XML Injection**  (Extensible Markup Language)  

XML injections can be used to manipulate an XML-based system and can cause the system configuration, changes in data streams, changes in outputs, etc.  
This occurs when user-supplied input isn't validated or sanitized before it is added to a web application's XML documents; then they are processed and executed.  

##

🟢 **Pointer/Object Dereference**  

Used to access or manipulate data contained in memory location pointed to by a pointer. Asterisk symbol is used with pointer variable when dereferencing the pointer variable, it refers to variable being pointed, so this is called dereferencing of pointers.
The act of getting the value at the memory location denoted by a pointer variable is known as *dereferencing*.  
Mistakes in the input validation can lead to errors in the pointer dereference, which may or may not trigger an error, as the location will contain data and it will be returned, dereferencing the pointer causes a dereferenced on the object.  

🟢 **Directory Traversal**  

When an attacker uses special inputs to circumvent the directory tree structure of the filesystem.  
Adding encoded symbols for "../.." in an invalidated input box can result in the program executing commands in a different location than designed.  
When combined with a command injection, the input can result in the execution of code in an unauthorized manner.  

🟢 **Buffer Overflow**  

This occurs when the input buffer that is used to hold program input is overwritten with data that is larger than the buffer can hold. This happens by taking advantage of input routines that do not validate the lenght of the inputs.  
Buffer overflows inlude many variants such as static buffer overruns, indexing errors, format string bugs, unicode and ANSI buffer size mismatches, and heap overruns.  
Buffer overflows can occur in any code, and code that runs with privilege has an even greater risk profile.  

🟢 **Race Condition**  

Also called Time of Check to Time of Use, or TOCTTOU attacks, take advantage of the need that programs have to execute some tasks in a specific sequence. In any such sequence, there is a small period of time when the system has carried out the first task but not started on the second. If this period is long enough or the attacker is lucky and knowledgeable, a race condition vulnerability exists where an attacker can trick the system into carrying out unauthorized actions in addition to its normal processes.
There are two main ways this attack is carried out:
   * **Interference by an untrusted process**: The attacker inserts a piece of code in between the steps of a secure process.
   * **Interference by a trusted process**: The attacker exploits two different processes that share some state in common.

🟢 **Race Condition**  

Also called Time of Check to Time of Use, or TOCTTOU attacks, take advantage of the need that programs have to execute some tasks in a specific sequence. In any such sequence, there is a

