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

### Real-World Example

### Impact

### Mitigation Strategies

---

## IP Spoofing

### How It Works

### Real-World Example

### Impact

### Mitigation Strategies

---

## Conclusion

---

## References
