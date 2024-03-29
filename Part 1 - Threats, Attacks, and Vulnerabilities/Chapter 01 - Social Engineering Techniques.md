# CompTIA SY0-501 Security+ Study Notes

## Part 1 - Threats, Attacks, and Vulnerabilities  

🟢 **What is a threat?**  

A threat in cybersecurity refers to any circumstance, event, or actor with the potential to adversely impact organizational operations, assets, or individuals through an information system. This can include unauthorized access, disclosure, modification, destruction of information, or denial of service. Threats can arise from various sources, such as accidental occurrences, environmental factors like natural disasters, human negligence, or deliberate actions by threat actors.
Cybersecurity threats encompass a range of malicious activities aimed at compromising computer systems and networks. These include malware like viruses and ransomware, phishing attacks that deceive users into revealing sensitive information, and denial-of-service assaults that overwhelm systems with traffic. Social engineering tactics manipulate individuals, while SQL injection and cross-site scripting target databases and websites. Zero-day exploits that exploit previously unknown vulnerabilities, and insider threats involve misuse of access within an organization. IoT vulnerabilities, cryptojacking, eavesdropping, and password attacks are also prevalent. Drive-by downloads install malware on unsuspecting users' devices, while credential theft and man-in-the-middle attacks exploit weaknesses in authentication.

🟢 **What is an attack?**  

An attack is an intentional and offensive action launched by cybercriminals or other threat actors to compromise a system, network, or asset. The primary objective of a cyber attack is to gain unauthorized access, disrupt, disable, alter, or steal data from targeted systems. Cyber attacks can take various forms, including the deployment of malware, phishing, ransomware, and denial of service, among other methods. Attackers typically follow a method and have a motive when seizing an opportunity to exploit vulnerabilities.

🟢 **What is a vulnerability**  

A vulnerability in an IT system refers to a weakness that can be exploited by an attacker to carry out a successful attack. Vulnerabilities can range from flaws in software or hardware to inherent features, or user errors. Attackers often seek to exploit these weaknesses, either individually or in combination with others, to achieve their objectives. These weaknesses can lead to security and privacy risks, potentially resulting in unauthorized access, data breaches, or other forms of compromise.
Well-known cyber and IT vulnerabilities encompass a range of weaknesses that can be exploited by attackers. These include outdated software and hardware, weak passwords, unsecured networks, and social engineering tactics. Misconfigured security settings, insufficient access controls, and unpatched software vulnerabilities also pose significant risks.
Other vulnerabilities stem from phishing attacks, lack of employee training, and inadequate malware protection. Additionally, physical security lapses, data leakage, and supply chain weaknesses can create avenues for unauthorized access.

### Chapter 01 - Social Engineering Techniques  
* Social engineering is a method of using people as part of an attack process.  
* The key in all social engineering attacks is that you are manipulating a person and their actions by manipulating their perception of a situation.  
* A social engineer preys on people's beliefs, biases, and stereotypes.  
* This is hacking the human side of a system, is an attack against the user, and involves some form of social interaction.
* The best defense against social engineering attacks is a comprehensive training and awareness program.  
* The tools to perform social engineering attacks are based on a knowledge of psychology and usually don't require a sophisticated knowledge of software or hardware.  

### Principles (Reasons for Effectiveness)  
Social engineering is very successful for two general reasons:  
* The first is the basic desire of most people to be helpful.  
The problem with this is that seemingly innocuous information can be used either directly in an attack or indirectly to build a bigger picture that an attacker can use to create an aura of authenticity during an attack.  
* The second reason is that individuals normally seek to avoid confrontation and trouble.  
Usually, the attacker attempts to intimidate the victim, threatening to call the victim's supervisor because of lack of help, the victim may give in and provide the information to avoid confrontation.

