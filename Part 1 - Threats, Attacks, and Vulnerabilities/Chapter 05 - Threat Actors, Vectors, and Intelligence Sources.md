# CompTIA SY0-501 Security+ Study Notes

## Part 1 - Threats, Attacks, and Vulnerabilities  
### Chapter 05 - Threat Actors, Vectors, and Intelligence Sources

First a few definitions:
Cyber **threats** are potential dangers that could compromise a system's security.<br>
A **threat actor**, the source of such threats, utilizes various methods, known as **vectors**, to exploit system vulnerabilities for their goals. <br>
**Threat intelligence** is evidence-based knowledge that aids in preventing or mitigating cyber attacks.<br>
**Intruders**, varying in sophistication, are individuals or groups attempting unauthorized access into a system.<br>

## **Actors and Threats**

<img src="https://raw.githubusercontent.com/DelfinoRT/CompTIA-Sec-SY0-601-In-Depth-Study-Notes/main/Part%201%20-%20Threats%2C%20Attacks%2C%20and%20Vulnerabilities/Distribution%20of%20attacker%20skills.png" width="50%" title="Intro Card" alt="Intro Card">

🟢 **Advanced Persistent Threats (APTs)**  

An Advanced Persistent Threat (**APT**) attack uses toolkits to infiltrate a target network and maintain a prolonged presence to avoid detection.<br>
Due to the intensive resources required, **APTs typically target high-value entities** like nation states or large corporations with the aim of long-term information theft, unlike the quick "hit and run" tactics of many black hat hackers.<br>
APTs typically progress in stages: <br>
1) Gaining Access
2) Establishing a Foothold
3) Deepening Access
4) Moving Laterally
5) Observing, Learning, and Remaining undetected

🟢 **Insider Treats**  

While most security measures focus on protecting against external threats, insider threats pose a unique challenge as they **come from within the organization**.<br>
Insiders, with their access and knowledge, can cause significant damage. These threats often originate from disgruntled employees seeking to disrupt operations, but can also be unintentional.<br>
However, employees aren't the only potential insiders. Others with physical access to company facilities, like contractors, partners, and maintenance crews, should also be considered when addressing insider threats.

🟢 **State Actors**  

**State-sponsored** hackers, often considered elite due to their highly technical skills, exploit and discover new vulnerabilities. Some work for cybersecurity firms combating cybercrime, while others operate under nation-states, running groups of skilled hackers to conduct large-scale attacks.<br>
These state actors, **typically well-funded**, primarily aim to **compromise intelligence data of other governments** and frequently **execute Advanced Persistent Threat (APT) attacks**.<br>
Many countries now have the capability to conduct information warfare, characterized by extended preparation, significant financial support, and organized hacker groups. Potential targets for state actors include military forces, national infrastructure (water, gas, electricity, oil), refineries, distribution systems, banks, and telecommunications.

🟢 **Hacktivists**  

A step above the script kiddies, we find **intermediate threat actors**. These individuals are considerably more **technically competent**, capable of writing scripts to exploit known vulnerabilities. They are far more advanced than script kiddies, who can sometimes be used as 'ground troops' to amplify an attack.<br>
When these hackers unite for a collective effort, typically in support of a cause, they are referred to as **hacktivists**. A **hacktivist** is someone who leverages hacking to effect political or social change. The term "hacktivist" can be traced back to 1994, originating from the hacker group **"Cult of the Dead Cow"**.<br>
Hacktivism represents a blend of **activism and hacking**, often deployed as a form of civil disobedience to protest against issues like censorship, human rights violations, or other political and social matters. Despite the potentially noble intentions, hacktivism activities are **illegal** and can cause significant damage, disrupting services and leaking sensitive information.<br>
Therefore, it's crucial to have robust **cybersecurity measures** in place to protect against these sophisticated threats.

🟢 **Script Kiddies (Skiddies)**  

