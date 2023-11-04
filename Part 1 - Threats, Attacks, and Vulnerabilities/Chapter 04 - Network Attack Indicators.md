# CompTIA SY0-501 Security+ Study Notes

## Part 1 - Threats, Attacks, and Vulnerabilities  
### Chapter 04 - Network Attack Indicators

## **Wireless**

🟢 **Evil Twin**  

An **Evil Twin** attack involves the attacker creating a **"cloned" access point (AP)**, tricking victims into connecting to it instead of their legit network. The malicious AP, often powered by high-gain antennas, appears more attractive. This attack usually coincides with a DoS attack, forcing users to disconnect from their network and connect to the evil twin.

🟢 **Rouge Access Point**  

A **Rogue Access Point (AP)** is an illegitimate AP connected into a network, creating a bypass into the legit network. It's typically used for MITM attacks, redirecting traffic from the victim's device to the network router via the rogue AP.<br>
The network owner does not administer the rogue AP and as the AP is already part of a network, the attacker does not need to make it visible or advertise it in any way.

🟢 **Bluejacking**  

**Bluejacking** is an attack where an actor sends unsolicited messages over Bluetooth to Bluetooth-enabled devices. While typically not harmful, victims often misunderstand the situation, assuming their device is malfunctioning. The attack can include sending text messages, images, or sounds.<br>
The victim's device must also have Bluetooth enabled and must be in discoverable mode.

🟢 **Bluesnarfing**

**Bluesnarfing** is the unauthorized access of information from a wireless device through a Bluetooth connection, devices do not necessarily need to be paired for bluesnarfing to work.<br>
The attacker can access calendars, contact lists, emails, text messages, pictures, and private videos without the device owners' knowledge.<br>
The goal of Bluesnarfing is the theft of information from the target device.

🟢 **Disassociation**  

A disassociation attack is **a type of DoS attack** where the attacker breaks the wireless connection between the victim device and the access point using a special disassociation frame specified under **IEEE 802.11**. After a successful attack, the victim's device may connect to an evil twin router set up by the attacker.

🟢 **Jamming**  

In a jamming attack, malicious nodes block legitimate communication by causing intentional interference in wireless networks. The attacker uses a device to create interfering radio signals, disrupting the connection between the AP and any client devices.

🟢 **Radio Frequency Identification (RFID)**  

RFID tags come in several different forms and can be classified as either active or passive. Active tags have a power source, while passive tags utilize the RF energy transmitted to them for power.  
Several different attack types can be performed against RFID systems:
* Against RFID devices themselves (the chips and readers)  
* Against the communication channel between the device and the reader
* Against the reader and back-end system  
*
The main attacks against RFID are replay, skimming, eavesdropping and MITM.  

* In a **replay attack**, the RFID information is recorded and then replayed later.  
* In an **eavesdropping attack**, an attacker intercepts the communication between a tag that is authenticating with a reader, using a separate eavesdropping antenna. An eavesdropping attack is passive, meaning that the attacker's antenna only listens in on the communications, this has to happen in the vicinity of an authorized reader when the authentication is conducted.  
* In a **skimming attack**, an attacker secretly activates a tag and communicates with it. A skimming attack is active, meaning the antenna has to generate a field to power the tag. This limits the maximum distance for a skimming attack compared to an eavesdropping attack.  
A skimming attack can be used as part of a relay attack, where the information from the victim's tag can be relayed to a genuine terminal.  
* **Man-in-the-middle RFID attack** is where the hacker listens for communication between an RFID tag and reader and then intercepts and manipulates the information. The attacker diverts the original signal and then sends false data while pretending to be a normal component in the RFID system.  

🟢 **Near Field Communication (NFC)**  

NFC is a subset of RFID and acts over a shorter distance.<br>
It enables radio communication between devices over a typical distance of 10cm or less and is often used for mobile payments.<br>
In an attack scenario, an attacker can relay data from the victim's card to another reader to emulate the victim's card.

🟢 **Initialization Vector (IV)**  

An initialization vector (IV) adds randomization to the encrypted data. However, because WEP uses small 24-bit IVs, the keys ended up being reused with the same IV, making it easy for an attacker to crack the WEP secret key by capturing enough repeating IVs.<br>
This is one reason why WEP was replaced with more secure wireless protocols (WPA2 and WPA3).

## **On-path Attacks**

