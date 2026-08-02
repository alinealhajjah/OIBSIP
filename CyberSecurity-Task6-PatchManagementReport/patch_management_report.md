# Importance of patch management

## Introduction

According to **NIST SP 800-40 Rev. 4**, patch management is the process of identifying, prioritizing, acquiring, installing, and verifying the installation of patches, updates, and upgrades throughout an organization. The purpose of patch management is to reduce security risks by fixing vulnerabilities before attackers can exploit them. These are the five essential activities that NIST recommends.
Patch management has a huge role in the vulnerability management lifecycle. The lifecycle starts when a vulnerability is discovered. Then, it is assessed to determine how severe it is and how it could affect an organization's assets. After that, the software vendor develops and releases a security patch. Organizations then identify the affected systems, test the patch, install it, and verify that the installation was successful. The final stage is validation and monitoring, where systems are scanned again to confirm that the vulnerability has been removed and to make sure no new security issues have been introduced. This shows that patch management is the remediation stage of the vulnerability management lifecycle.

---
## why patches matter 

All software have vulnerabilities that why there are researchers who look for them after these vulnerabilities are discovered vendors release patches. These patches if not installed attackers will find the vulnerabilities and exploit them. This is why CVE is so important.
Common vulnerabilities and exposures ( CVE)  is a dictionary or a naming system that has a collection of publicly disclosed security flaws.  The mission of this program is to have a record for each vulnerability discovered , in this record the vulnerability is defined , identified and have a brief description. 
CVE record life cycle consist of :

1- discover 

2- Report : Discoverer reports a vulnerability to a CVE Program partner .

3- request : CVE  program partner assigns a CVE ID to the discovered vulnerability
-  CVE ID  is unique to every vulnerability it has the following format    
-  CVE prefix + Year + Arbitrary Digits --> the year section is not for the year it was discovered in but  the year it was published.
  
4- reserve : this is the first state of the CVE record this  means that CVE stakeholders are using the CVE ID for early-stage vulnerability coordination and management, but the CVE numbering authority (CNA) is not yet ready to publicly disclose the vulnerability.
   
5- Submit : the program partners submit the details like the impact , vulnerability type and root cause 

6- Publish : this is the last step of the life cycle , they  publish the record of the vulnerability which is the descriptive data about a vulnerability associated with a CVE ID

 Now we will take a look on famous real world breaches caused by unpatched systems.

 WannaCry Ransomware Attack (2017)
 This is one of the most famous attacks caused by weak patch management. On May 12, 2017 Microsoft server message block version 1 had a vulnerability that was exploited . The vulnerability, identified as **CVE-2017-0144**  allowed threat actors to exploit and execute malicious code remotely on vulnerable windows systems.  Microsoft had already released the **MS 17-010 security update on March 14, 2017**, nearly two months before the attack. However, many organizations had not installed the patch, leaving their systems exposed.
 Wanna cry was not only a ransomware attack but also behaved like a worm. When a computer was infected wanna cry encrypted the files of victims and demanded a payment in bitcoin. Spreading automatically to other unpatched computers on the same network. This malware infected thousands of computers across a 150 countries .

Equifax breach
In 2017 a huge security breach happened at Equifax  where the hacker stole the PII of  nearly 150 million people from Equifax database. This happened when  the attacker gained unauthorized access via the Internet to the online dispute portal that maintained documents used to resolve consumer disputes, this dispute resolution documents contained PII then the attacker located additional servers and login credential and kept extracting data for 76 days while remaining hidden. They slowly extracted data from 51 databases. 
 Unpatched system cause a huge threat to the company  it will result in Financial losses incurred to restore systems and files, and Potential harm to an organization’s reputation , also harms the costumers or vendors by stealing their PII.
 
---

## Consequences of not patching

### Damage to Reputation

Customers expect organizations to protect their personal information. A breach caused by poor patch management can damage an organization's reputation, reduce customer confidence, and lead to the loss of business opportunities.

### Operational downtime 

Attacks may force organizations to shut down for a period of time which will delay services , business operations this also reduce costumers trust 

### Compliance violations 

