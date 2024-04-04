Forensic Ethics & Methodologies
 Amateur
 By: Yosri Ghorbel
 Weight: 1
 Migrated to checker v2:
 Your score will be updated as you progress.


Resources
Read or watch:
What is Computer Forensics
What is SEIM
Ethical Insights: IT Forensics, Ethics and Risks
Digital Forensics and Incident Response
Digital Forensics Methodologies
Digital Forensics: What, Why and How ?
The Digital Forensic Investigation Process
Basic Steps in Forensic Analysis of Unix Systems
References:
ACPO
SWGDE
DFRWS
ISFCE
IJDE
NIST
Forensic Focus
Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

What is digital forensics?
Why is ethics important in digital forensics?
What are common ethical issues in digital forensics?
What is the role of integrity in forensic analysis?
How does one maintain objectivity in digital investigations?
What are the ACPO principles for computer forensics?
How do you ensure evidence is admissible in court?
What is chain of custody and why is it crucial?
What are the stages of the digital forensic process?
How does one document findings in a forensic report?
What are some standard digital forensic methodologies?
How does one handle digital evidence to preserve its integrity?
What are some common tools used in digital forensics?
What organizations set standards for digital forensic practices?
How do you stay current with evolving technology in forensics?
What are the legal implications of digital forensic investigations?
Requirements
General
All your files will be run on Kali Linux 2023.2
Allowed editors: vi, vim, emacs
You must substitute the IP range for $1.
The first line of all your files should be exactly #!/bin/bash.
All your files should end with a new line.
All your scripts should be less than 4 lines long $ wc -l file should print <= 4.
You are not allowed to use backticks, &&, || or ;.
Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
Quiz questions
Great! You've completed the quiz successfully! Keep going! (Show quiz)
Tasks
0. The Case of the Mysterious Image
mandatory
Welcome to your first foray into the world of digital forensics.
Your mission is to employ forensic analysis tools to reveal any concealed information or metadata, guiding your understanding of forensic concepts and methodologies.

Scenario:

You’ve been provided an image file (download), that is believed to contain crucial evidence related to an ongoing investigation.
Your objective is to analyze this image for hidden metadata or embedded information that could provide leads or insights into the case.

Examine Metadata:
Utilize exiftool to thoroughly analyze the image file’s metadata.
Identify Anomalies:
Look for any unusual or suspect metadata entries that could suggest the owner name.
Submission example:
$ cat 0-mystery.txt
John_Doe
Repo:

GitHub repository: holbertonschool-0x02_forensic_methodologies
Directory: cybersecurity_basics
File: 0-mystery.txt

0/4 pts
1. Unraveling Location Clues from Image Metadata
mandatory
Dive into the realm of geolocation forensics by unlocking the secrets hidden within image metadata. Your mission involves employing forensic tools to extract GPS coordinates from an image and use them to pinpoint the exact location on a map. This task not only expands your understanding of metadata’s value but also showcases how digital content can inadvertently reveal real-world locations.

Scenario:

Amid an ongoing investigation, you’ve obtained an image (download), allegedly linked to suspect activities. Initial assessments suggest the image contains embedded GPS coordinates. Your objective is to uncover these coordinates, utilize them to identify the location, and deduce the street name where the activities occurred.

Extract GPS Coordinates:
Use exiftool to meticulously extract the GPS coordinates from the image file’s metadata.
Pinpoint Location:
Enter the extracted GPS coordinates into Google Maps to locate the precise area.
Submission example:
$ cat 1-location.txt
123 Example St, Forensics City
Repo:

GitHub repository: holbertonschool-0x02_forensic_methodologies
Directory: cybersecurity_basics
File: 1-location.txt

0/4 pts
2. Deciphering the Intruder's Intent
mandatory
Sharpen your investigative reasoning by analyzing a cybersecurity incident scenario. Your understanding of cyber threats and their implications will guide you to deduce the intent behind a suspicious network activity.

