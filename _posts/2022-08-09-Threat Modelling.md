---
title: 'Threat Modelling'
date: 2022-08-09
permalink: /posts/2022/08/Threat Modelling/
tags:
  - Vulnerability
  - OWASP TOP 10
  - Threat Modelling
---
What is Threat Modeling

Threat modeling is a structured approach of identifying,analyzing and mitigating potential security threats in the system, application or network in the early stage of the design phase of SDLC. The purpose of threat modelling is to identify, communicate, and understand threats and mitigations within the context of protecting something of value.

![Alt text](https://docs.microsoft.com/en-us/azure/security/media/azure-security-threat-modeling-tool-feature-overview/sdlapproach.png)

Why Threat Modeling Need

* Identify the threat in the early stage of SDLC it will reduce the cost and effort of fixing in the vulnerabilities software developer life cycle.
* Make sure we follow the compliance standard framework e.g.OWASP ASVS, NIST, ISO 27001.
* Creates security mindset across the team.

How to perform and what things need to be collected before doing theat modeling.

1) Understand the scope given. 

2) Have a small call with stakeholders (developer, product manager, business owner, Security member)

4) Gather documentation and Articture diagram( Collect DFD diagram )

5) Identify the threat using various frameworks like STRIDE, PASTA

6) Assess the security risk and evaluate the security impact using the CVSS score system 

7) Explain them to Mitigating using Proper security controls and reduce the security risk

8) validate the security test using dast and sast.

Tools:

* Irurisk

* Microsoft Threat Modeling 

* OWASP Threat Dragon

DFD is Often used to represent the following diagram.

Rectangle(External entities) - Actor interacting with the systems.

circle (Process) - logical operation been performed.

Arrow(Data flow) - The movement of data.

parallel line(data store) - where data will store

dotted line - inside and outside the boundary ( a user interacting outside the internet ).

**A threat model typically includes:**

* Description of the subject to be modelled

* Assumptions that can be checked or challenged in the future as the threat landscape changes

* Potential threats to the system

* Actions that can be taken to mitigate each threat

* A way of validating the model and threats, and verification of the actions taken

**Top Threat Modelling Framework**

* STRIDE

* OWASP Top 10

* MITRE ATT&CK


**Let  take STRIDE threat modelling**

STRIDE is a threat modeling framework developed by Microsoft employees and published in 1999. The STRIDE threat model is focused on the potential impacts of different threats to a system:

* Spoofing

* Tampering

* Repudiation

* Information disclosure

* Denial of service

* Escalation of privileges


