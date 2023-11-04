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

Unauthori

🟢 **Internal/External**  

Unauthori

🟢 **Levels of Sohistication/Capability**  

Unauthori

🟢 **Resources/Funding**  

Unauthori

🟢 **Intent/Motivation**  

Unauthori

## **Vectors**  

Unauthori

🟢 **Direct Access**  

Unauthori

🟢 **Wireless**  

Unauthori

🟢 **E-mail**  

Unauthori

🟢 **Supply Chain**  

Unauthori

🟢 **Social Media**  

Unauthori

🟢 **Removable Media**  

Unauthori

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