Scenario:

A corporate network intrusion detection system (IDS) triggers an alert indicating a potential breach.
The alert details suspicious SSH (Secure Shell) login attempts from an unfamiliar IP address.
Analysts quickly isolate the IP and review access logs, discovering multiple failed login attempts followed by a successful authentication on a high-privilege user account.
Further investigation reveals a command history that includes network mapping and data exfiltration activities. Given the sequence of actions, you must determine the primary intent of the intruder.

What was the intruder’s primary intent?

A) To deploy ransomware across the network.
B) To conduct reconnaissance for future attacks.
C) To exfiltrate sensitive corporate data.
D) To sabotage the company’s website.
Submission example:

$ cat 2-intruder_intent.txt
F
Repo:

GitHub repository: holbertonschool-0x02_forensic_methodologies
Directory: cybersecurity_basics
File: 2-intruder_intent.txt

0/4 pts
3. Identifying the Vulnerability Type
mandatory
This exercise challenges you to apply your knowledge of common vulnerabilities, requiring logical deduction to identify the flaw that allowed an attacker to compromise a system.

Scenario:

A web application recently fell victim to an attack that led to unauthorized access to its customers data.
Investigators found that the attacker was able to inject malicious queries through the application’s user login form.
This unauthorized access resulted in the exposure of sensitive user data. Based on the information provided, determine the type of vulnerability exploited by the attacker.

Which type of vulnerability was exploited in this attack?

A) Cross-Site Scripting (XSS)
B) SQL Injection (SQLi)
C) Cross-Site Request Forgery (CSRF)
D) Remote Code Execution (RCE)
Submission example:

$ cat 3-vulnerability_type.txt
F
Repo:

GitHub repository: holbertonschool-0x02_forensic_methodologies
Directory: cybersecurity_basics
File: 3-vulnerability_type.txt

0/4 pts
4. Pinpointing the Attack Method
mandatory
Refine your ability to analyze and interpret cyber attack techniques through a detailed scenario.

Scenario:

An organization’s web server was compromised, leading to a significant data breach.
The initial forensic analysis revealed that the attacker gained access to the server by exploiting a service running on an open port.
This service was intended for remote management and was not updated regularly.
Further investigation showed that the attacker executed a series of commands to escalate privileges shortly after gaining initial access.
Given these details, determine the attack method employed by the attacker to compromise the web server.

Which attack method was most likely used by the attacker?

A) Phishing
B) Denial of Service (DoS)
C) Exploit of a Known Vulnerability
D) Password Spraying
Submission example:

$ cat 4-attack_method.txt
F
Repo:

GitHub repository: holbertonschool-0x02_forensic_methodologies
Directory: cybersecurity_basics
File: 4-attack_method.txt

0/4 pts
5. Unveiling the Ripple Effect
mandatory
Elevate your analytical prowess by sifting through the undercurrents of a cybersecurity scenario to deduce its indirect consequences.

Scenario:

Following routine maintenance, a retail corporation’s IT department notices an uptick in server load and irregular access patterns within their customer relationship management (CRM) system.
Initially dismissed as a side effect of recent system updates, further probes reveal unauthorized modifications to several customer profiles.
Although the alterations are subtle—changes to contact details and marketing preferences—the breach’s source remains elusive.
The corporation prides itself on customer service and data integrity, promoting these values as central to its brand identity.

Given the subtle nature of the breach, what indirect impact should the corporation be most concerned about?

A) Immediate financial losses due to operational downtime
B) Undermining of brand reputation and customer trust
C) A direct increase in spam emails sent to customers
D) Short-term website performance issues
Submission example:

$ cat 5-ripple_effect.txt
F
Repo:

GitHub repository: holbertonschool-0x02_forensic_methodologies
Directory: cybersecurity_basics
File: 5-ripple_effect.txt

0/4 pts
