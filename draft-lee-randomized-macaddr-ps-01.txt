



Internet Engineering Task Force                            Y.L. Lee, Ed.
Internet-Draft                                                   Comcast
Intended status: Informational                              J. Weil, Ed.
Expires: 21 March 2021                            Charter Communications
                                                       17 September 2020


            Problem Statements for Mac-Address Randomization
                     draft-ietf-xml2rfc-template-06

Abstract

   Insert an abstract: MANDATORY.  This template is for creating an
   Internet Draft.

Status of This Memo

   This Internet-Draft is submitted in full conformance with the
   provisions of BCP 78 and BCP 79.

   Internet-Drafts are working documents of the Internet Engineering
   Task Force (IETF).  Note that other groups may also distribute
   working documents as Internet-Drafts.  The list of current Internet-
   Drafts is at https://datatracker.ietf.org/drafts/current/.

   Internet-Drafts are draft documents valid for a maximum of six months
   and may be updated, replaced, or obsoleted by other documents at any
   time.  It is inappropriate to use Internet-Drafts as reference
   material or to cite them other than as "work in progress."

   This Internet-Draft will expire on 21 March 2021.

Copyright Notice

   Copyright (c) 2020 IETF Trust and the persons identified as the
   document authors.  All rights reserved.

   This document is subject to BCP 78 and the IETF Trust's Legal
   Provisions Relating to IETF Documents (https://trustee.ietf.org/
   license-info) in effect on the date of publication of this document.
   Please review these documents carefully, as they describe your rights
   and restrictions with respect to this document.  Code Components
   extracted from this document must include Simplified BSD License text
   as described in Section 4.e of the Trust Legal Provisions and are
   provided without warranty as described in the Simplified BSD License.






Lee & Weil                Expires 21 March 2021                 [Page 1]

Internet-Draft              Abbreviated Title             September 2020


Table of Contents

   1.  Introduction  . . . . . . . . . . . . . . . . . . . . . . . .   2
     1.1.  Requirements Language . . . . . . . . . . . . . . . . . .   2
   2.  Problem Statement . . . . . . . . . . . . . . . . . . . . . .   2
   3.  IANA Considerations . . . . . . . . . . . . . . . . . . . . .   3
   4.  Security Considerations . . . . . . . . . . . . . . . . . . .   3
   5.  References  . . . . . . . . . . . . . . . . . . . . . . . . .   3
     5.1.  Normative References  . . . . . . . . . . . . . . . . . .   4
     5.2.  Informative References  . . . . . . . . . . . . . . . . .   4
   Appendix A.  Additional Stuff . . . . . . . . . . . . . . . . . .   4
   Authors' Addresses  . . . . . . . . . . . . . . . . . . . . . . .   4

1.  Introduction

   MAC-Address is the address that are being used for forwarding frames
   at Ethernet layer.  It is defined in IEEE 802.1.  MAC-Address is
   48-bit long and usually defined in the hardware.  Each Ethernet
   interface usually comes with a MAC-Address assigned by the
   manufacturer.  MAC-Address is used at the Local-Area-Network (LAN)
   for frame forwarding.  It is locally significant in the LAN and
   critical LAN-to-LAN communication.

   Major operating systems have implemented and deployed MAC-Address
   randomization to improve device and user privacy.  It is common
   practice on many types of networks today to use the MAC-Address as a
   form of device identification.  Some examples are LAN forwarding
   policy, sticky DHCP IP assignments, static NAT policy and MAC address
   ACL for blocking malicious or unwanted devices.  We are interested in
   determining if there is sufficient support in the IETF community to
   define best practices and potentially a new protocol for service
   continuity in the presence of MAC-Address randomization.

1.1.  Requirements Language

   The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT",
   "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this
   document are to be interpreted as described in RFC 2119 [RFC2119].

2.  Problem Statement

   Unlike IP Address that is usually dynamic assigned by the network,
   MAC-Address is statically assigned by the manufacturer.  Many
   networks today use MAC-Address to uniquely identify a device.  For
   example: Sticky DHCP assignment often maps to MAC-Address.  In
   additional, many local network policies such as port-forwarding, DMZ
   setup and LAN QoS are all based on MAC-Address.  There are also
   business policies that are making assumptions on MAC-Address.  For



