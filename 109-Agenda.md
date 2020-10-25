# DRAFT Agenda for IETF-109 BoF - MADINAS
MAC Address Device Identification for Network and Application Services

2 Hours

## Welcome & Agenda Review (BoF Chair)
- Juan Carlos Zuniga <j.c.zuniga@ieee.org>


## Background, Use Cases & Problem Statement -- 10 Mins
- One presentation, 2-4 slides, link TBD - (Jason Weil and/or Yiu Lee)

### Background
- MAC address privacy (e.g., OUI, traceability, refer to IEEE privacy doc). MAC address is sending over clear text 
- How MAC address randomization addresses the privacy
- How MAC address randomization is implemented today


## Use Cases -- 60 Mins
### Home Network Use Cases
Background: MAC address based Device Identity
- Use case for diagonstic and customer support (Simon Ringland, BT)
- Use case for Wi-Fi band and AP steering (Simon Ringland, BT)
- Use case to setup a server at home - (Yiu Lee, Comcast)
- Use case to protect DDoS mitigation - (Med, Orange)
- Use case for access controls / parental controls - (Charter)
- Use case for service policy based on device identity (Plume)

### Community Wi-Fi and Hospitality Use Cases
- Use case for auto-authentication for Open SSID (Comcast, Rajat)
- Use case for UE mobility in Wi-Fi (Ajay, Benu Networks)
- Use case for DHCP Table Exhaustion (ComScope, Eli)

### Cloud Management
- Use case for resource management when mac-address is randomized (Plume)


## Problem Statement -- 10 Mins
- Overview of OS deployment of MAC Address randomization, 2 slides, link TBD - (Jason Weil and/or Yiu Lee)
- High-light the work in IEEE, WBA, WFA and BBF
- In the light of mac address randomation, the presented use cases may be impacted. This will create inconventience and unintended consequences for both users and operators.
- Seeking for recommendations and best practices for OS, applications and services to behave better in the presence of mechanisms such as MAC address randomization.


## Discussion, Interest & Next Steps -- 30 Mins (BoF Chair w/AD Support)
- What other SSOs are working on this topic or related topics & how to best coordinate?
- Identify community of interest 
- Document all major use cases currently deployed
- Define best practices for enabling service continuity in the presence of MAC Address randomization
- Potentially define a method for service continuity in the presence of MAC Address randomization
- Whether the host OS shoud/must cooperate with the network
- Whether the applications hosted on the endpoint should/must be aware and whether they should/must cooperate with the network or end-to-end service
- Whether applications are sensitive to this MAC address randomization, ...
- How frequenetly randomize the mac-address will have major impact to the system design and resource management
- For enterprise Wi-Fi network, it is the users to authenticate themselves to the network. Is there a way for the network to present an identity and in-exchange the network can request some sticky information that can offer enhance services. 
- Define a way for the device to communicate to the network about the mac addreess charcteristics (e.g., semi-persisent, random, etc)
