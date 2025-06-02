# Securing the Perimeter![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.001.png)
### *Siddh Samarth![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.002.png)*
Securing the Perimeter: Beca*C*suese*B*emBt*S*itocto*-*hin*0*inskd*9*soon*2*!’t grow on trees, but hackers
## ***Project Information Slide![ref1]***
# How to Use this Template
- We have provided these slides as a guide to ensure you submit all the required components to complete your project successfully.
- When presenting your project, remember that these slides are merely a guide. We strongly encourage you to embrace your creative freedom and make changes that reflect your unique vision as long as the required information is present.
- You can add slides to the template when your answers or screenshots do not fit on the previously provided pages.
- Delete this and all other project instruction slides before submitting your project.
- **Remember to add your name and the date to the cover page.**
# Project Scenario![ref2]
## ***Project Information Slide![ref1]***
# ![ref3] Overview
XYZ is the premier cryptocurrency exchange. They transact over a billion trades everyday and are considered to be one of the most reliable and secure exchanges in the world. Due to their rapid growth, they've faced challenges in scaling their security posture.

The largest challenge they've faced is with their Perimeter Network Security being secure. The networking team was overburdened with the rapid growth and a majority of the network infrastructure was built insecurely.

Due to a lack of visibility and a lack of proper access control setup on the network, it was inevitable that a breach took place! XYZ was hit with a massive attack in which their network was breached and their internal servers were compromised resulting in over 500 Bitcoin being stolen!

