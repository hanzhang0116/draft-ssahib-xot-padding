--- 
title: Padding Considerations for DNS Zone Transfers-over-TLS
abbrev: Padding Considerations for XoT
docname: draft-ssahib-xot-padding
category: info

ipr: trust200902
area: General
workgroup: dprive
keyword: Internet-Draft

stand_alone: yes
pi: [toc, sortrefs, symrefs]

author:
    -
        ins: S. Sahib
        name: Shivan Sahib
        organization: Salesforce.com
        email: ssahib@salesforce.com
    -
        ins: H. Zhang
        name: Han Zhang
        organization: Salesforce.com
        email: hzhang@salesforce.com
    -
        ins: S. Dickinson
        name: Sara Dickinson
        organization: Sinodun IT
        email: sara@sinodun.com


normative:
  RFC2119:

  I-D.draft-ietf-dprive-xfr-over-tls:
    title: "DNS Zone Transfer-over-TLS"
    date: 2020
    author:
      - ins: W. Toorop
      - ins: S. Dickinson
      - ins: S. Sahib
      - ins: P. Aras
      - ins: A. Mankin
    target: https://datatracker.ietf.org/doc/draft-ietf-dprive-xfr-over-tls

informative:



--- abstract

{{I-D.draft-ietf-dprive-xfr-over-tls}} specifies use of TLS to prevent zone content collection via passive monitoring of zone transfers. This document lists considerations for various padding policies and provides recommendations.

--- middle

# Introduction

TODO


# Conventions and Definitions

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD",
"SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY", and "OPTIONAL" in this
document are to be interpreted as described in BCP 14 {{RFC2119}} {{!RFC8174}}
when, and only when, they appear in all capitals, as shown here.

# Padding for AXoT

As mentioned in {{I-D.draft-ietf-dprive-xfr-over-tls}}, the goal of padding AXoT responses would be two fold:

- to obfuscate the actual size of the transferred zone to minimize information leakage about the entire contents of the zone.
- to obfuscate the incremental changes to the zone between SOA updates to minimize information leakage about zone update activity and growth.


 

# Padding for IXoT


# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.



--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
