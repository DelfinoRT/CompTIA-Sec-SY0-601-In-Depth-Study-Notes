# CompTIA SY0-501 Security+ Study Notes

## Part 1 - Threads, Attacks, and Vulnerabilities  
### Chapter 02 - Type of Attack Indicators 
* Each type of attack threatens at least one of the three security requirements: Confidentiality, Integrity, and Availability (the CIA of security).  
* Attacks on computer systems and networks can be grouped into two broad categories: attacks on specific software (applications or operating systems), and attacks on specific protocol or service.  

## Malware
* Refers to software that has been designed to cause damage to a system or to create a backdoor into the system to grant access to unauthorized individuals.
* The installation of malware is done so that it is not obvious to the authorized users.  

🟢 **Ransomware**  

This type of malwaare typically encrypt files on a system and then leaves them unusuable either permanently, acting as a denial of service, or temporarily until a ransom is paid.  
Ransom is typically a worm, completely automated and can be spread through a phishing email or unknowingly infected website.  

🟢 **Trojan**  
A piece of software that appears to do one thing (and in fact can actually do that thing) but hides some other functionality that generally generates a negative impact for the host system.  
A trojan is a standalone program that must be copied and installed by the user in order to work, this means that usually the trojan is disguised as something that the user would want to run.  
Many trojans communicate with the outside through a port that the trojan opens, and this is one of the ways trojans can be detected.  

🟢 **Virus**  
A type of malware that, when executed, replicates itself by modifying other computer programs and inserting its own code into those programs.  
The nature of a virus implies that it reproduces by itself without user interaction but it relies on other software to attach and spread.  
Once a system is "infected", the virus is capable causing a detrimental effect, such as corrupting the system, destroying data, exploiting operating system vulnerabilities, consuming bandwidth, overloading web servers, etc.  

🟢 **Worm**  
Pieces of code that attempt to penetrate networks and computer systems.  
Once a penetration occurs, the worm will create a new copy of itself on the penetrated system.  
Reproduction of a worm does not rely on the attachment of its code to another piece of software or to a file.  
A worm usually has the same impact as a virus.  

* The important distinction is whether the code has to attach itself to something else (**virus**) or if it can "survive" on its own (**worm**).  

🟢 **Potentially Unwanted Programs (PUPs)** 
These are a form of malware that may have adverse effects on a computer's security or privacy.  
Frequently PUPs involve adware or spyware components and are uses for revenue generarion purposes.  
Some of the undesired characteristics cause by PUPs are: Slowing down the computer, displaying a ton of annoying ads, adding toolbars and steal space on the browser, collecting private information.  

🟢 **Fileless Viruses**  
A piece of malware that operates only in memory, never touching the filesystem, this makes it much harder to detect.  
Also known as memory-based malware attack.  
Fileless viruses continue to run until the device is powered down.  

🟢 **Command and Control**  
This revers to a server program used by hackers to control malware that has been launched agains targets.  
The attacker manages multiple malware elements on multiple systems under various IDs from the command and control server.  

🟢 **Bots**  
A piece of software that performs specific actions as a part of a larger entity known as a botnet.  
A series of bots is controlled across the network in a group by using command and control servers, and the entire assembly is called a botnet.  

🟢 **Crypto-malware**  
A program that installs without the user being aware of it and designed to use system resources to mine cryptocurrency.  
This is a thef-of-services attack where the threat actor is using the CPU cycles of someone else's computer to do crypto mining.  

🟢 **Logic Bombs**  
A type of malware that is deliberately installed, generally by an authorized user and sits dormant for a period of time until some event or date invokes its malicious payload.  
Logic bombs are difficult to detect because they are often installed by authorized users or administrators from a system.  

🟢 **Spyware**  
Software that "spies" on users , recording and reporting on their activities without user's knowledge.  
Soecifically designed to steal information.  

🟢 **Keylogger**  
Software that logs all of the keystrokes that a user enters on the infected machine.  

🟢 **Remote-Access Trojan (RAT)**  
A toolkit designed to provide the capability of hide a surveillance process on a device or gain unauthorized access to a system.  
A RAT employs malware to infect a system and has an operator behind it and guiding it to cause persistent damage (Remotely operated trojan).  
RATs typically involve the creation of hidden file structures on a system.  

🟢 **Rootkit**  
A malware designed to modify the operation of the operating system to facilitate nonstandard functionality.  
A rootkit can do virtually anything on the infected operating system as it can modify the kernel and support functions to avoid detection and alter the security functions of the operating system.  
Allows the threat actor to maintain command and control over a computer through a backdoor.
Five types/levels of rootkit exist: Firmware, Virtual, Kernel, Library, and application level.

🟢 **Backdoor**  
Programs installed after attackers gaining unauthorized access to a system to ensure that they can continue to have unrestricted access to it.  

## Password Attacks

🟢 **Spraying**  
An attack that uses a limited number of commonly used passwords and applies them to a large number of accounts.  

🟢 **Dictionary**  
A password-cracking method that employs programs with a list of dictionary words to try to guess the password.  
The password can be used by themselves, or two or more smaller words can be combined to form a single possible password.  
These programs often permit the attacker to create rules that tell the program how to combine words or substite special characters for other characters.  

🟢 **Brute Force**  
A method where the program used attempts all possible password combinations including those not found on a dictionary.  
The length of the password and the size of the ser of possible characters in the password will greatly affect the time a brute force attack will take.  
This type of attack can take place at two levels: it can attack a system to guess the password at a login prompt or it can attack password files and the password hashes contained on them.

* Offline: Perform hash comparisons agains a stolen password file, oftenly high-performance GPU-based parallel machines are used at very high rates and against multiple accounts at the same time.  
* Online: When the brute force attack occurs in real time agains a system, it is frequently neing done to attack a single account with multiple sets of passwords.  

🟢 **Rainbow tables**  
Are precomputed hash values associated with passwords, this changes the search for a password from a computational problem to a lookup problem.  
Large pre-generated data sets of encrypted passwords used in password attacks.  
The best defense agains rainbow tables is salted hashes (a random set of characters designed to increase the lenght of the item being hashed).

🟢 **Plaintext/Unencrypted**  
A type of attack where the threat actor has both the plaintext and its encrypted version.  
The goal is to guess the secret key (or a number of secret keys) or to develop an algorithm which would allow to decrypttion if the password.  

## Physical Attacks

🟢 **Rainbow tables**  
A type of attack where the threat actor has both the plaintext and its encrypted version.
