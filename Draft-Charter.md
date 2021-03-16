#### Charter of Working Group
##### MAC address is the Link Layer address used in IEEE 802 technologies. It is usually assigned statically for each network card by the Network Interface Card manufacturer and is used for forwarding and receiving frames.  The default static assignment of the MAC address raises privacy concerns and MAC address randomization is being implemented by end-device vendors. 

##### Currently, many use cases and applications make an implicit assumption of unique association between the device identity and its MAC address. This assumption is being used in both control plane and data plane. Device identity is important in scenarios where the network needs to know the device before offering services. Randomized and Changing MAC address (RCM) will break this assumption. This requires update of the current applications to function accross MAC address changes.  

##### The MADINAS working group will examine the effect of RCM schemes on network services. The group will examine which services continuity gets broken when the client MAC address changes. The group will also examine which identifiers (beyond the MAC address) are expected by network services.

##### For scenarios where session continuity is desirable, the group will recommend improvements to protect the exchange of identifiers between the client and the service source. For scenarios where privacy is paramount, the group will recommend best practices to ensure that the privacy achieved with RCM rotation is not damaged by the unprotected communication of other stable identifiers.

* Assess, define and publish the impacts of current use caess in various environments after introducing Randomized and Changing MAC address.

* Research existing mechanisms and analyze the needs to define a new consent-based mechanism to securely exchange identity between networks and user devices.

* Define the MADINAS problem statements.