On the **lower end of the technical spectrum**, we find individuals known as **script kiddies**. These are individuals who lack the technical expertise to create scripts or unearth new software vulnerabilities. However, they possess just enough understanding of computer systems to download and execute scripts developed by others.<br>
The majority of the **'unfriendly' activities** noted on the internet are likely the work of these individuals. It's important to note that not all novice hackers fall into the script kiddies category. Some less experienced attackers strive to comprehend the tools they utilize.<br>
In contrast, **script kiddies show no interest in learning** about the exploits they use. They prefer what's easily accessible and readily available. Their motivations are typically simple and personal, ranging from seeking fun, creating chaos, and craving attention, to exacting revenge.<br>
The term **"script kiddie"** made its first appearance in hacker magazines, blogs, message boards, and Internet Relay Chat around the mid-1990s. It's worth mentioning that, despite their limited skill, script kiddies can still pose a threat due to the powerful exploits available online. Therefore, it's vital to maintain up-to-date system security to defend against such potential threats.


🟢 **Criminal Syndicates**  

Criminal syndicates represent a significant category within **cybersecurity criminals**. They operate under the veil of anonymity, focusing on creating malware and launching attacks aimed at **stealing identities, financial data, and intellectual property**. Their primary motivation is financial gain.<br>
A key distinction between criminal syndicates and the "average" hacker lies in the level of organization. Criminal groups typically demonstrate a higher degree of planning and coordination in their attacks, often backed by substantial financial resources. Their determination to reap high rewards makes them willing to invest more time and money into their illicit activities.<br>
Criminal syndicate attacks usually fall into the **structured threat category**. These threats are characterized by extensive planning, longer operation times, sizable financial backing, and potential corruption or collusion with insiders.<br>
In the present day, criminal syndicates often exploit national jurisdictions lacking robust legal frameworks and technical capabilities to combat cybercrime. The ease of communication, anonymity, and accessibility of tools for illegal operations have transformed cybercrime into a **global, rapidly growing, and profit-driven industry**. Organized criminal groups thrive in this environment, making them a major concern in the field of cybersecurity.

## **Hackers**  

The term 'hacker' originally referred to individuals who sought to understand the workings of a system in order to control it beyond its intended design. Over time, the term has evolved and is now used to describe **anyone who improperly uses computers**, including those engaged in criminal activities.<br>
To categorize hackers based on the legality and ethicality of their activities, descriptors such as **authorized, unauthorized, and semi-authorized** are used. An *authorized* hacker, often known as a 'white hat' hacker, legally tests systems for vulnerabilities with the intent to improve security. An *unauthorized* hacker, or 'black hat', exploits system vulnerabilities for malicious or personal gain. A *semi-authorized* hacker, or 'grey hat', operates in the middle ground, often hacking without explicit permission but with no malicious intent.<br>
Understanding the different types of hackers is crucial in the field of **cybersecurity** as it helps in developing targeted defense strategies against potential cyber threats. 

🟢 **Authorized**  

**Authorized hackers**, often termed as **"white hat" hackers**, are professionals who use their exceptional skills to enhance cybersecurity. They function with the main aim to **identify vulnerabilities** and **strengthen security systems**.<br>
These individuals could be **security consultants** who perform a range of activities, including but not limited to, **chasing vulnerabilities** and **conducting penetration tests**. They implement the **same tools and techniques** as malicious hackers, however, the distinguishing factor is their **ethical approach**.<br>
Their operations are **registered and monitored** by the organizations or firms they work for, allowing them to understand the system's weaknesses in-depth. With this knowledge, they can devise strategies to **fix the identified vulnerabilities**, ultimately bolstering the cybersecurity infrastructure.<br>
In essence, white hat hackers play a pivotal role in **proactive cybersecurity**, aiding organizations in staying one step ahead of potential cyber threats.

🟢 **Unauthorized**  

