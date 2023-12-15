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

The TRM methodology selected, NIST, will now be applied to evaluate the cyber risks of this organisation, across the defined tiers mentioned in 2.3.

### 2.4.1 Tier 1 – Prioritisation and scope

The scope should be narrowed, as attempting to do an organisational-wide risk analysis approach would exceed the available bandwidth provided. Daily operations and serving customers, which are common company processes, include prioritised Active Directory (AD) servers, Microsoft Exchange environment, and Oracle SaaS-based enterprise solutions. Verified asset categories include covering the breadth of the 460 Windows 11 endpoints, 12 servers, and cloud applications. Additionally, sensitive data such as user credentials, may be stored in the AD, employee personal information on the Microsoft Exchange Server, and financial records within Oracle's cloud application. This is categoried as "high-value information assets", which required strict access controls.

### 2.4.2 Tier 2 – Infrastructure evaluation

There is a technical lag from running out of support or outdated software – case in point, Windows 11 Pro, so this means that the OS is susceptible to known and publicly available exploits. For third-party services, however, there needs to be a detailed assessment of concepts such as Identity and Access Management (IAM), security monitoring, and key management. A diagnosis of Windows 11 Pro would reveal security gaps, such as pending AES-256 bit encryption for endpoints as well as anti-virus definitions, which results in older malware signatures. Keeping a good asset inventory will assist in identifying any misconfigurations and required server hardening.

### 2.4.3 Tier 3 – Risk assessment process

Efficient thread modeling focused on devices running Windows 11 Pro can help to recognise ransomware, password dictionary attacks, and insider threats and will all be considered high-impact information security events. For the Azure-hosted Oracle cloud solution applications, unauthorised data processing actions and lack of awareness when handling data, in general, should alert the Cloud Security Alliance (CSA). There should be rigorous documentation addressing risk scenarios specific to the company's information security – any likelihood and magnitudes. The mapping of any risks will help realise what security aspects most of the company's attention is required for, and what mitigation strategies need to be put in place.

### 2.4.4 Tier 4 – Ongoing risk monitoring

This tier focuses on the ongoing tracking of information security risks through relevant key risk indicators (RKIs) to enable a quick response if needed. Implementing a Security Information and Event Management (SIEM) platform allowing the company to track critical risk metrics across Windows servers, endpoints, and Oracle Cloud assets. Setting up dashboards for information security admins with details on critical risks, reminders for patch delays, unathorised access attempts, and anomalous data transfers. This relies on the risk register (see 3) to be constantly updated with the latest mediation statuses related to high-priority threats. Any new infrastructure that the company decides to adopt will undergo risk evaluations to see how it synchronises with the other technology used, and if it compromises any existing infrastructure, thus introducing security gaps. This will further demonstrate compliance with UK governmental agencies and any new future contract proposals that the company will get.

# 3 Risk register

A risk register is a tool to document all identified threats and vulnerabilities that pose a problem to the organisation's commercial aims and technological resources, along with the corresponding risk parameters and what infrastructure aspects are affected. This table, developed specifically for this company, maps various cyber risk scenarios that arose as a result of using the NIST TRM to the following parameters:

- $Impact$: refers to the severity of commercial or technological consequences if the risk ends up happening
- $Likelihood$: stands for the probability based on existing infrastructure security gaps
- $Inherent$ $risk$ $rating$: is the product of the $Impact$ and $Likelihood$.
- $Assets$ $affected$: are the specific components of the infrastructure that the risk targets.

| Risk ID | Risk description | Impact | Likelihood | Inherent risk rating | Assets affected |
|:---:|:---|:---:|:---:|:---:|:---|
| R1 | Outdated Windows 11 Pro server OS exposes services to remote code execution and privilege escalation exploits (PVE) | High | High | Extreme | AD servers, E-mail servers |
| R2 | Vulnerabilities in third-party apps like Oracle ERP Cloud applications enable backend server compromise, may allow for data theft | High | Medium | High | Oracle ERP Cloud applications |
| R3 | Lack of endpoint encryption results in the breach of sensitive customer data if the device is lost or stolen | Medium | High | High | Windows 11 laptops and workstations |
| R4 | Obsolete antivirus definitions are unable to recognize the latest malware signatures, which may lead to ransomware attacks | Medium | High | High | Windows endpoints |
| R5 | Weak administrator passwords allow brute force or dictionary attacks and enable backend takeover | High | Medium | Extreme | Domain admin accounts |
| R6 | Unpatched network devices act as an entry point for accessing other servers hosting sensitive information | Medium | Medium | Moderate | Firewalls, Switches, VPN devices |

# 4 Mitigation strategies

Effective mitigation strategies are a combination of introducing multiple security controls. The aim, given in mind the $Inherent$ $risk$ $rating$, would be to reduce the risk likelihood or the impact itself. A wide range of intervention measures should be employed, including those that are technical, operational, or commercial. Any thought of measures should efficiently address information security gaps within the existing infrastructure technology, as brought up by the risk assessment conducted.

## 4.1 R1 mitigation – Outdated Windows Server OS

This risk arises as a result of using an unsupported version of Microsoft Windows Server – still active within the organisation's infrastructure, meaning that it opens exposure to publicly available vulnerabilities where security patches are still necessary. This opens up a much-needed migration plan, in which an upgrade to the latest Windows Server OS (or a Linux equivalent alternatively) should be the main priority. Additionally, regular OS patches in the form of updates should be automated using in-build tools such as Windows Server Update Services (WSUS) rather than relying on system administrators to manually apply patches. Furthermore, legacy servers with any pending updates should be hardened and reviewed against credible benchmarking software, such as CIS. Finally, constant access reviews on the Active Directory can help minimise the attack surface.

