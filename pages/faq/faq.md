---
title: Frequently Asked Questions
layout: docs
permalink: /faq/
---

- [What is the U.S. Federal Public Trust TLS PKI?](#what-is-the-us-federal-public-trust-tls-pki)
- [What kind of certificates will this service issue?](#what-kind-of-certificates-will-this-service-issue)
- [When will this service be available?](#when-will-this-service-be-available)
- [What are the requirements to use this service?](#what-are-the-requirements-to-use-this-service)
- [How much will it cost to use this service?](#how-much-will-it-cost-to-use-this-service)
- [What is the relationship between the U.S. Federal Public Trust TLS PKI and the Federal PKI?](#what-is-the-relationship-between-the-us-federal-public-trust-tls-pki-and-the-federal-pki)
- [Who can I contact for support or to report an incident?](#who-can-i-contact-for-support-or-to-report-an-incident)


### What is the U.S. Federal Public Trust TLS PKI?
The U.S. Federal Public Trust Transport Layer Security (TLS) Public Key Infrastructure (PKI) is a service offered collaboratively by the General Services Administration (GSA) and the Defense Information Systems Agency (DISA). Teams from GSA and DISA have worked together since 2016 to design and build a service that issues TLS certificates for federal *.gov* and *.mil* web services. 

**The U.S. Federal Public Trust TLS PKI will...**
- satisfy modern Web PKI requirements like Certificate Transparency (CT) and shorter certificate validity periods.
- be agile, purpose-driven, open, and transparent.
- promote automation to improve U.S. Federal Government efficiencies.
- be separate from the [Federal Public Key Infrastructure](https://www.idmanagement.gov/topics/fpki/){:target="_blank"}.


### What kind of certificates will this service issue?
The service will issue 2048-bit RSA certificates signed with the SHA-256 hashing algorithm. Certificates will have a validity **no longer** than 13-months and will be published to **at least** two CT Logs.


### When will this service be available?
There's a lot that goes into building a publicly-trusted Public Key Infrastructure.
- Policy, practices, and procedures must be written.
- Certification Authorities need to be built and audited.
- Applications must be submitted to commercial trust store and CT Log operators to facilitate global trust.
- If applications are approved, the Root CA signing certificate must be globally distributed to operating-systems and web-browsers.

We **cannot** guarantee commercial trust store operators like Microsoft, Apple, or Mozilla will approve our application for distribution. **Best-case scenario**, initial issuance of publicly-trusted TLS certificates could begin **Q1 FY 2021**.


### What are the requirements to use this service?
- The service will only issue certificates to **federal** .gov and .mil web services.
- Web services must be **Internet-accessible** to communicate with the Issuing Certification Authority (CA) for certificate issuance.
- Certificate issuance must take place using the **Automated Certificate Management Environment** protocol. **No human Registration Authorities.**
- Certificates will be published to **at least** two (2) publicly-accessible CT Logs.
- Certificate validity will be limited to **13 months or less**.


### How much will it cost to use this service?
We're figuring this out. We'll have more information for you shortly.


### What is the relationship between the U.S. Federal Public Trust TLS PKI and the Federal PKI?
The GSA currently oversees the Federal Public Key Infrastructure (FPKI), a trust framework comprised of over 150 Certification Authorities used to issue and manage person identity and enterprise device identity certificates for the Federal Government and mission partners. The FPKI is managed and operated as a bridged PKI, whose original purpose was intended to establish trust across related communities of interest. 

The U.S. Federal Public Trust TLS PKI will be managed as a separate and distinct PKI. It will support the automated issuance of publicly trusted TLS certificates to federal DotGov and DotMil web services. 

For now, the FPKI Policy Authority maintains the governance and voting rights to manage the U.S. Federal Public Trust TLS PKI Certificate Policy. 

Click [here](https://www.idmanagement.gov/topics/fpki/){:target="_blank"} to learn more about the FPKI.


### Who can I contact for support or to report an incident?
For general questions, email us at {{site.email}}.

To report an incident, review our [incident reporting procedures]({{site.baseurl}}/docs/incident-reporting).