### Psychological Components of Social Engineering
* **Authority**: The actor acts as an individual of authority, this leads to an environment where one party feels at risk of challenging another.
* **Intimidation**: Frightening or threatening the victim, this uses communication that builds an expectation of superiority.
* **Consensus**: Convince based on what's normally expected, the attacker motivates others to achieve a desired outcome.
* **Scarcity**: Limited resources and time to act. If something is in short supply and is valued, arriving with what is needed can bring rewards and acceptance.
* **Familiarity**: The victim is well known. The sense of familiarity and appeal can lead to misplaced trust.
* **Trust**: Gain their confidence, and be their friend. Not forcing people to do things they would normally not do, lead the victims to feel they are doing the correct thing.
* **Urgency**: Limited time to act, rush the victim. Give a reason to believe that the victim could take advantage of a timely situation.

### Defenses
* Stopping social engineering begins with policies and procedures that eliminate the pathways used by the attacks.
* Visitor access rules, customer support guidelines, verifying requests for legitimacy.
* Employee training, frequent reminders, retraining programs, and awareness campaigns.
* Have multiple layers of defenses including approvals and authentication processes.

## **Social Engineering Techniques**

🟢 **Phishing**  

Is when an attacker attempts to obtain sensitive information (such as usernames, passwords, credit card numbers, and details about the user's bank accounts) from users by masquerading as a trusted entity in an e-mail or instant message sent to a large group of often random users.  
The message encourages the user to visit a website that appears to be for a reputable entity.   
The information gathered by the attacker is often used to steal the user's money, credentials, or identity.  
Phishing is the most common form of social engineering attack related to computer security.  

🟢 **Smishing**  

It is a version of phishing and the attack is performed using Short Message Service (SMS).  
The SMS usually directs the user to a website that can serve as a vector for different attack types including malware injection.  
This attack works primarily due to the use of urgency and intimidation in the message.  

🟢 **Vishing**  

It is another variation of phishing that uses voice communication to obtain information from the target.  
This technique takes advantage of the trust that some people place in the telephone network.  
We must be aware that attackers can spoof (simulate) calls from legitimate entities using VoIP technology.  

🟢 **Spam**  

Spam references to bulk unsolicited e-mail, this email can be malicious and could include attachments that contain malicious software designed to harm systems or link to malicious websites.  

🟢 **Spam over Instant Messaging (SPIM)**  

It is basically spam delivered via instant messaging applications, the purpose of hostile SPIM is the same as that of spam.  

🟢 **Spear Phishing**  

This refers to a phishing attack that targets a specific person or group of people with something in common.  
Usually, the attack is customized to the target after previous data is gathered from that user or group.  

🟢 **Dumpster Diving**  

This is the process of going through a target's trash searching for valuable information that might be used in an attack.  
To reduce risks, an organization should have policies about discarding materials. Sensitive information should be shredded and the organization should consider securing the trash receptacle so that individuals can't forage through it.

🟢 **Shoulder Surfing**  

When an attacker directly observes the individual entering sensitive information on a form, key, pad, or keyboard.  

🟢 **Pharming**  

This attack consists of misdirecting users to fake websites made to look official, usually done after a phishing attack.  
The user will be directed to the fake website due to another attack technique such as DNS poisoning or modification of local host files.  

🟢 **Tailgating**  

Is the action of following closely behind a person who has just used their accesses to a room or building.  
This method relies on poor security practices in order to be successful.  

🟢 **Eliciting(Obtaining) Information**  

Calls to or from the help desk and tech support units can be used to elicit information.  
This technique aims to convince people to perform tasks resulting in security compromises.  
Posing as an employee, an attacker can get a password reset or information about the target systems.  

🟢 **Whaling**  

High-value targets are referred to as "whales".  
A whaling attack is where a target is a high-value person (such as a CEO, CFO, or CTO) and it is custom-built to increase the odds of success.  

🟢 **Prepending**  

This refers to adding something else to the beginning of an item, supplying information that the target will act upon before they even ask for that information in an attempt to legitimize the actual request coming later.  
This is a way to justify why the target should perform a specific action.  

🟢 **Identity Fraud**  

This is the use of fake credentials to achieve an end.  
Examples: Pretending to be an official representative of a government agency, a regulator, a lower risk person, a contractor, or the person that waters the plants.   
This works best when the target is expecting the impersonated individual.  

🟢 **Invoice Scams**  

Using a fake invoice in an attempt to get a company or entity to pay for things that were not ordered.  
Usually, the fake invoice is accompanied by a message suggesting a sense of urgency, a final notice, or a threat.  

🟢 **Credential Harvesting**  

Involves the collection of credential information (such as user ID, password, etc) enabling an attacker a series of access to a system.  
A common form of credential harvesting starts with a phishing e-mail that convinces a user to click a link.  
The objective is just to obtain credentials. Once the attacker has tricked the target, they will either redirect the user to the correct website or provide an error and a new connection to the correct website, this is a way to mask the attack.  

🟢 **Reconnaissance**  

This happens when an attacker examines the systems they intend to attack using a wide range of methods like google searches, public records, OSINT, social media, surveying a company's org charts, calling and asking for information, reading press releases, etc.   
The goal is to gather as much information as possible about the system and environment that will be under attack. 

🟢 **Hoax**  

A hoax can be damaging if it causes users to take some actions that weaken the security of a system.  
Users should be trained to be suspicious of unusual e-mails and stories and should validate the information with the system administrators or the company's security entities.  

🟢 **Impersonation**  

In this technique, an attacker assumes a role that is recognized by the target, the attacker uses the target's biases against their better judgment to follow procedures.  
Impersonation can occur in different ways, from third-party contractors to help desk agents, to vendors or even online resources.  
The best defense is simple: have processes in place that require employees to see a person's ID before engaging with them if the employees do not know them, this includes people such as delivery drivers.  
In addition to having policies, regular training and continuous awareness programs have proven to be effective.  

* **Third-Party Authorization**  
Using previous information about a project, deadlines, bosses, etc., the attacker arrives or comes up with something that the victim will see as normal or expected.  
The attacker is viewed as helpful or someone not to upset, the main goal is to create the appearance of a third-party authorization when there is none. 

* **Contractors/Outside Parties**  
It is common nowadays to have outside contractors clean the building, water the plants, or perform other routine chores.  
Without proper safeguards or policies, an attacker can simply put on clothing that matches a contractor's uniform, show up to do the expected job at a slightly different time than it's usually done, and roam the halls unnoticed while gathering information about the target system/environment.  

* **Online Attacks**  
This refers to the use of impersonation employed in online attacks: pop-ups, phishing, social media scams, etc.  

🟢 **Watering Hole Attack**  

Attackers can plant malware at sites where users are likely to frequent it.  
This attack involves infecting a target website with different types of malware.
This technique is complex to achieve and appears to be backed by nation-states and other high-resource attackers.  
The typical attack vector will be a zero-day attack or vulnerability to furthr avoid detection.  

🟢 **Typosquatting**  

Is an attack form that involves capitalizing upon common typographical errors.   
The attacker registers mistyped URLs so the victim will land on the attacker's website to perform a chained attack such as phishing, impersonating, credential harvesting, or malware infection.  
This attack is also referred to as URL hijacking, fake URL, or brandjacking.  

🟢 **Pretexting**  

This occurs when the attacker uses a narrative (pretext) to influence the victim into giving up some information.  
The pretext does not have to be true, it only needs to be believable and its main goal is to gain the target's trust and exploit it.  

🟢 **Influence Campaigns**  

It involves the use of collected information and selective publication of material to alter perceptions and change people's minds on a topic.  
This attack becomes more powerful when used in conjunction with social media to spread influence.   
Nation states have used this technique as a form of conflict (hybrid warfare), in previous wars, this was known as "propaganda".  
The information is used to sway people towards a position favoring those spreading it.


