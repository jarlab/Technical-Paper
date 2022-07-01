# Firewalls
![Illustration of a firewall][[https://www.netstar.co.uk/wp-content/uploads/2014/05/Firewall.jpg | width=100px]]

## What is a firewall?
A firewall is a piece of software or a physical device which is used to protect us from threats on the internet. A firewall can be a software installed on your computer or a physical device that sits in between the internet and your network.

## Difference between software and physical firewall1. 
1. Since the software firewall is installed on a user's device, it consumes the resources of the host which may make the computer slower, while the physical firewall consumes resources of the separate physical device and won't make the user's computer slower.
2. A software firewall only protects a single user, whereas a physical firewall can protect an entire network.

## How do firewalls work?
Firewalls inspect all incoming and outgoing traffic and block the traffic originating from a harmful source, this is called stateful inspection. Firewalls also maintain an access list, which is basically a list of computers we are allowed to connect to and not to. Only if a packet belongs in the allowed list is it forwarded to its destination, thus this way of blocking harmful content is called packet filtering.

## Types of firewall
1. Packet filtering firewall - The firewall inspects a data packet's address header and matches them against an access control list, which then decides whether to allow the connection or not. This has a disadvantage as since it only checks the address header and not the payload, someone can hide malicious content in the payload from a trusted source and cause damage to our computer. While this is the quickest way to implement a firewall on your network since routers already come with this feature out of the box, you should only use it for a low risk environment because of the aforementioned vulnerability.
2. Application / Proxy firewall - This firewall sits between your network and the internet. It forwards any requests to the internet through itself, therefore not revealing our computer's IP address. It is better in terms of security than packet filtering firewall as proxy firewall also checks the payload/content of the data packet, though this comes at a price as it makes connection slower.
3. Hybrid firewall - This is the combination of packet filtering and proxy firewall where they are connected in series and provides the most security compared to the above methods therefore, it is used in scenarios where user data is extremely important e.g. hospitals.

## Limitations of firewall
1. A hacker can spoof the IP address and disguise themselves as originating from a trusted source thus, passing through our firewall undetected and spread malware. - If the attacker is on the same network as the user e.g. a public Wi-Fi then there is nothing to protect the user from an attack unless there is a software firewall installed on the user's device, therefore a physical firewall is unable to protect the user here.
2. Allowing an exception for different applications in software firewall rules can allow the attacker to send malware directly to the user's device if the trusted application itself has been compromised. Therefore, it is really important to install an antivirus program.

## Resources used
* TechTerms's Firewall video playlist https://www.youtube.com/watch?v=eO6QKDL3p1I&list=PLBbU9-SUUCwV7Dpk7GI8QDLu3w54TNAA6
* Firewall image from https://www.netstar.co.uk
