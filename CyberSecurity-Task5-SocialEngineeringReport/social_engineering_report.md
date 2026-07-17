## Introduction 

Social engineering is one of the most hacking techniques used , it is a manipulation technique that exploits human error to gain access to private information. Human error is the result of trusting someone  without a question the hacker creates an environment of false trust and lies to exploit many people as possible.  
In order to achieve social engineering you need to follow a few tactics 
1st is authority , they impersonate individuals with power on purpose , because people are condition to respect and follow authority figures. 
2nd is intimidation they do this by bullying and  persuasion. 
3rd is consensus for example a threat actor might try to gain access to private data by telling an employee that other people at the company have given them access to the data in the past . 
4th is scarcity it is used to show that services are limited .
5th is urgency , attacker persuades others to respond quickly and without questioning. 
And the last one is trust , it is when an attacker builds and emotional relationship with the user so it can be exploited over time.


## Phishing 
Phishing is the use of digital communications to trick people into revealing sensitive data of deploying malicious software 
Types of phishing 
Business email compromise (BEC) is when a threat actor sends an email message that seems to be from known source to make a seemingly a true  request for information , in order to obtain a financial advantage.
Spear phishing is a malicious email attack that targets a specific user or group of users. The email seems to originate from a trusted source. Whaling is also a form of spear phishing . It is when a threat actors targets company executives to gain access to sensitive data . 
Vishing its is the exploitation of electronic voice communication to obtain sensitive information or impersonate a known source. 
Smishing is the use of text messages to trick users in order to obtain sensitive information.

### Real world case study

In march 2011 an RSA employee opened an email from their junk folder that contained a malicious excel sheet . This sheet triggered an unpatched adobe flash zero day exploit and installed a back  door called poison ivy  , allowing the elite Chinese cyber espionage unit to silently breach the network . They targeted RSA's secret keys that generated numbers for millions of secure ID fobs. This incident  birthed the cryptographic, un-phishable hardware keys used today


### Prevention methods 
Do not open links or attachments without verifying the sender 
Do not reveal any personal or organizational information to anyone 
Use multifactor authentication 
Utilize any anti-phishing features offered by a web browser 

---

## pretexting

threat actors take advantage of the weakest point of your network whitch is you. pretexting is basically when a threat actor search their victims
social media to collect informatio before making any move.When it is time to attack they already know stuff about the victims life. They make up a false  story or impersonate as some one who is trust worthy to the victim , persuading them into revealing confidential information.



## Case study 

In 2006 hewlet Packard noticed that private information is being leaked from it's board of directors , so he hired privet investigators to identify the source . Investigators used the pretexting method , pretending they are an HP board members. Through this impersonations they convinced companies to disclose confidential phone records without authorization. When the deception became public, it led to investigations by law enforcement, legal action, the resignation of HP's chairwoman Patricia Dunn, and increased awareness of the risks of social engineering. The incident became one of the most well-known real-world examples of pretexting, demonstrating how attackers can manipulate people into revealing sensitive information without using technical hacking methods.

## Prevention methods
- Verify the identity of anyone requesting sensitive information.
- Never disclose passwords or confidential information without independent verification.
- Conduct regular employee security awareness training focused on impersonation attacks.

## USB  baiting 
A threat actor strategically leaves a malware USB stick for an employee to find and install , to unknowingly infect a network. This happens when there is  a physical social engineering attack which is when a threat actor impersonates an employee , customer or a vendor to have unauthorized access to a location.

## Prevention 

For  this type of attack you have to aware of your surrounding so it is advised to be suspicions of random visits from customers or vendors . 
Do not use USB's that are not yours or not knowing where they came from.
Be alert for any suspicious or unusual activity.

## Case study 
One of the most famous baiting attacks is credit union USB drop experiment 2006
A security consultant wanted to do an authorized penetration testing so what he did is that he scattered 20 USB flash drives infected with harmless trojan in employee parking lots and smoking areas. Employees found 15 out of 20 USBs and all of them were plugged into the company computers , the malware successfully collected information like usernames , passwords and computer information.


## Quid pro quo

Quid pro quo means " something for something" just like a transaction , if you do this i will do something in return for you.  An attacker will act like a IT  support and will  keep calling people to find someone who actually has a problem . Once they find a victim, they give them malicious instruction When executed, these instructions compromise the victim’s computer. This attacker can install a malware or collect information. 

## Prevention methods 
- Do not pickup calls from unknown numbers
- Try to identify the person who is talking to you
- Do not give any information about you 
- Make sure to contact the company IT support team through the company website 

## Social Engineering Attack Comparison

| Attack | Primary Target | Attack Type | Psychological Lever Exploited | Best Countermeasures |
|--------|----------------|-------------|-------------------------------|----------------------|
| **Phishing** | General users and employees | Fraudulent emails, messages, websites, or phone/text communications to steal credentials or deliver malware | **Urgency, fear, trust, curiosity** | Verify the sender before opening links or attachments, use Multi-Factor Authentication (MFA), avoid sharing sensitive information, enable anti-phishing protection |
| **Pretexting** | Employees and individuals with access to sensitive information | Impersonation using a fabricated identity or scenario to obtain confidential information | **Trust, authority, helpfulness** | Verify identities before sharing information, never disclose passwords or confidential data without independent verification, provide employee security awareness training |
| **USB Baiting** | Employees with physical access to company computers | Physical social engineering using infected USB devices left in public areas | **Curiosity, temptation** | Never connect unknown USB devices, report suspicious devices, educate employees, restrict USB access through security policies |
| **Quid Pro Quo** | Employees seeking technical support or assistance | Offering a service or benefit in exchange for information or system access | **Reciprocity (something for something), trust, authority** | Verify the caller's identity, contact the official IT department through trusted channels, never follow unsolicited instructions, avoid sharing sensitive information |

## organizational reccomendations 


  *Employees should be trained to identify scam calls from legitimate ones
  
  *Employees should be trained to spot malicoius links before opening them
  
  *Employees should have situational awarness in thier work invironment
  
  *Employees should learn to identify the person they are communicating with in order to make sure it's not an attacker
  
  *They should not give any personal or organizational information


## citations 

Brozycki, J. (2009). Inside a phish. SANS Institute Reading Room. https://www.sans.org/white-papers/33139

Cybersecurity and Infrastructure Security Agency. (2021, February 1). Avoiding social engineering and phishing attacks. https://www.cisa.gov/news-events/news/avoiding-social-engineering-and-phishing-attacks

Greenberg, A. (2020, August 18). Inside the Twitter hack—and what happened next. WIRED. https://www.wired.com/story/inside-twitter-hack-election-plan/

Greenberg, A. (2021, May 20). The full story of the stunning RSA hack can finally be told. WIRED. https://www.wired.com/story/the-full-story-of-the-stunning-rsa-hack-can-finally-be-told/

National Institute of Standards and Technology. (n.d.). Phishing. Computer Security Resource Center Glossary. https://csrc.nist.gov/glossary/term/phishing

National Institute of Standards and Technology. (n.d.). 
Social engineering. Computer Security Resource Center Glossary. https://csrc.nist.gov/glossary/term/social_engineering

SANS Institute. (n.d.). Glossary of security terms: Social engineering. https://www.sans.org/security-resources/glossary-of-terms

University of Florida Information Technology. (n.d.). 
Quid pro quo. https://it.ufl.edu/security/learn-security/social-engineering/quid-pro-quo/

Zetter, K. (2006, September 14). Protect yourself from pretexting. WIRED. https://www.wired.com/2006/09/protect-yourself-from-pretexting/



















