# CompTIA SY0-501 Security+ Study Notes

## Part 1 - Threads, Attacks, and Vulnerabilities  
### Chapter 04 - Network Attack Indicators 

## **Wireless** 

🟢 **Evil Twin**  

The main directive is to get victims to connect to the attacker's network instead of the victim's network by using the attacker's "cloned" access point (this is the evil twin) instead of a legitimate access point, the evil twins are usually enhanced with high-power and high-gain antennas to look like a better connection.  
Once the attacker clones a legitimate AP, attacker makes thar AP (the evil twin) visible to others in an attempt to trick people associating with it.  
Usually an evil twin is visible to the victims at the same time that a DoS attack is taking place to force users to disconnect from their legitimate network and use the evil twin instead.  

🟢 **Rouge Access Point**  

It is an ilegitimate AP (Access Point) that is physically plugged to a network to create a bypass from the outsite into a ligitimate network, typically used to perform MITM attacks to redirect the traffic from the victim's device to the network router but passing through the rouge access point.   
A rouge point, being ilegitimate is not administered by the network owner.  
As the AP is already part of a network, the attacker does not need to make it visible or advertise it in any way.  

🟢 **Bluejacking**  

Is an attack to bluetooth wireless technology where the thread actor sends unsolicited messages over Bluetooth to Bluetooth-enabled devices such as mobile phones, PDAs or laptop computers.  
Bluejacking is usually not very harmful, except that bluejacked people generally don't know what has happened, and so may think that their phone is malfunctioning. Usually, a bluejacker will only send a text message, but with modern phones it's possible to send images or sounds as well.  
The victim's devuce must also have bluetooth enabled and must be in discoverable mode.  

🟢 **Bluesnarfing**  
The unauthorized access of information from a wireless device through a Bluetooth connection, often between phones, desktops, laptops, and PDAs (personal digital assistant), devices do not necessarily need to be paired for bluesnarfing to work.  
This allows access to calendars, contact lists, emails and text messages, and on some phones, users can copy pictures and private videos. Both Bluesnarfing and Bluejacking exploit others' Bluetooth connections without their knowledge. 
Bluesnarfing is the theft of information from the target device.  

🟢 **Disassociation**  

A type of DoS attack in which the attacker breaks the wireless connection between the victim device and the access point.  
The method is based on the use of a special disassociation frame specified under IEEE 802.11. Transferring such a frame to the target device breaks the connection, and the Wi-Fi protocol does not require any encryption for it. For a successful attack, the cybercriminal needs to know only the victim’s MAC address.  
Asually, when the disassociation attack is successful, and the victim's device attempts to reconnect to the router, it'll be connecting to an evil twin router the attacker has set up for that purpose.  

🟢 **Jamming**  

Is a form of DoS (Denial of Service) that specifically targets the radio spectrum aspect of a wireless.  
This method involves the use of a device to intentionally create interfering radio signals to effectively “jam” the airwaves, resulting in the AP and any client devices connection being disrupted.  

🟢 **Radio Frequency Identification (RFID)**  

RFID tags come in several different forms and can be classified as either active or passive. Active tags have a power source, while passive tags utilize the RF energy transmitted to them for power.  
Several different attack types can be performed agains RFID systems:
* Against RFID devices themselves (the chips and readers)  
* Against the communication channel between the device and the reader
* Agains the reader and back-end system  
* 
The main attacks agains RFID are replay, skimming, eavesdropping and MITM.  

* In a **replay attack**, the RFID information is recorded and then replayed later.  
* In an **eavesdropping attack**, an attacker intercepts the communication between a tag that is authenticating with a reader, using a separate eavesdropping antenna. An eavesdropping attack is passive, meaning that the attacker's antenna only listens in on the communicationt, this has to happen in the vicinity of an authorized reader when the authentication is conducted.  
* In a **skimming attack**, an attacker secretly activates a tag and communicates with it. A skimming attack is active, meaning the antenna has to generate a field to power the tag. This limits the maximum distance for a skimming attack compared to an eavesdropping attack.  
A skimming attack can be used as part of a relay attack, where the information from the victim's the tag can be relayed to a genuine terminal.  
* **Man-in-the-middle RFID attack** is where the hacker listens for communication between an RFID tag and reader and then intercepts and manipulates the information. The attacker diverts the original signal and then sends false data while pretending to be a normal component in the RFID system.  