🟢 **Man in the Middle Attack (MITM)**  

Occurs when an attacker is able to place himself in the middle of two other hosts that are communicating, either to eavesdrop or to impersonate one of the parties.  
This is done by ensuring that all communications going to or from the target host are routed through the attacker's host.  
The attacker can then observe all traffic before relaying it and can actually modify or block traffic.  
To the target host, it appears that communication is occurring normally since all expected replies are received.  
The amount of information that can be obtained in a man-in-the-middle attack will be limited if the communication is encrypted.  

🟢 **Man in the Browser (MITB)**  

This is a variant of MITM attack where the attacker installs malware, generally a trojan horse on the victim's computer that is capable of modifying that victim's web transactions.  
The purpose of a man-in-the-browser attack includes eavesdropping, data theft, or session tampering.  
The malware can tamper the browser behavior through browser helper objects, plugins, or extensions.  

## **Layer 2 Attacks**  

Layer 2 of a network is where local addressing decisions are made (Data link layer).  
Switches operate at layer 2 using media access control (MAC) addresses.  
The data link layer is concerned with the local delivery of frames between nodes on the same level of the network. Data-link frames, as these protocol data units are called, do not cross the boundaries of a local area network.  

🟢 **Address Resolution Protocol (ARP) Poisoning/Spoofing**  

ARP helps devices to know where to send a packet using the MAC or layer 2 address, such ARP table is stored in the RAM of the device. Each entry (or row) of the ARP table, binds an IP address with a MAC address.  
The ARP protocol uses four basic message types:
* **ARP Request**: "Who has this IP address?"
* **ARP Reply**: "I have that IP address; my MAC address is..."
* **Reverse ARP request (RARP)**: "Who has this MAC address?"
* **RARP reply**: "I have that MAC address; my IP is..."

The messages are used in conjunction with the device's ARP table, where a form of short-term memory associated with these data elements resides.  
When an ARP reply is received, the data is entered into all devices that hear the reply to facilitate the address lookup process.  

There's no mechanism to verify the veracity of the data received, hence, an attacker could send falsified ARP messages over a local area network (LAN) to link the attacker's MAC address with the IP address of a legitimate computer or server on the network, this will corrupt the ARP table and cause packets to be misrouted, this will result in malicious address redirection that the attacker could exploit to inject himself into the middle of a conversation between 2 devices (MITM).   

🟢 **Media Access Control (MAC) Flooding**  

Addressing at the layer 2 interface is done by media access control (MAC) addresses using switches and hubs.  
Mac flooding is an attack on the network switches where the threat actor floods these devices with fake MAC addresses to compromise their security, when the MAC table reaches the allocated storage limit, it begins removing old addresses with the new ones which make the switch unable to find the correct address for a packet and it will lead the switch to enter into a fail-open mode where the switch will now behave as a network hub.  

Once the first part of the attack is completed and the switch is acting as a hub, it will forward the incoming data to all ports (broadcasting), as the attacker is a part of the network, the attacker will also get the data packets intended for the victim machine. The attacker will now be able to steal sensitive data from the communication of the victim and other computers.  

## **Domain Name System (DNS)**

🟢 **Domain Hijacking**  

Is the act of changing the registration of a domain name without the permission of its original registrant.  
Generally, this attack occurs from unauthorized access to, or exploitation of a vulnerability in a domain name registrar system, through social engineering, or by gaining access to the domain name owner's email address and then resetting the password to their domain name registrar.  

🟢 **DNS Poisoning/Spoofing**  

Is the act of entering false information into a DNS cache, so that DNS queries return an incorrect response and users are directed to the wrong websites.  
When poisoned, a DNS resolver cache will store faulty information, traffic will go to the wrong places until the cached information is corrected manually or until the time to live (TTL) expires.  
There's no single DNS resolver system but rather a hierarchy of DNS servers, from root servers on the backbone of the internet to copies at your ISP, your home router, and your local machine, each in the form of a DNS resolver cache.  
DNS is an unencrypted protocol, making it easy to intercept traffic with spoofing. A project has begun to secure DNS infrastructure using the digital signing of DNS records, it is called Domain Name System Security Extensions (DNSSEC).  

🟢 **Universal Resource Locator (URL) Redirection**  

