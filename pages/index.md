---
layout: default
title: Introduction to PIV Guides
permalink: /
---

Welcome to the **Personal Identity Verification** (PIV) Guides! On these pages you will find information on how to implement common PIV configurations at your organization.  These guides are [open source](https://github.com/gsa/piv-guides) and a _work in progress_ and we [welcome contributions]({{ site.baseurl }}/contribute/) from our colleagues.

The guides focus on using PIV credentials for _logical access_ such as authenticating to networks or applications, or digitally signing and encrypting.  Using PIV for _physical access_ will be covered under another section of guides.

The information on this page provides introductory information.

1. [What is PIV?](#what-is-piv)
1. [Why is PIV usage important?](#why-is-piv-usage-important)
1. [What systems should use PIV?](#what-systems-should-use-piv)
1. [What is in the PIV Guides?](#what-is-in-the-piv-guides)
1. [Where can I find the Standards?](#where-can-i-find-the-standards)

#### What is PIV?

A Personal Identity Verification (PIV) credential is a US Federal government-wide credential used to access Federally controlled facilities and information systems at the appropriate security level.

PIV credentials have certificates and key pairs, pin numbers, biometrics like fingerprints and pictures, and other unique identifiers.  When put together into a PIV credential, we have the capabilities to implement multi-factor authentication for networks, applications and buildings.

#### Why is PIV usage important?

Enabling systems and facilities to use PIV credentials for authentication greatly enhances the security stance of an organization. PIV credentials allow for a high level of assurance in the individuals that access your resources, as they are only issued by trusted providers to individuals that have been verified in person.  The PIV credentials are highly resistant to identity fraud, tampering, counterfeiting, and exploitation.

PIV credentials are _standardized_ as well.  PIV credentials might be issued by different organizations using different commercial or open source products, on different form factors (cards, mobile devices, etc).  However, the PIV credentials are standardized - every PIV credential is required to have specific information, using technology which is _interoperable_.

Your PIV credential from one agency will have the same basic required format, information and technology as a PIV credential from your partner agencies. This allows us to trust each other, share applications, and architect and implement systems using common patterns for authentication.

#### What systems should use PIV?

Any system at your organization that requires heightened security for determining who should gain access can and should use PIV for authentication.  While PIV credentials can be used for authentication on almost any system, they are especially useful for systems that protect sensitive information.

* PIV should be used for all authentication for all _privileged_ users.  This includes authentication to servers, networks, and applications.
* PIV should be used for all _network_ authentication for _all_ users.
* PIV should be used for all application authentication for _all_ users of an application that protects or contains sensitive information.
* PIV should be used for access to facilities and buildings.


#### What is in the PIV guides?

First, we cover the basics of PIV credentials including:

1. What PIV is, contains and looks like
1. The basics of getting started with PIV credentials
1. Using PIV for network authentication (smartcard logon)

We also have sections for Applications, Developer Guides and User Guides.  All these guides need your contributions.  We want you to contribute and share lessons learned when configuring systems or applications, tuning considerations, **code**, common challenges, troubleshooting errors, and any information you think is helpful for your colleagues.  

#### Where can I find the Standards?

If you are interested in PIV credentials or working on _using_ PIV credentials, you should review pages on this site and other online resources.

If you are really interested in the bits and bytes of PIV credentials, you can review the Standards. The Standards are best to review if you develop products such as hardware or software that are _specific_ to PIV credentials for the US Federal Government.  However, for most users and engineers, the Standards may seem overwhelming and will be too detailed for your needs.

To review the Standards, there is a [NIST website](http://csrc.nist.gov/groups/SNS/piv/standards.html) with all PIV related Standards.  Below are links to some of the most common Standards:

- **[FIPS-201](http://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.201-2.pdf)** specifies the issuance and management of PIV credentials.
- **[NIST Special Publication 800-73, "Interfaces for Personal Identity Verification"](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-73-4.pdf)** specifies the interface and data elements of PIV credentials.
- **[NIST Special Publication 800-76, "Biometric Data Specification for Personal Identity Verification"](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-76-2.pdf)** specifies the technical acquisition and formatting requirements for biometric data of PIV credentials.
