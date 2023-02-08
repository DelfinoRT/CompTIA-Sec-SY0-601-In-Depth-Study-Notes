# CompTIA SY0-501 Security+ Study Notes

## Part 1 - Threads, Attacks, and Vulnerabilities  
### Chapter 02 - Type of Attack Indicators 
* Each type of attack threatens at least one of the three security requirements: Confidentiality, Integrity, and Availability (the CIA of security).  
* Attacks on computer systems and networks can be grouped into two broad categories: attacks on specific software (applications or operating systems), and attacks on specific protocols or services.  

## **Malware**
* Refers to software that has been designed to cause damage to a system or to create a backdoor into the system to grant access to unauthorized individuals.
* The installation of malware is done so that it is not obvious to authorized users.  

🟢 **Ransomware**  
This type of malware typically encrypts files on a system and then leaves them unusable either permanently (acting as a denial of service) or temporarily until a ransom is paid.  
Ransom is typically a worm, completely automated, and can be spread through a phishing email or unknowingly infected website.  

🟢 **Trojan**  
A piece of software that appears to do one thing (and in fact can actually do that thing) but hides some other functionality that generally generates a negative impact for the host system.  
A trojan is a standalone program that must be copied and installed by the user in order to work, this means that usually the trojan is disguised as something that the user would want to run.  
Many trojans communicate with the outside through a port that the trojan opens, and this is one of the ways trojans can be detected.  

🟢 **Virus**  
A type of malware that, when executed, replicates itself by modifying other computer programs and inserting its own code into those programs.  
The nature of a virus implies that it reproduces by itself without user interaction but it relies on other software to attach and spread.  
Once a system is "infected", the virus is capable of causing a detrimental effect, such as corrupting the system, destroying data, exploiting operating system vulnerabilities, consuming bandwidth, overloading web servers, etc.  

🟢 **Worm**  
Pieces of code that attempt to penetrate networks and computer systems.  
Once penetration occurs, the worm will create a new copy of itself on the penetrated system.  
The reproduction of a worm does not rely on the attachment of its code to another piece of software or to a file.  
A worm usually has the same impact as a virus.  

* The important distinction is whether the code has to attach itself to something else (**virus**) or if it can "survive" on its own (**worm**).  

🟢 **Potentially Unwanted Programs (PUPs)** 
These are a form of malware that may have adverse effects on a computer's security or privacy.  
Frequently PUPs involve adware or spyware components and are used for revenue generation purposes.  
Some of the undesired characteristics caused by PUPs are: Slowing down the computer, displaying a ton of annoying ads, adding toolbars and stealing space on the browser, and collecting private information.  

🟢 **Fileless Viruses**  
A piece of malware that operates only in memory, never touching the filesystem, this makes it much harder to detect.  
Also known as a memory-based malware attack.  
Fileless viruses continue to run until the device is powered down.  

🟢 **Command and Control**  
This refers to a server program used by hackers to control malware that has been launched against targets.  
The attacker manages multiple malware elements on multiple systems under various IDs from the command and control server.  

🟢 **Bots**  
A piece of software that performs specific actions as a part of a larger entity, the entire assembly is called a botnet.  
A series of bots are controlled across the network in a group by using command and control servers.  

🟢 **Crypto-malware**  
A program that installs without the user being aware of it and designed to use system resources to mine cryptocurrency.  
This is a theft-of-services attack where the threat actor is using the CPU cycles of someone else's computer to do crypto mining.  

🟢 **Logic Bombs**  
A type of malware that is deliberately installed, generally by an authorized user, and sits dormant for a period of time until some event or date invokes its malicious payload.  
Logic bombs are difficult to detect because they are often installed by authorized users or administrators from a system.  

🟢 **Spyware**  
Software that "spies" on users, recording and reporting on their activities without the user's knowledge.  
Specifically designed to steal information.  

🟢 **Adware**  
A form of malware that hides on devices and serves advertisements.  
Some adware also monitors user behavior online so it can target specific ads.  
This software generates revenue for its developer by automatically generating online advertisements in the user interface.  

🟢 **Keylogger**  
Software that logs all of the keystrokes that a user enters on the infected machine.  

🟢 **Remote-Access Trojan (RAT)**  
A toolkit designed to provide the capability of hiding a surveillance process on a device or gaining unauthorized access to a system.  
A RAT employs malware to infect a system and has an operator behind it guiding it to cause persistent damage (Remotely operated trojan).  
RATs typically involve the creation of hidden file structures on a system.  

🟢 **Rootkit**  
A type of malware designed to modify the operation of the operating system to facilitate nonstandard functionality.  
A rootkit can do virtually anything on the infected operating system as it can modify the kernel and support functions to avoid detection and alter the security functions of the operating system.  
Allows the threat actor to maintain command and control over a computer through a backdoor.
Five types/levels of rootkit exist: Firmware, Virtual, Kernel, Library, and application level.