Unauthorized hackers, also known as '**Black Hat**' hackers, are the antithesis of '**White Hat**' hackers. Their expertise and knowledge are predominantly used for illicit activities and operations that violate laws, thereby posing a significant risk to various systems.<br>
The term '**Black Hat**' originates from the 1950s Western films where the villains typically wore black hats, while the heroes wore white hats. This has led to the use of the term in the cybersecurity context to differentiate between ethical and non-ethical hackers.<br>
**Black Hat hackers** exploit security vulnerabilities primarily for financial gain. Their activities may include stealing or destroying private data and manipulating, disrupting, or shutting down websites and networks. Their actions often result in substantial damage, causing significant financial losses and reputational harm to the affected parties.

🟢 **Semi-authorized**  

**Gray hat hackers** are semi-authorized actors who may sometimes breach laws or typical ethical norms, but unlike black hat hackers, they **don't usually possess malicious intentions from start**. They are positioned between white hat hackers, who exploit system vulnerabilities legally and ethically (while at their job), and black hat hackers, who exploit weaknesses illegally and with harmful intent.<br>
Gray hat hackers often justify their actions by arguing that the **internet is not safe** and it is their mission to enhance its security for individuals and organizations. They do this by hacking websites and networks, creating disruptions to prove their point. Their curiosity may lead them to probe high-profile systems, even if it infringes on privacy rights and other laws.<br>
Despite their controversial methods, gray hat hackers often provide **valuable information** to companies about their system vulnerabilities. However, their actions are generally viewed as unethical by the white hat community and are considered illegal as they **usually don't seek permission to infiltrate systems**.<br>
To encourage gray hat hackers to report vulnerabilities rather than exploit them, some companies run **bug bounty programs**. These programs provide incentives for gray hats to disclose system vulnerabilities instead of exploiting them for personal gain. It's important to note that obtaining the company’s permission is the only legal means to probe their systems.<br>
In certain instances, **if organizations do not promptly respond or comply, gray hat hackers may resort to black hat tactics by publishing exploitation methods on the internet** or directly exploiting the vulnerability themselves.

## **Shadow IT**  

**Shadow IT** signifies the unauthorized use of technology by employees, including software, hardware, and cloud services. This issue often surfaces when employees deviates from active IT policies to use unapproved tools for accomplishing tasks more efficiently. These shadow IT groups usually rise up of a desire to 'get things done' when central IT does not respond in what the unit considers to be a reasonable timeframe.<br>
While Shadow IT may occasionally increase productivity, it inadvertently exposes organizations to security threats, compliance problems, and financial liabilities. <br>
Key concerns related to Shadow IT and cloud security include:
* **Data Leakage** – Unauthorized cloud services often lack robust security controls, elevating the risk of sensitive data access or leakage. <br>
* **Compliance Violations** – Using unsanctioned cloud services may lead to non-compliance with industry regulations or internal policies, potentially resulting in fines and damage to reputation. <br>
* **Limited Visibility** – IT departments may find it difficult to maintain visibility and control over the organization's cloud environment in the presence of Shadow IT, making the detection and response to potential security incidents challenging. <br>
* **Increased Attack Surface** – Unauthorized cloud services can broaden an organization's attack surface, offering cybercriminals more entry points to exploit. <br>
Often, users resort to Shadow IT to expedite their work, but such usage remains unknown to the IT team and thus, unprotected by the organization's cybersecurity measures. In the context of cloud workloads and developer services, assets may harbor significant vulnerabilities like default passwords or misconfigurations, amplifying the risk of data breaches, noncompliance, and other liabilities.

## **Competitors**  

**Competitors** can pose significant threats to businesses, not only through traditional means such as sales, markdowns, and rival products but also in the digital realm. The fight is essentially for **customer acquisition** and retention. <br>
In the digital world, competitors may resort to various unethical and potentially illegal methods, ranging from mild to severe. These methods may include:
* **False product reviews**: This is a less severe but still harmful method used to tarnish a company's reputation and sway potential customers. 
* **System hacking**: This is a more severe method where competitors may hack a company's systems. The consequences can be quite harmful, including:
  - **Theft of intellectual property**
  - **System disruptions**
  - **Access to customer lists**
* **Denial-of-service attacks**: This is an extreme form of cyber threat where the competitor overwhelms the company's server with unnecessary requests, causing it to crash and become unavailable to customers. <br>