🟢 **Near Field Communication (NFC)**  

NFC is a subset of RFID and acts over a much shorter distance.  
NFC enables smartphones and other devices to establish radio communication over a distance of typically 10cm or less and this has become the mainstream method of making payments via mobile phones.  
In the attack scenario the attacker holds the NFC reader near the victim's card and relays the data over another communication channel to a second NFC reader placed in proximity to the original reader that will emulate the victim's card.  

🟢 **Initialization Vector (IV)**  

One method to encrypt data is to add a initialization vector (or IV) to the data that is up to be encrypted, this adds extra randomization to the final ciphertext. Then, on the second block of data, we use the resulting ciphertext as the IV for the next block, and so on.  
Because WEP uses 24-bit IVs, which is quite small, IVs ended up being re-used with the same key. Because IV keys are transferred with the data in plaintext so that the receiving party is able to decrypt the communication, an attacker can capture these IVs.  
By capturing enough repeating IVs, an attacker can easily crack the WEP secret key. This is one of the many reasons that WEP was deprecated and replaced with much more secure wireless protocols (WPA2 and WPA3).  

## **On-path Attacks** 

🟢 **Man in the Middle Attack (MITM)**  

Occurs when an attacker is able to place himself in the middle of two other hosts that are communicating, either to eavesdrop or to impersonate one of the parties.  
This is done by ensuring that all communocations going to or from the target host is routed through the attacker's host.  
The attacker can then observe all traffic before relaying it and can actually modify or block traffic.  
To the target host, it appears that communication is occurring normally since all expected replies are received.  
The amount of information that can be obtained in a man in the middle attack will be limited if the communication is encrypted.  

🟢 **Man in the Browser (MITB)**  

This is a variant of MITM attack where the attacker installs malware, generally a trojan horse on the victim's computer that is capable of modifying that victim's web transactions.  
The purpose of a man-in-the-browser attack includes eavesdropping, data theft or session tampering.  
The malware can tamper the browser behaviour through browser helper objects, plugins or extensions.  

## **Layer 2 Attacks**  

Layer 2 of a network is where local addressing decisions are made (Data link layer).  
Switches operate at layer 2 using media access control (MAC) addresses.  
The data link layer is concerned with local delivery of frames between nodes on the same level of the network. Data-link frames, as these protocol data units are called, do not cross the boundaries of a local area network.  

🟢 **Address Resolution Protocol (ARP) Poisoning/Spoofing**  

ARP helps devices to know where to send a packet using the MAC or layer 2 address, such ARP table is stored in the RAM of the device. Each entry, or row, of the ARP table binds an IP address with a MAC address.  
The ARP protocol uses four basic message types:
* **ARP Request**: "Who has this IP address?"
* **ARP Reply**: "I have that IP address; my MAC address is..."
* **Reverse ARP request (RARP)**: "Who has this MAC address?"
* **RARP reply**: "I have that MAC address; my IP is..."

The messages are used in conjunction with device's ARP table, where a form of short-term memory associated with these data elements reside.  
When an ARP reply is received, the data is entered into all devices that hear the reply to facilitate the address lookup process.  

There's no mechanism to verify the veracity of the data received, hence, an attacker could send falsified ARP messages over a local area network (LAN) to link the attacker's MAC address with the IP address of a legitimate computer or server on the network, this will corrupt the ARP table and cause packets to be misrouted, this will result in malicious address redirection that the attacker could exploit to inject himself into the middle of a conversation between 2 devices (MITM).   

🟢 **Media Access Control (MAC) Flooding**  

Addressing at the layer 2 interface is done by media access control (MAC) addresses using switches and hubs.  
Mac flooding is an attack to the network switches where the thread actor floods these devices with fake MAC addresses to compromise their security, when the MAC table reaches the allocated storage limit, it begins removing old addresses with the new ones which makes the switch unable to find the correct address for a packet and it will lead the switch to enter into a fail-open mode where the switch will now behave as a network hub.  

Once the first part of the attack is completed and the switch is acting as a hub, it will forward the incoming data to all ports (broadcasting), as the attacker is a part of the network, the attacker will also get the data packets intended for the victim machine. The attacker will now be able to steal sensitive data from the communication of the victim and other computers.  


## **Layer 2 Attacks** 