Needing to get the bottom of this breach and resolving their current perimeter issues they've contracted you from SecureCorp, a world renowned cybersecurity consulting firm.
# Section 1:![ref2]
Designing a secure Network Architecture
## ***Project Information Slide![ref1]***
# ![ref3] Network Description
*Download the[ drawio.com](http://drawio.com/) file [from here.*](https://drive.google.com/file/d/1TDzbbcS_14MjAmrovcn2rp41ldFJribH/view?usp=sharing)*

![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.006.png)

- *The on-premise network is connected to a virtual network through the internet.*
- *All five servers are located within a single virtual network and in one subnet.*
- *All servers have direct connections to the internet.*
- *The two web servers are required to communicate with the two database servers to function correctly.*
- *The file storage server only needs to be accessible from the on-premise network.*
## ***Project Information Slide![ref1]***
# ![ref3] Identify Network Vulnerabilities
In your initial assessment of the company's network, it's essential to pinpoint specific vulnerabilities that could be exploited by malicious actors. Identifying these weaknesses is the first step in reinforcing the network's defenses.

- *Review the provided network diagram*
- *Identify three major security problems with the current network setup*
- *Describe each identified problem and explain how it poses a risk to the network*
## ***Project Information Slide![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.007.png)***
Ide ntify Ne tw ork Vulne ra bilitie s

XYZ’s network was so open that it practically handed out free passes to hackers. Result? 500 Bitcoins poofed into thin air! Talk about an expensive oops moment.

1. **No Proper Segmentation for the Network ![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.008.png)**

All servers are in one big happy family... until a hacker joins the reunion!

**Problem**: All servers are in the same subnet leaving no safety and security between public and private resources.

**Risk**: If any of the server is compromised , gaining lateral access and east-west navigation becomes a lot easier.

2. **Direct Exposure to the internet**

Every server has a direct internet connection—because who needs doors when you can have wide-open windows?

**Problem**: Each server has a direct connection to the internet ,making it very vulnerable to external attacks.

**Risk**: The lack of proper perimeter defense allows attackers to attack individual servers increasing the attack surface

||
| :- |
||
||
|***Project Information Slide***|
||
|<p>**3. Unrestricted Traffic to and fro for the File Storage Server**</p><p>The file storage server is a free-for-all buffet for hackers. Talk about serving data on a silver platter!</p>|
|<p>**Problem:**The file storage server should have network traffic regulators and should only be accessible from the on-premises network. </p><p>**Risk:** High risk of data breaches because unauthorized users can gain access to the server.</p>|

![ref3]
## ***Project Information Slide![ref1]***
# ![ref3] Network Redesign
With the vulnerabilities identified, it’s time to rearchitect the network. A well-structured network with proper security controls is vital for defending the company's digital assets.

- Use [drawio.com](http://drawio.com/) to create the updated[ ](https://drive.google.com/file/d/1TDzbbcS_14MjAmrovcn2rp41ldFJribH/view?usp=sharing)diagram. You can download the original diagram from[ here](https://drive.google.com/file/d/1TDzbbcS_14MjAmrovcn2rp41ldFJribH/view?usp=sharing).
  - *Update the network diagram to include:*
    - *Network segmentation separating public-facing services from internal services.*
      - *Placement of firewalls to control and filter traffic*
      - *A secure, encrypted connection method for the on-premise network to access the file storage server.*
  - *Ensure the updated diagram reflects these additions clearly.*
# Network Redesign
Think of firewalls as bouncers at a VIP club—no entry ![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.009.jpeg)![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.010.png)![ref3]without approval!

![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.011.png) We’re separating the servers like quarrelsome siblings—web servers in

one room, databases in another, and no peeking!"

VPN: Because a little      ![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.012.png)encryption never hurt anyone (except hackers).
## ***Project Information Slide![ref1]***
# ![ref3] Convince the Stakeholders
With a proposed network redesign, stakeholders will require a clear understanding of the benefits and necessity of these changes. Your next task is to prepare answers to the following potential questions they may have. In all your answers, make sure to emphasize the security aspects.

- Why do we need to add firewalls to our network?
- What is the benefit of having different areas in our network for web servers and database servers?
- What does a VPN do for our connection to the file storage server?
# ***Project Information Slide![ref1]***
**Why do we need to add firewalls to our network?![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.013.png)![ref3]**

Firewalls are like medieval castle walls—minus the moats and alligators, but just as effective.

Firewalls act as a barrier between trusted internal networks and untrusted external networks (like the internet). They filter incoming and outgoing traffic based on security rules, preventing malicious traffic from reaching critical systems.

By deploying firewalls, we can:

- Block unauthorized access: Only allow specific services or IP

ranges to connect to our      servers.

- Detect anomalies: Log suspicious traffic patterns for further

analysis.

- Minimize attack surface: Reduce exposure by restricting

unnecessary access to sensitive resources.

Firewalls are like medieval castle walls—minus the moats and alligators, but just as effective.

**What is the benefit of having different areas in our network for web servers and database servers?**

Think of it as building lanes on a highway: you don’t want trucks driving in the bike lane, right?

Separating web servers and database servers into different zones (public and private) ensures that public-facing servers cannot directly access sensitive internal resources.

Benefits include:

- Improved security: Even if a web server is compromised,

attackers cannot access the database directly.

- Compliance: This design aligns with industry standards like

PCI-DSS and GDPR, which mandate strict access controls.

- Better performance: Reduced traffic between zones minimizes

bottlenecks and resource contention.

||
| :- |
||
||
||
|***Project Information Slide***|
||
|**What does a VPN do for our connection to the file storage server?**|
|<p>VPN is like a private tunnel—no one sees what’s inside, not even the nosy neighbor.</p><p>A VPN (Virtual Private Network) establishes a secure, encrypted connection between the on-premises network and the file storage server. **Advantages**:</p><p>**Encryption**: Data transmitted over the VPN is encrypted, making it unreadable to attackers.</p><p>**Access control**: Only authorized users with VPN credentials can access the file storage server.</p><p>**Reduced exposure**: The file storage server is no longer directly accessible over the internet.</p>|

![ref3]
# Section 2:![ref2]
Building a secure Network Architecture in VirtualBox
## ***Project Information Slide![ref1]***
# ![ref3] Network Setup
Following the favorable reception of your network diagram, management is keen to see this blueprint come to life in a test environment. They have chosen VirtualBox as the platform to host this venture into the cloud. Your next task is to build the test network, which is detailed below. 

- *Construct two VirtualBox virtual networks (VNet):*
  - *Name the first VNet DMZ. Within it, create two subnets:*
    - *Public-DMZ for future web servers.*
    - *Private-DMZ for database servers.*
  - *Name the second VNet Internal and create one subnet within it called Internal-Subnet.*
- *Take and submit a screenshot of the DMZ Virtual Network with the two subnets*
- *Take and submit a screenshot of the Internal Virtual Network with the subnet*
## ***Project Information Slide![ref1]***
# ![ref3] Network Setup
*Screenshot of the DMZ Virtual Network with the two subnets*

![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.014.png)

![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.015.png)
# Section 3:![ref2]
Continuous Monitoring with a SIEM
## ***Project Information Slide![ref1]***
# ![ref3] Understanding SIEM Benefits
As cyber threats evolve, staying ahead with proactive monitoring is crucial. It's time to get everyone on board with adding a SIEM system to the network. Your task is simple but crucial: convince the stakeholders by pinpointing three major benefits of implementing a SIEM. 

- Identify at least 3 distinct benefits of implementing a SIEM in an enterprise environment
- Write a short description of each benefit 

***Project Information Slide![ref1]***
# ![ref3] Understanding SIEM Benefits


|1\.**Centralized Logging**|
| - |
|<p>- SIEM consolidates logs from all devices (servers, firewalls, endpoints) into a single system, making it easier to detect and investigate suspicious activities.</p><p>- Example: If multiple failed login attempts occur on different servers, SIEM will flag it as a potential brute force attack.</p>|
|**2. Real Time Threat Detection**|
|<p>Imagine a security guard who never blinks and doesn’t need coffee breaks. That’s SIEM!"</p><p>- A SIEM continuously monitors events and triggers alerts for unusual behavior, such as unauthorized access or data exfiltration.</p><p>- Example: An alert is generated if someone tries to download sensitive files outside business hours.</p>|
|**3. Compliance and reporting**|
|<p>SIEM: Making audits less painful, one preconfigured report at a time.</p><p>- SIEM simplifies compliance by providing built-in reports for standards like ISO 27001, GDPR, and HIPAA. It also helps maintain audit trails for forensic investigations.</p><p>- Example: A preconfigured GDPR report can be generated to demonstrate compliance during audits.</p>|
||
## ***Project Information Slide![ref1]***
# ![ref3] Deploy SIEM Components in VirtualBox
To give management a tangible understanding of how a Security Information and Event Management (SIEM) system operates, we're going to set up a demonstration in our VirtualBox test environment. This setup will involve deploying a virtual machine for the ELK server within the private subnet and a virtual machine for Filebeat within the public subnet. These components will work in tandem to illustrate the power of centralized logging and real-time analysis.

- *Deploy a virtual machine named Elk-Server in the Private- DMZ subnet of the DMZ VNet for the ELK stack.*
- *Deploy a virtual machine named Filebeat-VM in the Public-*

  *DMZ subnet of the DMZ VNet for Filebeat.*

- *Take and submit screenshots of the VM instances confirming their creation and network placement.*
## ***Project Information Slide![ref1]***
# ![ref3] Deploy SIEM Components in VirtualBox
[Add Screenshot here]![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.016.png)
## ***Project Information Slide![ref1]***
# ![ref3] Setup Monitoring
To fully showcase our SIEM's capabilities, we will set up the ELK (Elasticsearch, Logstash, Kibana) server, install Filebeat on our web server, and ensure that web server logs are correctly forwarded and displayed in Kibana. This comprehensive task is pivotal for demonstrating effective real-time monitoring and analysis of web server activity, which is essential for maintaining operational health and security within our infrastructure.

- *Install and configure the ELK server on a VM within the Private-DMZ subnet.*
- *Install Filebeat on the web server in the Public-DMZ subnet.*
- *Configure Filebeat to forward logs to the ELK server's Elasticsearch.*
- *Generate traffic on the web server to create log data (i.e. access the server).*
- *Verify logs are forwarded to Elasticsearch and visible in Kibana.*
- *Create screenshots to confirm that the services are running:*
  - *Filebeat service running on the web server* 
    - *Make it from the CLI, with the ‘systemctl status filebeat’*

*Kib i l f h Fil b h*
## ***Project Information Slide![ref1]***
# ![ref3] Setup Monitoring
*Screenshot of the Filebeat service on the web server (command: ‘systemctl status filebeat’)![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.017.jpeg)*

*.*

[Add Screenshot here]
## ***Project Information Slide![ref1]***
# ![ref3] Setup Monitoring
*Screenshot showing that Kibana receives logs from the Filebeat host (SIEM/Hosts/Filebeat-VM)![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.018.png)*

[Add Screenshot here]
# Section 4:![ref2]
Zero Trust
## ***Project Information Slide![ref1]***
# ![ref3] Zero Trust Comparison
Following a significant security breach at XYZ, the necessity to reassess and strengthen our network security architecture is paramount. A comparison between the emerging Zero Trust architecture and traditional network security models will highlight the potential enhancements Zero Trust can offer. Your task involves selecting three key principles from Zero Trust architecture, comparing them to traditional models, and evaluating the benefits of Zero Trust. This analysis is crucial for guiding XYZ towards a more resilient cybersecurity framework.

- Select three principles of Zero Trust architecture (you can find them in the classroom and in the next page)
- Compare each selected principle to its counterpart in traditional network security models, focusing on:
  - Differences in approach
  - Potential benefits of Zero Trust over traditional methods
## ***Project Information Slide![ref1]***
# ![ref3] Zero Trust Principles
Select three principles to use in the comparison:

- Consideration of all resources: Every device, software, and system is a potential security vector.
- Secured communication: Encrypt all data transfers, irrespective of location.
- Per-session access: Grant access to resources only for the duration of a session.
- Dynamic access policy: Access is based on real-time evaluations of multiple factors.
- Continuous monitoring: Real-time assessment of asset integrity and security.
- Dynamic authentication: Ongoing verification before allowing access.
- Extensive data collection: Gather detailed information for security enhancement.

***Project Information Slide![ref1]***
# ![ref3] Zero Trust Comparison
1. **Per-Session Access![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.019.png)**

**Zero Trust**: Access is granted only for the **Traditional Approach:** Access is often duration of a session. persisted once granted

**Benefits of Zero Trust:** Minimizes the risk of unauthorized access due to stolen credentials.

2. **Secured Communication![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.020.png)**

**Zero Trust Approach:** Encrypts all data **Traditional Approach:** Focuses on perimeter transfers, irrespective of location. encryption.

**Benefits of Zero Trust:**  Protects data even if intercepted

***Project Information Slide![ref1]***
# ![ref3] Zero Trust Comparison
3. **Continuous Monitoring![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.021.png)**

**Zero Trust Approach:** Real-time evaluation of

asset integrity. **Traditional Approach:** Periodic checks.

**Benefits of Zero Trust:** Early detection of compromises.
## ***Project Information Slide![ref1]***
# ![ref3] The Zero Trust Model
Following your analysis of Zero Trust versus traditional security models, it’s clear that a Zero Trust framework is essential for enhancing XYZ's network security. The challenge now shifts to selecting the most appropriate Zero Trust model for XYZ from three distinct options: Device Agent & Gateway, Enclave Gateway, or Resource Portal. This selection is critical, as it must align with the unique challenges and goals of the company. Your task is to make an informed choice and articulate why this model stands out as the best fit for XYZ, considering their need for a robust response to recent security vulnerabilities.

- Choose one Zero Trust model for XYZ from the following options:
  - Device Agent & Gateway
  - Enclave Gateway
    - Resource Portal
- Justify why the selected model is the best fit for XYZ’s current network challenges and security objectives.
## ***Project Information Slide![ref1]***
# ![ref3] Zero Trust Model
Device Agent & Gateway![](Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.022.png)

Allows real-time access control for individual devices. Ideal for environments with a mix of on-premises and remote access needs.

Reduces the risk of insider threats by verifying device integrity.

***Conclusion***

***By addressing XYZ’s vulnerabilities, redesigning the network,     implementing SIEM, and transitioning to Zero Trust, we ensure a secure, scalable infrastructure ready for future challenges.      Remember, cybersecurity isn’t just about building walls; it’s      about smartly managing the doors, windows, and secret tunnels too.***

[ref1]: Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.003.png
[ref2]: Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.004.png
[ref3]: Aspose.Words.f3b1576e-6227-412a-920f-a34794e1a96e.005.png
