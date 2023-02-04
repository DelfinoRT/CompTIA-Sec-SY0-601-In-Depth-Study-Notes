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
The main attacks agains RFID are replay, skimming, eavesdropping, MITM.  
* In a replay attack, the RFID information is recorded and then replayed later.  
* In an eavesdropping attack, an attacker intercepts the communication between a tag that is authenticating with a reader, using a separate eavesdropping antenna. An eavesdropping attack is passive, meaning that the attacker's antenna only listens in on the communicationt, this has to happen in the vicinity of an authorized reader when the authentication is conducted.  
* In a skimming attack, an attacker secretly activates a tag and communicates with it. A skimming attack is active, meaning the antenna has to generate a field to power the tag. This limits the maximum distance for a skimming attack compared to an eavesdropping attack.  
A skimming attack can be used as part of a relay attack, where the information from the victim's the tag can be relayed to a genuine terminal.  
* Man-in-the-middle RFID attack is where the hacker listens for communication between an RFID tag and reader and then intercepts and manipulates the information. The attacker diverts the original signal and then sends false data while pretending to be a normal component in the RFID system.  

🟢 **Near Field Communication (NFC)**  

Is a form of DoS (Denial of Service) that specifically targets the radio spectrum aspect of a wireless.  
This method involves the use of a device to intentionally create interfering radio signals to effectively “jam” the airwaves, resulting in the AP and any client devices connection being disrupted.  
