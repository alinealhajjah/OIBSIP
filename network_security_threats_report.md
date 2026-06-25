# Common Network Security Threats

## Introduction

Today's world relies heavily on the internet, whether it's for our daily lives or business. Everything exists and has a digital footprint on the internet. That is why internet security and cybersecurity are important. The excessive use of the internet has made us vulnerable by having our PII or SPII stored in it by organizations. Cyber attacks happen every single day, and it is crucial to learn about them. In order to protect valuable information, we have to study those attacks. Organizations should also carry the responsibility of maintaining a strong security posture in order to ensure business continuity, gain customer trust, and keep a good reputation. Having security controls and safety measures will ensure customer safety and the continuity of a business, and both parties remain happy. There are many types of threats, and all organizations should analyze the threat, protect their systems, and respond effectively.

---

## DoS/DDoS Attacks

### How It Works

Denial of Service Attack (DoS) is when legitimate users are no longer able to access information, systems, devices, or other networks. This attack works by targeting the availability of resources to users. Simply, it is carried out with a large number of systems attacking a specific victim. Threat actors flood the network with a huge amount of service requests that are illegitimate or have a fabricated return address. It exhausts the network's bandwidth. As a result of this traffic, the receiver crashes, preventing access to users.

#### Examples

##### Smurf Attack

The attacker sends Internet Control Message Protocol (ICMP) broadcast packets to multiple hosts while spoofing the victim's IP address. The hosts respond to the victim, flooding it with traffic and overwhelming its resources.

##### TCP SYN Flood

The above-described method works by consuming bandwidth space, whereas this attack aims at exploiting server CPU memory. Whenever a host attempts to connect to a server, a three-way handshake protocol is established before any actual data transfer occurs. Firstly, the host sends a SYN packet to initiate the handshake. The server then replies with an acknowledgement packet. At last, the host needs to send a ACK packet to establish a successful connection. However, attackers leave the handshake half-open by not sending the final SYN-ACK. Such a half-open state is stored in the server's memory, and the server keeps waiting for the host to send the final packet. When thousands of such half-open connections are initiated, the server runs out of memory and crashes. It will not be able to serve legitimate clients, as its memory is filled with forged packets.



Distributed Denial of Service Attack (DDoS) is when a threat actor exploits a weakness or a vulnerability in a group of interconnected servers to carry out large-scale attacks. This works by installing command-and-control software. After taking control of the infected devices, which are now called botnets or zombies, attackers send an escalating amount of service requests or traffic to the victim. They could use software exploitations such as buffer overflow, dangling pointers, code injection, etc. DDoS attacks have a large magnitude because many IoT devices are vulnerable because they often have weak default passwords, outdated firmware, or limited security controls.        


### Real-World Example

One of the most famous attacks was in year 2000, February 7 when yahoo servers were crashed. Yahoo was unavailable for several hours which had a lot of negative impact on its business. Buy. Com, e-bay and CNN were the other giant companies that were attacked, the very next day after yahoo. Since E-bay is an e-commerce marketplace and takes millions of transactions daily shutting down for several hours made a huge loss to the company.


Another famous DDoS attack occurred on September 20, 2016, when cybersecurity journalist Brian Krebs was targeted by a massive attack exceeding 620 gigabits per second (Gbps). The attack was carried out using the Mirai botnet, which continuously scanned the Internet for vulnerable IoT devices and used them to generate malicious traffic.

### Impact

* Service outages and downtime
* Financial losses due to interrupted operations
* Reputational damage and loss of customer trust
* Reduced productivity and business continuity issues
* Increased operational and recovery costs

### Mitigation Strategies

#### 1. Traffic Filtering and Scrubbing

Organizations can work with Internet Service Providers (ISPs), Content Delivery Networks (CDNs), or specialized DDoS mitigation providers to identify and filter malicious traffic before it reaches the target system.

#### 2. Access Control Lists (ACLs)

Access Control Lists (ACLs) are sets of rules used on network devices such as routers and firewalls to control network traffic. They help block unwanted traffic based on predefined criteria, reducing exposure to attack traffic.

#### 3. Rate Limiting and Load Balancing

Rate limiting restricts the number of requests a user can send within a specific period, while load balancing distributes traffic across multiple servers. Together, these controls help prevent resource exhaustion and improve availability during attacks.