## **Attributes of Actors**  

**Threat actors** in cybersecurity are classified based on several factors. These include their abilities, location (either internal or external), level of sophistication, resources and funding, and their intent and motivation. <br>
Not all threat actors are driven by financial gain. Their motivations can be diverse, ranging from political or commercial espionage to pursuing a social or political agenda. Some threat actors are motivated by the thrill of discovering vulnerabilities to make a name for themselves. <br>
The key characteristics that distinguish different types of threat actors are their level of sophistication and the resources they have at their disposal to execute attacks. <br>

🟢 **Internal/External**  

**Threat actors** can be categorized into two main types: **internal** and **external**. <br>
**Internal threat actors** have a significant advantage in that they already possess access to the system. Even if this access is restricted to a user level, it still enables them to execute their attack. This access privilege significantly reduces the steps they need to take to compromise the system. <br>
On the other hand, **external threat actors** must first establish access to the target system. External threats typically originate outside the network, including public-facing forums and global events. <br>
Therefore, an effective cybersecurity strategy should consider both internal and external threats, and implement measures to protect against both types of threat actors.

🟢 **Levels of Sohistication/Capability**  

Threat actors' skill levels can vary significantly within a group, with a few highly skilled individuals often leading a larger number of less skilled participants. The higher the skill level, the more likely the individual is to design and lead attacks. <br>
Interestingly, as skill level increases, the use of minimal methods also rises. **True zero-day vulnerabilities** are seldom exploited; they are preserved for situations with no other options due to the fact that once these vulnerabilities are exploited, they are promptly patched. Despite the resources available to nation-state teams, many attacks are old, exploit outdated vulnerabilities, and use simple methods that exploit easy targets. <br> 
The sophistication level of a threat actor is a critical factor in assessing the risk of an attack. More skilled threat actors have a higher chance of a successful attack, while less skilled attackers have a lower probability of success. <br>
Currently, a 'de-facto' standard, **STIX (Structured Threat Information eXpression)**, is trending. STIX is a language designed for sharing cyber threat intelligence. Version 2.0 defines Threat Actor Sophistication in seven levels, ranging from None to Strategic. The None level denotes actors who carry out random acts of disruption or destruction with tools they don't understand, while the Strategic level includes state actors who create vulnerabilities in commercial products during design, development, or manufacturing, or have the ability to impact products while in the supply chain to enable network and system exploitation. <br>

🟢 **Resources/Funding**  

**Threat actors**, such as **criminal organizations and nation-states**, often have robust resources including larger budgets, more personnel, and the ability to sustain long-term campaigns. These resources are critical, as Advanced Persistent Threats (APTs) demand significant expenditure to maintain teams and tools for prolonged periods. <br>
**APTs** are particularly resource-intensive, requiring sustained funding and effort to successfully infiltrate and compromise systems. These resources often come from well-funded organizations capable of managing such campaigns over an extended period. <br>
In summary, the scale and duration of cyber threats, are often directly correlated to the resources and funding of the threat actors. This explains why major organizations like criminal networks and nation-states are often behind the most significant and persistent cyber threats.

🟢 **Intent/Motivation**  

The intent or motivation of a threat actor can range from simple curiosities to highly complex objectives. A useful framework for understanding their motivations is the **M.I.C.E** acronym:
- **M – Money**
- **I – Ideology**
- **C – Compromise**
- **E – Ego**

**Money** <br>
Money is the most common motivator. Threat actors, driven by financial gain, often cast a wide net, targeting easy victims. They can profit from selling stolen data on the black market or engaging in ransom attacks. Even nation states, like North Korea, have been found to target companies for financial gain, specifically those in cryptocurrency exchange or intellectual property sectors. <br>

**Ideology** <br>
Threat actors driven by ideology pose a unique challenge, as their actions are often based on subjective beliefs. These individuals or groups may aim to shame or embarrass organizations that conflict with their principles. Nation states can also be motivated by ideology, targeting specific groups with well-funded and persistent attacks. It's crucial for organizations to understand the data these actors may pursue and to protect it diligently. <br>

