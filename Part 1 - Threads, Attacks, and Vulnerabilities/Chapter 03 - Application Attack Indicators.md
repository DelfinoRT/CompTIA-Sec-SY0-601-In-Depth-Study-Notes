# CompTIA SY0-501 Security+ Study Notes

## Part 1 - Threads, Attacks, and Vulnerabilities  
### Chapter 03 - Application Attack Indicators 


🟢 **Privilege Escalation**  

Most attacks begin at a privilege level associated with an ordinary user. From this level, the attacker exploits vulnerabilities that enable them to achive root or admin level access. This step is called privilege escalation.  
The act of exploiting a bug, a design flaw, or a configuration oversight in an operating system or software application to gain elevated access to resources that are normally protected from an application or user.  
A method to limit the attack surface of this attack is to reduce the processes and services that run in elevated mode.  

🟢 **Cross-Site Scripting (XSS)**  

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

**Input validation** is especially well suited for many vulnerabilities including: buffer overflow, XSS, XSRF, path traversal, and some more.

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
Race conditions can be used for privilege elevation and denial of servive attacks.  
Developers can use reference counters, kernel locks, and thread synchronization to prevent race conditions.  
There are two main ways this attack is carried out:
   * **Interference by an untrusted process**: The attacker inserts a piece of code in between the steps of a secure process.
   * **Interference by a trusted process**: The attacker exploits two different processes that share some state in common.

🟢 **Improper Error Handling**  

During an exception, it is common practice to record/report the condition, typically in a log file, including supporting information such as the data that resulted in the error, data structures, data elements, sensitive information such as filenames, paths and server names. If attackers manage to capture this logs due to improper error handling, they can use this information for develop further attacks.  
The best method to defend agains this is to captire the errors/exceptions in a log file were it can be secured by an access control list (ACL).  
The worst methid is to echo the information to the user.  

🟢 **Improper Input Handling**  

During an exception, it is common practice to record/report the condition, typically in a log file, including supporting information such as the data that resulted in the error, data structures, data elements, sensitive information such as filenames, paths and server names. If attackers manage to capture this logs due to improper error handling, they can use this information for develop further attacks.  
The best method to defend agains this is to captire the errors/exceptions in a log file were it can be secured by an access control list (ACL).  
The worst methid is to echo the information to the user.  

🟢 **Reply Attacks**  

A replay attack is a form of Man-in-the-Middle (MITM) attack against applications in which valid data transmission is captured and maliciously or fraudulently repeated or delayed, what was valid before may well be valid again. 

🟢 **Session Replay**  

When a user connects to a system via the web, the connection forms a "session" that keeps record of the interaction and the various elements that are transmitted back and forth from client-server interaction.  
A session replay event is the re-creation of the interaction after it has occurred. 

🟢 **Integer Overflow**  

A programming error conditon that occurs when a program attempts to store a numeric value, which is an integer, in a variable that is too small to hold it.  
This can create significant logic errors in a program.  

## **Request Forgery**  

A class of attacks where a user performs a state-changing action on behalf of another user, typically without their knowledge.  
These attacks explit the caracteristics of web-based protocols and browsers.  

🟢 **Server Side Request Forgery (SSRF)**  

An exploit where an attacker abuses the functionality of a server causing it to access or manipulate information in the realm of that server that would otherwise not be directly accessible to the attacker.  
Common attacks include having the server attack itself or attack another server in the organization.  
The attacker targets an application that supports data imports from URLs or allows them to read data from URLs. URLs can be manipulated, either by replacing them with new ones or by tampering with URL path traversal.

🟢 **Cross-Site Request Forgery (SCRF)** (XSRF, “Sea Surf”, Session Riding, Cross-Site Reference Forgery, and Hostile Linking)  

An attack that forces an end user to execute unwanted actions on a web application in which they’re currently authenticated.  
For most sites, browser requests automatically include any credentials associated with the site, such as the user’s session cookie, IP address, Windows domain credentials, and so forth. Therefore, if the user is currently authenticated to the site, the site will have no way to distinguish between the forged request sent by the victim and a legitimate request sent by the victim.  
A successful CSRF attack can force the user to perform state changing requests like transferring funds, changing their email address, and so forth. If the victim is an administrative account, CSRF can compromise the entire web application.

🟢 **API Attacks** (Application Programming Interface)  

An attack where the attacker specifically attacks the API and the service behind it by manipulating inputs.  
An API attack can result in mass data losses, stolen private information and service disruption.  
API security vulnerabilities include poor authentication and no data encryption.  

🟢 **Resource Exhaustion**

Reource exhaustion is the state where a system does not have all of the resources it needs to continue to function (memory, bandwith, storage, etc.).  
These types of attacks aim to deplete the system resources and when one of these resources becomes exhausted, an operational failure can ensure and systen could crash.  

🟢 **Memory Leak**

Errors in memory management can result in a memory leak, which can grow over time, consuming more and more resources.  
This commonly occurs when there is no garbage collection routine in the program or it is failing to work properly.  

🟢 **SSL Stripping** (Secure Sockets Layer)

This is a Man-in-the-Middle (MITM) attack agains all SSL and early versions of TLS connections.  
The attack is performed anywhere a MIM can happen, which makes wireless hotspots a prime location.  
The attack works by intercepting the initial connection requests for HTTPS, redirecting it to an HTTP site and then mediating in the middle (Stripping away the encryption offered by HTTPS).

🟢 **Driver Manipulation**  

Is an attack on a system by changing drivers code, thus changing the behaviour of the system it is installed to.  
Drivers sit between the hardware and the operating system itself, thisus a great place to put a piece of malicious software.  

🟢 **Shimming**  

Application shimming is a Windows Application Compatibility framework that Windows created to allow programs to run on versions of the OS that they were not initially created to run on.
Shimmng is the process of addig malware to the Windows Application Compatibility framework, allowing attackers to intercept an API and change the arguments passed, redirect the operation or handle the data in some other way, thus bypassing system's security measures.   

🟢 **Refactoring**  

This refers to the process of restructuting existing computer code without changing its external behaviour.  
Refactoring can uncover design flaws that lead to exploitable vulnerabilities in which an attacker can add functionallity to a driver yet mantaining its desired operation.  

🟢 **Pass the Hash**  

A technique that allows an attacker to authenticate to a remote server or service by using the underlying hash of a user's password, instead of requiring the associated plaintext password as is normally the case. It replaces the need for stealing the plaintext password to gain access with stealing the hash.  
he attacker captures the hash used to authenticate a process then injecting that captured hash into a process in place of the actual password.  
The attack exploits an implementation weakness in the authentication protocol, where password hashes remain static from session to session until the password is next changed.  