---

## Man-in-the-Middle (MITM)

### How It Works

Man in the middle (MitM) attack targets the integrity and confidentiality. The attacker intercepts and alter the data  between two entities involved in communication association . This means that data is no longer authentic and reliable and an lawful hacker can access it.
For example hackers may alter victims domain name system (DNS) so when the victim types a web address, they are redirected to harmful locations controlled by the attacker. They could also manipulate victims DNS to intercept user credentials .
There a possibility that this attack could work on two or more network  devices this supports acts like network sniffing , transmitted data manipulation. Exploitation for credential access.

### Real-World Example

Peter Burkholder (2002) analyzed a real-world example of a Man-in-the-Middle attack against SSL/TLS connections. He described how Dug Song’s tool _webmitm_ demonstrated that attackers could transparently intercept encrypted traffic when clients failed to properly validate certificates. The problem was that browsers like Microsoft Internet Explorer would accept any certificate signed by a trusted Certificate Authority, even if it was not issued to the actual server being visited. This allowed an attacker to impersonate a legitimate site, capture sensitive data, and relay traffic without the user realizing.
Burkholder explained that Dug Song solved the demonstration by exploiting this weakness: he set up _webmitm_ to act as a proxy, presenting a valid but misleading certificate to the client. Because the browser trusted the certificate, the user’s traffic flowed through the attacker’s system, giving full visibility and control.
The mitigation technique Burkholder emphasized was strict SSL/TLS client configuration and certificate validation. He argued that users and administrators must enforce proper certificate checking, reject mismatched or suspicious certificates, and educate users not to ignore browser warnings. By ensuring that clients verify the authenticity of certificates, the attack could be prevented, closing the gap that allowed _webmitm_ to succeed.


### Impact

**Intercept communicated data**
    - A MitM attacker positions themselves between two communicating parties and can intercept data traveling between them. This allows the attacker to gain unauthorized access to sensitive information.
- **Alter data traveling between communicating parties**
    - The attacker can modify messages in transit without the knowledge of either party, potentially changing the content or meaning of the communication.
- **Masquerade as one or more entities involved in a communication association**
    - NIST describes MitM as an active wiretapping attack in which the attacker can masquerade as one or more legitimate entities, causing both parties to trust the malicious intermediary.
- **Compromise authentication processes**
    - In authentication scenarios, the attacker may position themselves between the claimant and verifier, or between a subscriber and a Credential Service Provider (CSP), enabling interception or manipulation of authentication data.


### Mitigation Strategies

**Mutual authentication**
     NIST authentication guidance emphasizes verifying the identities of both communicating parties, reducing the likelihood that an attacker can successfully position themselves between them.

     
**Transport Layer Security (TLS)**
    - Using TLS provides confidentiality and integrity protection for communications, making it more difficult for attackers to intercept and modify data in transit.

    
**Message Authentication Codes (MACs)**
    - NIST defines a MAC as a cryptographic checksum that detects both accidental and intentional modifications of data, providing authenticity and integrity    protection.

    
**Cryptographic integrity protection**
    - Applying cryptographic mechanisms to verify message integrity helps detect unauthorized modifications made by a MitM attacker.
**Strong authenticator binding**
    - NIST recommends secure authenticator binding between subscribers and Credential Service Providers to reduce opportunities for MitM attacks during enrollment and authentication processes.

---

## IP Spoofing

### How It Works

IP spoofing is when a threat actor create IP packets using a false IP address. Then attackers manipulate the source address in the packet header so that the victim believes the packet originated from a different system . This allows the attacker to impersonate another computing systems. IP spoofing exploits the fact that the Internet Protocol does not inherently verify whether the source IP address in a packet is  authentic. Attackers frequently employ IP spoofing in Distributed Denial-of-Service (DDoS) attacks, where spoofed addresses help obscure the true origin of the attack and complicate mitigation efforts. It can also support other attacks, including man-in-the-middle attacks and attempts to bypass IP-based trust relationships. This characteristic makes it well suited for large-scale flooding and increasing the magnitude of  attacks. 
### Real-World Example

### Impact

### Mitigation Strategies

---

## Conclusion

---

## References
