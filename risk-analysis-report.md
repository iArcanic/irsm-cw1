---
title: "Risk Analysis Report"
author: "2242090"
bibliography: references.bib
toc: true
toc-title: Table of Contents
toc-depth: 3
csl: harvard-imperial-college-london.csl
---

# 1 Introduction

A high-tech company with approximately 400 employees in its workforce, has recently been awarded a major UK government contract, with the additional bonus of 30% revenue to the organisation. This project is now therefore considered with the utmost importance and therefore requires significant focus and dedicated resources.

Since the company does not already work with any UK Governments beforehand, its existing information security policies and regulations are highly unlikely to meet the UK's governmental standards. This means that it is mandatory to implement robust compliance measures and information security protocols to adhere to UK government vendors.

This risk analysis report aims to analyse the company's current security mindset, identify any vulnerabilities within their present setup technologies and infrastructure used, and outline any outstanding actions to address any security gaps via a credible security framework. Based on this, recommendations will also be provided to execute the appropriate actions that help safeguard against security threats and sustainably comply with the necessary protocols or laws defined by the UK government. With this, it is advantageous for the company to capitalise on this opportunity for general business growth and profit maximisation.

# 2 Evaluation of organisational risk posture

## 2.1 Standards, controls, and policies

Given that the company looks to diversify into UK governmental territory, is it crucial that the information security policies are in alignment with governmental regulations and industrial standards.

### 2.1.1 Governmental policies – Security Policy Framework (SPF)

This is a framework that provides 14 guidelines across various categories, such as physical, personnel, and cybersecurity that third party-suppliers and any public entities must comply with when handling information assets relating to the public.

### 2.1.2 ISO/IEC standards – 27001:2013

An internationally recognised standard for security published by ISO and IEC as a set of requirements for information security management via a set of technical security mechanisms. A valid certification proves a secure information security management system in line with the CIA triad attributes.

### 2.1.3 Cloud security guidance – CSA Cloud Controls Matrix (CCM)

Guidance for cloud-based services and technologies adapted for security controls and general cyber resilience. Refers to best industry practices by adopting well-known frameworks such as to help evaluate risks and assess security obligations within a cloud context.

### 2.1.4 End user device guidelines – EUD Security Guidance

Published by the UK National Cyber Security Centre (NCSC), it is the risk treatment when considering deployment on the end user or personal devices to mitigate any remote-based vulnerabilities that could be exploited by malicious actors. Aims to help organisations manage risks from remote attacks.

## 2.2 Assessment of the current IT infrastructure

From the current IT infrastructure, the business has an acclimation to using Microsoft technologies, to deliver their services, with company statistics detailing that 86% of servers and 100% of user devices are based on the Windows platform. Although the infrastructure devices use modern and widely adopted enterprise solutions to be suitable for mainstream support, there are still inherent vulnerabilities that need to be addressed. This may include a large attack surface area being exposed, posing a variety of problems from an information security standpoint.

### 2.2.1 Server infrastructure

Looking more in-depth at the server landscape, 12 of their servers consist of Microsoft Server 2022 (specifically build 10.0.20348.1787) whilst the rest of the 2 servers host Linux Ubuntu 22.04 LTS. Both are critical to the key services of the company's computing environment, for functions such as Active Directory, e-mail, website hosting, DNS, and Oracle Cloud ERP services.

Even though the more up-to-date version of Windows is potentially more suitable for modern technological purposes, malicious entities work tirelessly to develop evolving exploits, so routine and timely patching is required. Additionally, third-party providers. such as Oracle, in this case, presents its own set of unique problems, in which vulnerability mitigation requires a coordinated response from both companies.

Specifically, the Research and Development (R&D) Engineering network segment – its specific division from the main production platform – indicates the presence of data flows to other environments, which may be intercepted in transmission. If there is an obvious lack of visibility of common server hardening practices that meet typical industrial baselines, the entire company's technological infrastructure could be exposed. This therefore makes these servers less trustworthy.

### 2.2.2 Endpoints

The entirety of the company's endpoint fleet relies solely on Windows 11 Pro (version 22H2), which has already been flagged as "end of support" by Microsoft themselves. This has a huge impact on future updates and security patches. Even generic configurations of system settings via the Control Centre could lead to vulnerabilities being brought to fruition. An over-dependence on Microsoft services only could lead to prominent security gaps. There are also issues in accommodating BYOD (Bring Your Own Device) schemes to be flexible for different company employees for various preferences to productivity lifestyles, such as the recent rise of remote working, for example.

### 2.2.3 Network components

Since network segmentation details are obscure due to the sensitivity of the information, not much assessment can be made on its current effectiveness relevant to security aspects. The current information given does not shed light on network security zoning concepts or if any access restrictions have been reinforced. However, given that the Research and Development (R&D) networking segment exists, the company may benefit from the introduction of VPNs and externally facing gateways.

In general, however, basic network security concepts apply. If the company has most of its technology components connected via wireless over ethernet, this not only increases the attack surface for endpoints and cloud services but compromises network traffic confidentiality. Without proper authentication, encryption, access logging, and monitoring controls, a network's CIA (Confidentiality, Integrity, and Availability).

In addition, although not directly security-related, thorough documentation should be a regular process that contains details about the network topology, external security access, and any wireless protection protocols. This will help the network administrators keep a track record of any changes that do occur, and if so, proactively make changes to address changes in any manner.

## 2.3 Selection of risk assessment methodology – NIST TRM

The National Institute of Standards of Technology (NIST) Tiered Risk Management (TRM) approach has been chosen to be applied to this company under an information security assessment. This specific TRM however offers a four-tiered scalable method scalable method to evaluate an organisation's cybersecurity practices.

Key features of this four-tiered TRM approach include:

- Tier 1: Prioritisation and scope focus
- Tier 2: Infrastructure evaluation
- Tier 3: Risk assessment process
- Tier 4: Ongoing risk monitoring

For any TRM, a crucial point starting point involves framing out an organisation's priorities, values, aims, and resource bandwidth constraints. From this, subsequent activities intrinsic to the rest of the framework can be carried out.

However, the key benefits of this TRM offered by NIST have to be in alignment with the company information security examination, so there needs to be robust justification as to why this specific TRM was chosen:

- Flexibility in a scalable, but adaptable program based on the company's technological resource capabilities.
- Promotes structure via the different tiers the TRM offers.
- Enables the progressive building of risk knowledge via each iteration (or tier) of the TRM.
- Allows for the continuous evolution and improvement through each iterative TRM loop.
- Encourages and inspires confidence for buy-in and financial commitments over time.

The above aspects lead themselves well, in terms of suitability for the organisation's objectives. A tiered progression path will help strike a balance between security optimization and capacity-related constraints.

## 2.4 NIST Tiered Risk Management (TRM) approach

# 3 Risk register

# 4 Mitigation strategies

# 5 Future recommendations

# 6 Appendices

# 7 References
