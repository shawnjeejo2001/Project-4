# Incident report analysis using the NIST cybersecurity framework


## Summary

### Identify
Today our network was down for 2 hours. The reason was that the network had been overloaded with ICMP packets coming. This is an ICMP flood attack that was used by the malicious actor. This is an example of DDoS attack since it came from multiple devices all at the same time. This attack was caused because of an unconfigured firewall that let the malicious actor carry out the attack. During the two hours normal internal network traffic could not access any network resources. All critical network resources needed
to be secured and restored to a functioning state.

### Protect
To protect the network, we would have to do a couple of things. We need a new configured firewall to control the amount of ICMP packets that goes to the server at a time. We could also have this firewall configured to do a source IP verification to check for spoofed IP addresses and to prevent IP spoofing.We could also install an IPS(Intrusion prevention software) that could detect and stop suspicious traffic from entering the internal network.
### Detect
The use of SIEM tools to log and analyze traffic could be useful. This way it is easier to detect when there’s unwanted traffic and it’s easier to stop it.Installing an IDS could also help detect unwanted traffic.
### Respond
The incident management team responded by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services.
### Recover
The team stopped more incoming ICMP and recovered the network back to normal.






