# DRAFT Agenda for IETF-109 BoF - MADINAS
MAC Address Device Identification for Network and Application Services

2 Hours

## Welcome & Agenda Review (BoF Chair)
- TBD

## Background - Problem Statement & Use Cases -- 10 Mins
- One presentation, 2-4 slides, link TBD - (Jason Weil and/or Yiu Lee)
## Background
- MAC address privacy (e.g., OUI, traceability, refer to IEEE privacy doc). MAC address is sending over clear text 
- How MAC address randomization addresses the privacy
- How MAC address randomization is implemented today
~~How residential network provider (both retailed and ISP) uses MAC addresses to provide services~~
~~How Community Wi-Fi and Hospitality network use MAC address to provide services~~
~~How Campus and Enterprise Wi-Fi networks use MAC address to provide services~~

### Use Cases -- 60 Mins
## Home Network Use Cases
Background: MAC address based Device Identity
- Use case for diagonstic and customer support (Simon, BT)
- Use case for Wi-Fi band and AP steering (Simon, BT)
- Use case to setup a server at home - (Yiu Lee, Comcast)
- Use case to protect DDoS mitigation - (Med, Orange)
- Use case for access controls / parental controls - (Charter)
- Use case for service policy based on device identity (Sky, TBD)

## Community Wi-Fi and Hospitality Use Cases
- Use case for auto-authentication for Open SSID (Comcast, Rajat)
- Use case for hotel, airplane and public facility (vendor)


## Enterprise Use Cases


### Problem Definition -- 10 Mins
- Overview of OS deployment of MAC Address randomization, 2 slides, link TBD - (Jason Weil and/or Yiu Lee)
##
- High-light the work in IEEE, WFA and BBF
- In the light of mac address randomation, the presented use cases may be impacted. This will create inconventience and unintended consequences for both users and operators.
- Seeking for guidelines and best practices for applications and services to behave better in the presence of mechanisms such as MAC address randomization.


## Discussion, Interest & Next Steps -- 30 Mins (BoF Chair w/AD Support)
- What other SSOs are working on this topic or related topics & how to best coordinate?
- Identify community of interest 
- Document all major use cases currently deployed
- Define best practices for enabling service continuity in the presence of MAC Address randomization
- Potentially define a method for service continuity in the presence of MAC Address randomization
- Whether the host OS shoud/must cooperate with the network
- Whether the applications hosted on the endpoint should/must be aware and whether they should/must cooperate with the network or end-to-end service
- Whether applications are sensitive to this MAC address randomization, ...
