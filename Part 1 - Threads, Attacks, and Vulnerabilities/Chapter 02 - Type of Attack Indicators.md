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

## Potentially Unwanted Programs (PUPs)  
* These are programs that may have adverse effects on a computer's security or privacy.  
* Frequently PUPs involve adware or spyware components and are uses for revenue generarion purposes.  

🟢 **Viruses**  
A type of malware that, when executed, replicates itself by modifying other computer programs and inserting its own code into those programs.  
The nature of a virus implies that it reproduces by itself without user interaction but it is dependant on other software to attach and spread.  