Many security frameworks require organizations to keep systems updated with security patches. Failing to do this may result in legal actions

  ### Financial Losses
  
- Incident response and forensic investigations
- System recovery and restoration
- Business downtime
- Lost productivity
- Legal expenses
- Compensation to affected customers
- Ransom payments 
### Real world statistics
Equifax agreed to a **settlement of up to $700 million** with the U.S. Federal Trade Commission, Consumer Financial Protection Bureau, and 50 states because it failed to protect consumers' personal information after an unpatched vulnerability was exploited.

According to the **IBM Cost of a Data Breach Report 2025**, the **global average cost of a data breach is USD $4.44 million**. The report also found that organizations using AI-powered security and automation saved an average of **USD $1.9 million** per breach compared with organizations that did not use these technologies. These findings show that investing in proactive security measures, including timely patch management, can significantly reduce the financial impact of cyber incidents.


##  Patch management lifecycle

life cycle consists of five stages:

1- Discovery : this is when organizations discover the vulnerability and make security audits to identify assets , software , libraries that are at risk.

2- Assessment: Evaluate the severity of each vulnerability using factors such as CVSS score, exploit availability, asset criticality, and business impact to determine patch priority.

3- Testing:  testing the patches should be planned before implementing the patch , they should make preparatory activities such as acquiring, validating, and testing patches for the vulnerable software; deploying additional security controls to safeguard the vulnerable software.They will prioritize the patch then schedule a deployment and test it to reduce operational risk .

4- Deployment : after the patch is tested we have several other factors affect the deployment of the patch: 
  The type of software being updated (e.g., firmware, operating system [OS], application)
  The asset platform type (e.g., IT, OT, IoT, mobile, cloud, virtual machine [VM],
Containers)
  Platform traits, such as managed/unmanaged asset, virtualized or not, and containerized or not
   Environmental limitations
   
5- Verification :  check if systems are working well and functioning and most important is to keep monitoring it.

## Best practices
* maintain a complete inventory of all hardware and software
* monitor for newly released vulnerabilities and patches
* identify risks and prioritize patches depending on the risk
* test patches
* deploy the patch
* verification phase
* keep monitoring , document and improve the process

## Challenges













## References section 

National Institute of Standards and Technology. (2022). Guide to enterprise patch management planning: Preventive maintenance for technology (Special Publication 800-40 Rev. 4). https://doi.org/10.6028/NIST.SP.800-40r4

The MITRE Corporation. (n.d.). Common Vulnerabilities and Exposures (CVE). https://www.cve.org/

National Institute of Standards and Technology. (n.d.). National Vulnerability Database. https://nvd.nist.gov/

U.S. Government Accountability Office. (2018). Data protection: Actions taken by Equifax and federal agencies in response to the 2017 breach. https://www.gao.gov/products/gao-18-559

Microsoft Security Response Center. (2017). Microsoft Security Bulletin MS17-010. https://msrc.microsoft.com/

Cybersecurity and Infrastructure Security Agency. (n.d.). Known Exploited Vulnerabilities Catalog. https://www.cisa.gov/known-exploited-vulnerabilities-catalog

National Institute of Standards and Technology. (2022). Guide to Enterprise Patch Management Planning: Preventive Maintenance for Technology (NIST SP 800-40 Rev. 4). https://doi.org/10.6028/NIST.SP.800-40r4

Cybersecurity and Infrastructure Security Agency. (n.d.). Known Exploited Vulnerabilities Catalog. https://www.cisa.gov/known-exploited-vulnerabilities-catalog


U.S. Government Accountability Office. (2018). Data Protection: Actions Taken by Equifax and Federal Agencies in Response to the 2017 Breach. https://www.gao.gov/products/gao-18-559

Federal Trade Commission. (2019, July 22). Equifax to pay $575 million as part of settlement with FTC, CFPB, and states related to 2017 data breach. https://www.ftc.gov/news-events/news/press-releases/2019/07/equifax-pay-575-million-part-settlement-ftc-cfpb-states-related-2017-data-breach

IBM. (2025). Cost of a data breach report 2025. https://www.ibm.com/reports/data-breach