**Compromise** <br>
The compromise category typically refers to insider threats. Sometimes, changes in business mandates or policies can lead employees to act against their own organizations. With the rise of "bring your own device" (BYOD) policies in hybrid work environments, organizations must remain vigilant and proactive in detecting potential insider threats. <br>

**Ego** <br>
Egotistical threat actors may target organizations to prove a point or settle personal scores. This motivation often comes into play in high-turnover companies or following contentious employee separations. To mitigate these threats, organizations need to implement dual control measures. <br>

It's worth noting that motivations can overlap or vary greatly depending on the threat actor's skill level and objectives. Other motivations for cyberattacks can include:

- **Financial Gain**: Cybercriminals often steal sensitive information for sale or fraudulent use.
- **Espionage**: Nation-states or corporate competitors may gather sensitive information for political, economic, or strategic advantages.
- **Hacktivism**: Individuals or groups may conduct cyberattacks to promote their ideologies or protest perceived injustices.
- **Sabotage and Disruption**: Some actors aim to disrupt critical infrastructure or services for political or ideological reasons.
- **Personal Vendettas**: Disgruntled employees or partners may misuse their access to sensitive information or systems for personal gain or revenge.
- **Ransom**: Ransomware attacks involve encrypting data and demanding payment for its release.
- **Political Discord**: Extremist groups may use cyber methods to spread propaganda, recruit members, or coordinate activities.
- **Competitive Advantage/Stealing Trade Secrets**: Business rivals may engage in cyber espionage or attacks to gain a competitive edge.
- **Thrill-Seeking and Notoriety**: Some individuals hack for the thrill, seeking recognition within hacker communities.

**Script Kiddies** are beginners in the world of hacking, with their primary goal being to merely execute a technique successfully. Their motivation is often driven by curiosity rather than malicious intent. <br>
**Hacktivists**, on the other hand, are more skilled threat actors. Their actions are purpose-driven and often aim to make a political or social statement. They use their skills to exploit vulnerabilities to make their point. <br>
Lastly, the **Advanced Persistent Threats (APTs)** are the most sophisticated category of threat actors. Their intent or motivation is tri-fold: 
1. Continual access: APTs strive to maintain constant access to their targets. 
2. Stealth: APTs aim to remain undetected for as long as possible to avoid raising suspicion and to continue their activities.
3. Theft: The ultimate goal of APTs is to steal valuable information from the network they have infiltrated. They don't expend resources on maintaining access and stealth without the intent of extracting something of value.


## **Vectors**  

**Threat vectors**, also known as **attack vectors**, refer to the various methods or pathways through which hackers can gain unauthorized access to confidential data or sensitive information. These vectors are essentially the potential weaknesses that cyber criminals exploit to breach a system's security. <br>
**The entry points for these threat vectors can be diverse**, ranging from direct access channels like wireless networks or emails, to more indirect methods involving social media, supply chain attacks, and external data sources such as removable media. Even cloud-based systems are not immune, serving as yet another potential entry point for these cyber-attacks. 

🟢 **Direct Access**  

**Direct Access** signifies that an attacker has direct interaction with the system. This threat vector could be a result of an **insider attack** (where a trusted user abuses their access) or could involve outsiders who are given the opportunity to engage directly with systems. For instance, this can occur with a web server exposed to the public internet.<br>
It's essential to note that Direct Access is the core reason for implementing the **Principle of Least Privilege (PoLP)**. The PoLP is a computer security concept in which a user is given the minimum levels of access, or permissions, necessary to perform his/her job functions. This approach minimizes the risk of a potential data breach.

🟢 **Wireless**  

**Wireless networking** significantly simplifies connectivity. It provides an array of benefits but also introduces numerous **security challenges** into the equation. <br>
Unlike wired networks, wireless networking removes the need for **physical access** to perform an attack. The wireless signal can reach an attacker who might be positioned at a remote location, such as a parking lot. This accessibility considerably expands the potential **attack surface** and introduces new vulnerabilities that must be addressed. <br>