Lee & Weil                Expires 21 March 2021                 [Page 2]

Internet-Draft              Abbreviated Title             September 2020


   example: Hospitality Internet service used in hotels, airplanes, and
   Community WiFi often uses MAC-Address to tie to Internet
   subscription.

   Recently, more and more privacy concerns are related to the static
   MAC-Address.  In particular, security community worries about people
   being able to tie the MAC-Address to a particular device.  This may
   enable device tracking and tracing.  Many modern Operation Systems
   such as Apple iOS, Google Android and Microsoft Windows 10 are
   experimenting to randomize MAC-Addresses.  The randomization policy
   could be time based, network based, commbination of both and more.
   This randomization will break many assumptions have been using for
   years.

   This document defines a set of problem statements to continue
   businesses when MAC-address is randomized.

   [PS-01] Internet Service Provider (ISP) must not make any assumption
   about the MAC-address

   [PS-02] ISP must not make any assumption of the Randomization Policy

   [PS-03] LAN policy must not tie to a fixed MAC-address

   [PS-04] A mechanism must be defined to securely identify a device.
   The mechanism can leverage existing protocols (e.g., EAP) or newly
   define protocol.

   [PS-05] ISP and device may leverage existing protocol or define a new
   mechanism to exchange information about MAC-address randomization

3.  IANA Considerations

   This memo includes no request to IANA.

   All drafts are required to have an IANA considerations section (see
   Guidelines for Writing an IANA Considerations Section in RFCs
   [RFC5226] for a guide).  If the draft does not require IANA to do
   anything, the section contains an explicit statement that this is the
   case (as above).  If there are no requirements for IANA, the section
   will be removed during conversion into an RFC by the RFC Editor.

4.  Security Considerations

   All drafts are required to have a security considerations section.
   See RFC 3552 [RFC3552] for a guide.

5.  References



Lee & Weil                Expires 21 March 2021                 [Page 3]

Internet-Draft              Abbreviated Title             September 2020


5.1.  Normative References

   [min_ref]  authSurName, authInitials., "Minimal Reference", 2006.

   [RFC2119]  Bradner, S., "Key words for use in RFCs to Indicate
              Requirement Levels", BCP 14, RFC 2119,
              DOI 10.17487/RFC2119, March 1997,
              <https://www.rfc-editor.org/info/rfc2119>.

5.2.  Informative References

   [DOMINATION]
              Mad Dominators, Inc., "Ultimate Plan for Taking Over the
              World", 1984, <http://www.example.com/dominator.html>.

   [RFC2629]  Rose, M., "Writing I-Ds and RFCs using XML", RFC 2629,
              DOI 10.17487/RFC2629, June 1999,
              <https://www.rfc-editor.org/info/rfc2629>.

   [RFC3552]  Rescorla, E. and B. Korver, "Guidelines for Writing RFC
              Text on Security Considerations", BCP 72, RFC 3552,
              DOI 10.17487/RFC3552, July 2003,
              <https://www.rfc-editor.org/info/rfc3552>.

   [RFC5226]  Narten, T. and H. Alvestrand, "Guidelines for Writing an
              IANA Considerations Section in RFCs", RFC 5226,
              DOI 10.17487/RFC5226, May 2008,
              <https://www.rfc-editor.org/info/rfc5226>.

Appendix A.  Additional Stuff

   This becomes an Appendix.

Authors' Addresses

   Yiu L. Lee (editor)
   Comcast
   Philadelphia, PA 19103
   United States of America

   Phone: +1 215 286 5894
   Email: yiu_lee@comcast.com









Lee & Weil                Expires 21 March 2021                 [Page 4]

Internet-Draft              Abbreviated Title             September 2020


   Jason Weil (editor)
   Charter Communications
   Orlando, FL
   United States of America

   Email: Jason.Weil@charter.com













































Lee & Weil                Expires 21 March 2021                 [Page 5]