🟢 **Backdoor**  
Programs installed after attackers gain unauthorized access to a system to ensure that they can continue to have unrestricted access to it.  

## **Password Attacks**

🟢 **Spraying**  
An attack that uses a limited number of commonly used passwords and applies them to a large number of accounts.  

🟢 **Dictionary**  

A password-cracking method that employs programs with a list of dictionary words to try to guess the password.  
The password can be used by themselves, or two or more smaller words can be combined to form a single possible password.  
These programs often permit the attacker to create rules that tell the program how to combine words or substitute special characters for other characters.  

🟢 **Brute Force**  

A method where the program used attempts all possible password combinations including those not found in a dictionary.  
The length of the password and the size of the set of possible characters in the password will greatly affect the time a brute force attack will take.  
This type of attack can take place at two levels: it can attack a system to guess the password at a login prompt or it can attack password files and the password hashes contained on them.

* Offline: Perform hash comparisons against a stolen password file, often high-performance GPU-based parallel machines are used at very high rates and against multiple accounts at the same time.  
* Online: When the brute force attack occurs in real-time against a system, it is frequently being done to attack a single account with multiple sets of passwords.  

🟢 **Rainbow Tables**  

Are precomputed hash values associated with passwords, this changes the search for a password from a computational problem to a lookup problem.  
Large pre-generated data sets of encrypted passwords are used in password attacks.  
The best defense against rainbow tables is salted hashes (a random set of characters designed to increase the length of the item being hashed).

🟢 **Plaintext/Unencrypted**  

A type of attack where the threat actor has both the plaintext and its encrypted version.  
The goal is to guess the secret key (or a number of secret keys) or to develop an algorithm that would allow to decryption of the password.  

## **Physical Attacks**

🟢 **Malicious USB Cable**  

A USB cable can have embedded electronics that could deliver malware to machines.

🟢 **Malicious Flash Drives**  

Infected USB devices for people to pick up and use on their systems, the attack is automate once the victims make use of these devices.

🟢 **Card Cloning**  

During the attack, the information is copied from the magnetic strip on the card, enabling the attacker to make a clone of it.  
In contactless cards (NFC), the chip is read, information copied and then the clone is implemented.  

🟢 **Skimming**  

This attack relies on physical devices built to intercept a credit card and are placed on card readers to skim the data while passing to the legitimate reader behind the skimming device.  
Skimmers can collect all the information from the magnetic strip as well as the PIN being entered.  

## Adversarial AI (Artificial Intelligence)
Attackers can use AI-enabled tools to improve their attacks, generally to avoid machine detection or to increase computation capabilities.

🟢 **Tainted Training Data for Machine Learning (ML)** 

Works by using a training data set to calibrate the detection model to enable the detection of sample data.  
The ability of the model to detect threats is a direct relation to the efficacy and quality of the training data set.  
The ML algorithm needs persistent retraining or updating to make it effective against differing inputs.  

## **Supply-Chain Attacks**
In the case of a computer, the supply chain provides the parts or devices that make the computer or system work.  
In the case of a program, the programmers are one part, but the libraries they use are another.   
The parts that are used can be tainted, either by accident or on purpose this would cause the final product to have vulnerabilities.  

## **Cloud-Based vs On-Premise Attacks**  
Attacks against data can happen whether the system is in-house (on-premise) or in the cloud (cloud-based).  
Using cloud computing to improve security only works if the cloud vendor offers security solutions as part of the package.  

## **Cryptographic Attacks**  
These are attacks against the cryptographic system/algorithm itself.  
The attacks are designed to take advantage of two specific weaknesses:
* First, the users generally view cryptography as incomprehensible stuff, leading to trust the results without any more reasons.  
* Second, Frequently happens that developers overlook algorithm weaknesses so no further work to improve it or fix it is done.  

🟢 **Birthday Attack**  

A brute force attack that got its name from the birthday paradox which states that in a group of at least 23 people, the chance that two individuals will have the same birthday is greater than 50%.  
The success of this attack largely depends upon the higher likelihood of collisions found between random attack attempts and a fixed degree of permutations.  
The birthday attack is used to create hash collisions and find a specific input with a hash that collides with another input.  

🟢 **Collision**  

This is where 2 different inputs yield the same output of a hash function.  
Through the manipulation of data, subtle changes are made to create different versions of a digital file.   
By creating many different versions of the file and using a birthday attack to find a collision between the versions, the attacker could create a file with visible changed content but identical hashes.

🟢 **Downgrade**  

This attack method takes advantage of the commonly employed principle to support backward compatibility and to downgrade the security system to a lower or nonexistent state.  


