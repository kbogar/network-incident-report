# Incident report analysis

## Scenario

I am a cybersecurity analyst working for a multimedia company that offers web design services to small businesses, and I was tasked to create an incident report following the National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF). 

The company recently experienced a DDoS attack, compromising the internal network for two hours until resolved.
During the attack, the companys network services suddenly stopped responding due to an incoming flood of ICMP packets.
Normal internal network traffic could not access any network resources. 

The incident management team responded by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services.

The company`s cybersecurity team then investigated the security event. They found that a malicious actor had sent a flood of ICMP pings into the network through an unconfigured firewall. This vulnerability allowed the malicious attacker to overwhelm the network through a distributed denial of service (DDoS) attack.

To address this security event, the network security team implemented:
- A new firewall rule to limit the rate of incoming ICMP packets
- Source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets
- Network monitoring software to detect abnormal traffic patterns
- An IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics

<hr>

![](/docs/ira1.png)
![](/docs/ira2.png)