## 4.2 R2 mitigation – Vulnerable Oracle Enterprise Cloud Solution

The cloud-based Oracle Enterprise Solution platform would benefit from a coordinated mitigation plan between the provider and the tenant. From the viewpoint of the tenant, any user accounts and their corresponding roles should be examined to ensure that any inactive identities and least privilege principles are promptly immobilised. Procedures involving data classification will swiftly categorise any sensitive financial information traversing within Oracle's data flow and prevent any data loss. It is also Oracle's responsibility to provide reliable assurance of their security certifications, vulnerability remediation measures, and patch deployments via clear documentation. Without this, the company should not announce a shift to using any Oracle services.

## 4.3 R3 mitigation – Unencrypted endpoints

A simple, but effective mitigation strategy would be to use full-disk encryptions through leveraging software such as BitLocker. The application would be necessary for all endpoint devices currently used by the infrastructure – laptops, desktops, and mobile devices. A Standardised Trusted Platform Module (STPM) can enable secure cryptographic storage for BitLocker's (or any encryption software for that matter) encryption keys. For existing hardware assets, this encryption process needs to be integrated into their typical lifecycle through straightforward interfaces to block unauthorised devices from accessing the infrastructure. This can even serve as an interim mitigation until full data protection measures are established.

## 4.4 R4 mitigation – Obsolete antivirus definitions

If there are any automated processes regarding antivirus definitions within the infrastructure technology, these need to be reviewed when updates are applied across all Windows endpoints. With endpoint protection enforced, the vendor will publish patches that include the malware definition for the latest threats. To further complement this, malware entry points should be reduced via prevention measures, such as enhanced spam filtering on mail gateways. Where feasible, the migration to advanced endpoint detection resources (EDR) tools to identify suspicious activity and incoherent signatures should be considered. Perhaps even options to segregate to different network segments for outdated endpoint devices lacking the latest detection for malware signatures.

## 4.5 R5 mitigation – Weak administrator passwords

Multi-factor authentication (MFA) should be enforced for all accounts and interfaces provided administrative access including domain controller logins to provide additional proof. Provision Privileged Access Management (PAM) solutions can serve as a secure password vault for administrator accounts. There should also be continuous scans for all password hashes across all systems within the infrastructure to pinpoint any weak credentials in active use – used in conjunction with strict password policies enforced by the company. The attack surface can be further reduced by disabling Windows file share mappings, which can easily help an attacker traverse and map a data flow. Also limiting endpoint workstations that host developer tools, such as debuggers and compilers – attackers may potentially load exploits via those applications.

## 4.6 R6 mitigation – Unpatched network devices

All network components within the infrastructure need to be tracked, including devices such as routers, switches, firewalls, and load balancers deployed on on-premise and cloud environments. Devices that continue to receive firmware debates that address vulnerability disclosures should remain supported. If a hardware device reaches the "end of support" status, network segmentation gateways should allow for lateral traversal across the different zones whilst that device is being replaced and integrated within the infrastructure's network. Network configurations against industry benchmarks should be a standard as it helps to minmise threats from exploitable network settings. If in the instance that there is a compromise, sufficient backup controls should be implemented, like additional robust firewalls to section off legacy equipment until they can either be patched or decommissioned.

# 5 Future recommendations

While the mitigation strategies outlined in the previous section focus on addressing the specific information security gaps and cyber risks identified in the risk assessment of the current state of the company's infrastructure, long-term information security management requires embracing evolving preventative measures as well. Implementing the following recommendations will facilitate greater data protection, improved threat visibility, and overall maturity in managing risks. This would be roadmaps across different areas in the organisation's infrastructure.

## 5.1 Adopting an information security framework

An Information Security Management System (ISMS) based on internationally well-known standards, such as ISO:27001 or the NIST Cybersecurity Framework can establish a structured approach to managing information risks with clear and defined policies, procedures, and controls. The ISMS is determined by factors such as the company's threat landscape and acceptable risk tolerance. This will promote security governance through industry best practices such as benchmarking, audits, and periodic gauging or security measures. An extensive documentation process will help the organisation to demonstrate diligence and maturity when it comes to information security.

## 5.2 Enhancing identity and access protections

Upgrading identity management and access controls through implementing additional safeguards like Privileged Access Management (PAM) solutions and Multi-factor Authentication (MFA). The introduction of these two security mechanisms will help to limit the exposure of confidential data or critical system assets – in the case of stolen account credentials. Regular reviews of account privileges will assist in mapping specific application roles to certain job functions only to tighten access spans. Automating access lifecycles with features like "just-in-time" evaluations and predefined session durations will prevent standing access.

## 5.3 Instituting configuration hardening standards

Configuration baselines should be formalised, specifically for this company's infrastructure by utilising industry benchmarks to avoid data exposure. Templates mapping best system hardening recommendations, especially for platforms such as Windows, would be beneficial for those servers and endpoints, as it would guide IT teams in sunsetting vulnerable configurations. Compliance can then be tested against established criteria outlined through automated tools.

## 5.4 Implementing SIEM-based security monitoring

# 6 References
