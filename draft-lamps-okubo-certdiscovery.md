---
title: "A Mechanism for X.509 Certificate Discovery"
abbrev: "TODO - Abbreviation"
category: std

docname: draft-lamps-okubo-certdiscovery-latest
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"
number:
date:
consensus: true
v: 3
# area: AREA
# workgroup: WG Working Group
keyword:
 - next generation
 - unicorn
 - sparkling distributed ledger
venue:
#  group: WG
#  type: Working Group
#  mail: WG@example.com
#  arch: https://example.com/WG
  github: "tomofumiokubo/certificatediscovery"
  latest: "https://tomofumiokubo.github.io/certificatediscovery/draft-lamps-okubo-certdiscovery.html"

author:
 -
    fullname: T. Okubo
    organization: DigiCert, Inc.
    email: tomofumi.okubo+ietf@gmail.com

 -
    fullname: C. Bonnell
    organization: DigiCert, Inc.
    email: corey.bonnell@digicert.com

 -
    fullname: J. Gray
    organization: Entrust
    email: john.gray@entrust.com

normative:

informative:


--- abstract

This document specifies a method to discover a secondary X.509 certificate associated with an X.509 certificate to enable efficient multi-certificate handling in protocols. The objective is threefold: to enhance cryptographic agility, improve operational availability, and accommodate multi-key/certificate usage. The proposed method aims to maximize compatibility with existing systems and is designed to be legacy-friendly, making it suitable for environments with a mix of legacy and new implementations. It includes mechanisms to provide information about the target certificate's signature algorithm, public key algorithm and the location of the secondary X.509 certificate, empowering relying parties to make informed decisions on whether or not to fetch the secondary certificate.

The primary motivation for this method is to address the limitations of traditional certificate management approaches, which often lack flexibility, scalability, and seamless update capabilities. By leveraging this mechanism, subscribers can achieve cryptographic agility by facilitating the transition between different algorithms or X.509 certificate types. Operational redundancy is enhanced by enabling the use of backup certificates and minimizing the impact of primary certificate expiration or CA infrastructure failures.

The approach ensures backward compatibility with existing systems and leverages established mechanisms, such as the subjectInfoAccess extension, to enable seamless integration. It does not focus on identity assurance between the primary and secondary certificates, deferring such considerations to complementary mechanisms.


--- middle

# Introduction

TODO Introduction


# Conventions and Definitions

{::boilerplate bcp14-tagged}


# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
