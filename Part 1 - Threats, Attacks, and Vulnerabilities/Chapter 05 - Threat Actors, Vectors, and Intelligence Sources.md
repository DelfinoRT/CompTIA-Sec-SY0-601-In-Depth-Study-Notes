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
Hacktivism represents a blend of **activism and hacking**, often deployed as a form of civil disobedience to protest against issues like censorship, human rights violations, or other political and social matters. Despite the potentially noble intentions, hacktivism activities are **illegal** and can cause significant damage, disrupting services and leaking sensitive information. 

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

**White hat hackers**, often referred to as **ethical hackers**, are individuals who utilize their hacking skills for legitimate purposes. They are often employed as **security consultants** to identify vulnerabilities and perform **penetration tests** in a system, among many other security-related activities.<br>
These authorized hackers employ the same tools and techniques as malicious hackers (**threat actors**), but with a significant difference - they operate with the explicit permission of the organizations. Their primary aim is to understand the **system's weaknesses** and devise strategies to address them, thereby improving the system's security posture. This approach allows organizations to proactively defend against potential cyber threats.

🟢 **Unauthorized**  

These are cybersecurity criminals who lurk in the shadows of anonymity, create malware and perform attacks to steal identities, financial data, and intellectual property, all with an eye on lorem ipsum

🟢 **Semi-authorized**  

These are cybersecurity criminals who lurk in the shadows of anonymity, create malware and perform attacks to steal identities, financial data, and intellectual property, all with an eye on nlorem ipsum