🟢 **E-mail**  

E-mail serves as a prominent **threat vector** in the realm of cyber security, frequently utilized in **social engineering attacks**. Given the reliance of most individuals and organizations on email for communication and coordination, it's a prime vector for cybercriminals aiming to trick users into divulging sensitive data, such as financial and personal information. <br>
Historically, email was developed without profound security measures, leaving it vulnerable to various forms of exploitation. Consequently, the cyber security community is continually battling to fortify email security against continuously evolving threats. <br>
One common attack method involves sending an email embedded with **malicious links or attachments**. If the email message is crafted convincingly enough, users may be enticed to click on the links or open the attachments. Once engaged, the threat vector effectively delivers its **payload**, successfully breaching the user's cyber defenses.

🟢 **Supply Chain**  

The **supply chain threat vector** involves exploiting a company's supply chain to execute a cyber attack. The attacker manipulates the supply chain by injecting malicious code into a product or its updates. This is achieved by either directly infiltrating the vendor's software or by tampering with the update mechanism to distribute corrupted files. <br>
Companies tend to trust their vendors implicitly, and this trust often leads them to overlook necessary security checks. In the absence of these checks, malware can easily spread to the vendor's customers. <br>
This form of attack, known as **supply chain attack**, is a serious threat that can't be mitigated solely through policy enforcement and contractual agreements. It emphasizes the importance of maintaining **rigorous security protocols at all points in the supply chain** process.

🟢 **Social Media**  

**Social media**, being a core business and communication platform, acts as a **vector for social engineering attacks**. Unlike corporate e-mail and other communication channels, it lacks numerous security checks, thus providing an easy passage for attackers to the user. <br>
Every industry confronts unique risks on social media, often leading to public controversy or negative press. These risks range from **phishing attacks** and **account compromise**, to **fraud**, **scams**, and **impersonation**. <br>
Therefore, **social media security** becomes a pivotal factor for modern business success. It involves the analysis of dynamic social media data to protect against cyber security and business threats. Many organizations, however, are yet to recognize social media as an evolving attack vector. These organizations remain vulnerable to potential threats due to this blind spot.

🟢 **Removable Media**  

**Removable media**, particularly **USB memory sticks**, represent a significant **threat vector** in cybersecurity. These devices require no special skill to use and **can be manipulated by attackers to execute malware** by an unsuspecting victim. <br>
This method is often employed in a social engineering attack known as a **USB drop attack**. In this scenario, the attacker leaves the infected USB device in a location where it's likely to be found and used, thus spreading the malware.

🟢 **Cloud**  

Unauthori

## **Threat Intelligence Sources**  

Unauthori

🟢 **Open Source Intelligence (OSINT)**  

Unauthori

🟢 **Closed/Proprietary**  

Unauthori

🟢 **Vulnerability Databases**  

Unauthori

🟢 **Public/Private Information Sharing Centers**  

Unauthori

🟢 **Dark Web**  

Unauthori

🟢 **Indicators of Compromise (IOC)**  

Unauthori

🟢 **Automated Indicator Sharing (AIS)**  

Unauthori

🟢 **Structured Threat Infomation Expression (STIX) / Trusted Automated Exchange of Intelligence Information (TAXII)**  

Unauthori

🟢 **Predictive Analysis**  

Unauthori

🟢 **Threat Maps**  

Unauthori

🟢 **File/Code Repositories**  

Unauthori

## **Research Resources**  

Unauthori

🟢 **Vendor Websites**  

Unauthori

🟢 **Vulnerability Feeds**  

Unauthori

🟢 **Conferences**  

Unauthori

🟢 **Academic Journals**  

Unauthori

🟢 **Requests for Comments (RFCs)**  

Unauthori

🟢 **Local Industry Groups**  

Unauthori

🟢 **Social Media**  

Unauthori

🟢 **Threat Feeds**  

Unauthori

🟢 **Adversary Tactics, Techniques, and Procedures (TTPs)**  

Unauthori
