
# STIR Working Group Charter -- Revision 03

## Background and Problem Statement

The Secure Telephone Identity Revisited (STIR) Working Group specifies Internet-based mechanisms that allow verification of the authorization to use a particular telephone number through cryptographic authentication. These mechanisms are widely deployed in SIP-based telephony networks and are used to mitigate impersonation, spoofing, and other forms of unwanted or fraudulent communications.

Operational experience has revealed that while STIR effectively authenticates the event of a call and the authorization to use a telephone number, it does not provide a means to identify the entity behind that authorization. Telephone numbers are assigned to entities that may use them through multiple services or providers acting on their behalf, and verifiers have no standardized way to determine which entity a delegate certificate represents. Additionally, existing mechanisms do not provide transparency into credential issuance. This rechartering extends the Working Group's scope to address these gaps while preserving compatibility with existing deployments and the STIR trust model.

## Scope of Work

The STIR Working Group will continue to specify and maintain the baseline protocols for cryptographic authentication of telephone calling party information using PASSporT and related mechanisms.

The Working Group will define a means to associate a PASSporT with an identifier representing the entity holding the right to use an assigned telephone number. This is expected to take the form of a new PASSporT claim whose value carries the entity identifier; the form of that value (for example, a URI, string, or structured object) and how it is bound to STIR credentials and the delegation model are matters for the Working Group to determine.

The Working Group will define certificate transparency mechanisms for telephone identity credentials that improve auditability and support detection of mis-issuance within the STIR ecosystem.

The Working Group will extend existing out-of-band mechanisms to support discovery of STIR credentials and services associated with telephone numbers, including the application of connected identity in scenarios where SIP signaling is not end-to-end. The Working Group will consider extensions that support the use of authenticated telephone identity in other communications contexts, including messaging.

The Working Group will continue to leverage existing Internet security mechanisms, including PKI, and will coordinate with other IETF working groups as appropriate.

## Out of Scope

The following items are out of scope for the STIR Working Group:

- Definition of jurisdictional or legal policy topics, including vetting policies, regulatory requirements, governance, or authorization frameworks.
- Definition of governance requirements for numbering authorities, certificate authorities, or transparency services.
- Any mechanism requiring changes to circuit-switched telephony technologies.
