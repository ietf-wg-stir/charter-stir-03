
# STIR Working Group Charter -- Revision 03

## Background and Problem Statement

The Secure Telephone Identity Revisited (STIR) Working Group specifies Internet-based mechanisms that allow verification of the authorization to use a particular telephone number through cryptographic authentication. These mechanisms are widely deployed in SIP-based telephony networks and are used to mitigate impersonation, spoofing, and other forms of unwanted or fraudulent communications.

Operational experience has revealed gaps in STIR's initial scope. Telephone numbers are assigned by service providers to entities that use those numbers across a broad range of calling and messaging scenarios, potentially through multiple software services or service providers acting on their behalf. While STIR provides delegate certificate mechanisms that support signing on behalf of such entities, it does not provide methods to uniquely identify those entities within credentials and signaling in a globally interoperable way. Furthermore, consumers increasingly encounter spoofed telephone numbers used as a trust signal across voice, messaging, email, and web interactions; the inability to authenticate telephone numbers consistently across these channels enables cross-channel fraud that exploits the assumed trustworthiness of a known number. Additionally, existing mechanisms do not provide transparency into credential issuance, leaving the ecosystem without a way to monitor and detect cases where unauthorized actors attempt to claim association with a telephone number. This rechartering extends the Working Group's scope to address these gaps while preserving compatibility with existing deployments.

## Scope of Work

The STIR Working Group will continue to specify and maintain the baseline protocols for cryptographic authentication of telephone calling party information using PASSporT and related mechanisms.

The Working Group will define protocol extensions that explicitly identify the entity holding the right to use an assigned telephone number as the responsible party for calls and messages originating from that number, including scenarios where communications are carried through multiple software services, service providers, or endpoints acting on that entity's behalf. Such extensions will require stable, globally unique identifiers to represent these authorized entities within credentials and signaling in a manner that supports interoperable verification across administrative boundaries, using existing Internet identifier mechanisms, such as domain names, consistent with established IETF practices.

The Working Group will consider extensions that enable verification of calling party information in scenarios where SIP signaling is not end-to-end, including extensions that support discovery of call processing services associated with telephone numbers.

The Working Group will also consider extensions that support the use of authenticated telephone identity in other real-time communications contexts, including messaging and application scenarios, to address cross-channel fraud in which spoofed telephone numbers are used as a trust signal across voice, messaging, email, and web interactions.

The Working Group will define certificate transparency mechanisms for telephone identity credentials that improve auditability and support detection of mis-issuance or misuse within the STIR ecosystem.

The Working Group will continue to leverage existing Internet security mechanisms, including PKI, and will coordinate with other IETF working groups as appropriate.

## Out of Scope

The following items are out of scope for the STIR Working Group:

- Definition of jurisdictional or legal policy topics, including vetting policies, regulatory requirements, governance, or authorization frameworks.
- Definition of governance requirements for numbering authorities, certificate authorities, or transparency services.
- Any mechanism requiring changes to circuit-switched telephony technologies.