This Is the use of a vulnerability that allows an attacker to force users to an external site which is usually a phishing site that impersonates a legitimate site and steals credentials from the victims.
The attack is most often performed by delivering a link to the victim, who then clicks the link and is unknowingly redirected to the malicious website.  

🟢 **DNS amplification**  

Is a Distributed Denial of Service (DDoS) attack in which the attacker exploits vulnerabilities in domain name system (DNS) servers to turn initially small queries into much larger payloads, which are used to bring down the victim’s servers.  

## **Distributed Denial-of-Service (DDoS)**  

In a DoS attack, the threat actor attempts to deny authorized users access either to specific information or to the computer system or network itself.  
This can be accomplished by crashing the system or by sending so many requests that the machine is overwhelmed.  
A DoS attack employing multiple attacking systems is known as a Distributed DoS.  
The creation of the attack network may be a multistep process in which the attacker first compromises a few systems that are then used as handlers or masters, which in turn compromise other systems. Once the network has been created, the agents (zombies) wait for an attack message that will include data on the specific target before launching the attack.  
A Defensive approach against DDoS involves changing the time-out option for TCP connections so that attacks such as the SYN flooding attack are more difficult to perform because unused connections are dropped more quickly.  

🟢 **Network**  

In this attack, service is denied by overwhelming the target with traffic from many different systems, the purpose of this attack is to prevent access to the target system, and blocking network connections will accomplish this.  
One method, a SYN flooding attack, can be used to prevent service to a system temporarily in order to take advantage of a trusted relationship that exists between that system and another. SYN flooding is an example of a DoS attack that takes advantage of the way TCP/IP networks were designed to function.  
The number of connections a system can support is finite, so when more requests come in that can be processed, the system will soon be reserving all its connections for fake requests. At this point, any further requests are simply dropped and legitimate users who want to connect to the target system will not be able to do so because the use of the system/service has been denied to them.  
Other common DoS methods are the POP (ping of death) and CLDAP (connectionless Lightweight directory access protocol) attacks.  

🟢 **Application**  

Applications are subject to DDoS as well, because, like all systems, they take user inputs, process the data and create user outputs.  This activity takes resources and the objective of an application-level DDoS is to consume all the resources to put the system into a failed state.  
One of the most common targets of an application layer attack is HTTP but these types of attacks work also against API interfaces.  

🟢 **Operational Technology (OT) DDoS attack**  

Operational Technology is the name given to networks of industrial devices, these devices use computers to control physical processes - from traffic lights to refineries, to manufacturing plants, and more.  
OT systems have OT-specific protocols that are used to perform the communications of equipment control.  
One of the system characteristics of these processes is the reliance on properly timed signals. These systems do not perform correctly when communications are interrupted, so DoS attacks of any kind, including DDoS, can result in significant problems.  
For these reasons and more, OT systems are not directly connected to the internet and have significant barriers preventing outside packets from getting into these networks.  

## **Malicious Code and Script Execution**  

Scripts and automation in systems promote speed, accuracy, reproducibility, and portability as well as offer a ton of other advantages.  
Many of these reasons are why attackers use them as well to code malicious software and script its automatic execution.  

🟢 **PowerShell**  

PowerShell is a command-line tool suite that is completely integrated with the Windows environment, allowing administrators to program virtually any function that can be done in the O.S.  
A wide range of toolsets built to leverage the power of PowerShell can be used to attack systems.  

🟢 **Python**  
Is an easy-to-learn programming/scripting language widely supported and good at automating tasks and data analysis. This makes Python very useful for cybersecurity teams and attackers alike.

🟢 **Bash (aka Bourne Again shell)**  

Is an interpreter that processes shell commands on Linux systems.  
Bash takes commands in plaintext format and calls OS services to perform the specified tasks. this enables complete automation of a Linux environment and is therefore valuable to system administrators and attackers alike.  
Threat actors use bash to search through the systems and perform tasks on Linux.  

🟢 **Macros (short for "macro instruction")**  

Macros are recorded sets of instructions, typically presented to an application to automate their function, with this functionality comes risk in the form of unwanted macros calling the system and performing system activities.  
Macros can be enabled in PDFs, Microsoft Office, and some other software applications.  

🟢 **Visual Basic for Applications (VBA)**  
VBA is an older technology from Microsoft that was used to automate many internal processes in applications and it is still valid on a lot of platforms and, as such, is still a vector for attackers.  
