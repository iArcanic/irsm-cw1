---
title: "Risk Analysis Report"
author: "2242090"
bibliography: references.bib
toc: true
toc-title: Table of Contents
toc-depth: 3
fontsize: 10
geometry: margin=1.5in
csl: harvard-imperial-college-london.csl
---

# 1 Introduction

A tech company with approximately 400 employees in its workforce, has recently been awarded a major UK government contract along with a bonus of 30% of revenue. This project is now considered with the utmost importance and requires significant focus.

As the company doesn't work with any UK government already, its existing information security policies are highly unlikely to meet their governmental standards. This means that it is mandatory to implement robust security regulations to adhere to UK government vendors.

This risk analysis report aims to analyse the company's current security mindset, identify any vulnerabilities within its present infrastructure, and outline any outstanding actions to address any security gaps, all via a credible framework. Based on this, recommendations will also be provided to help safeguard against threats and sustainably comply with any protocols or laws defined by the UK government.

# 2 Evaluation of organisational risk posture

## 2.1 Standards, controls, and policies

Given that the company looks to diversify into UK governmental territory, is it crucial that the information security policies are aligned with the relevant regulations.

### 2.1.1 UK governmental policies – Security Policy Framework (SPF)

This is a framework that provides 14 guidelines across various categories, including physical, personnel, and cybersecurity that third-party suppliers must comply with when handling information assets relating to the public [@UKGov2022].

### 2.1.2 ISO/IEC standards – 27001:2013

An internationally recognised standard for security published by ISO and IEC. Serves as a set of requirements for information security management via criteria of technical security mechanisms [@Nunn2021]. A valid certification proves secure information security practices whilst being in line with the CIA triad elements.

### 2.1.3 Cloud security guidance – CSA Cloud Controls Matrix (CCM)

Guidance for cloud-based services and technologies, adapted for security controls and general cyber resilience [@Skoutaris2020]. Refers to best industry practices by adopting well-known frameworks such as to help evaluate risks and assess security obligations within a cloud context.

### 2.1.4 End user device guidelines – EUD Security Guidance

Published by the UK National Cyber Security Centre (NCSC), it is the risk treatment when considering deployment on the end user or personal devices to mitigate any remote-based vulnerabilities that could be exploited by malicious actors [@ncsc2021]. Aims to help organisations manage risks from remote attacks.

## 2.2 Assessment of the current IT infrastructure

Although the infrastructure devices use modern and widely adopted enterprise solutions to be suitable for mainstream support, there are still inherent vulnerabilities that need to be addressed. This may include a large attack surface area being exposed, posing a variety of problems from an information security standpoint.

### 2.2.1 Server infrastructure

Looking more in-depth at their server landscape, 12 servers consist of Microsoft Server 2022 (specifically build 10.0.20348.1787), whilst the rest host Linux Ubuntu 22.04 LTS. Both are critical to the key services of the company's computing environment, for functions such as Active Directory (AD), e-mail, website hosting, DNS, and Oracle Cloud ERP services.

Even though the more up-to-date version of Windows may be more suitable for modern technological standards, malicious entities work tirelessly to develop evolving exploits, so routine and timely patching is required. Additionally, third-party providers such as Oracle present their own set of unique problems, in which vulnerability mitigation requires a coordinated response from both companies.

Specifically, the Research and Development (R&D) Engineering network segment indicates the presence of data flows to other environments, which may be intercepted in transmission [@Zou2013]. If there is an obvious lack of visibility of common server hardening practices that meet typical industrial baselines, the entire company's technological infrastructure could be exposed. This therefore makes these servers less trustworthy.

### 2.2.2 Endpoints

The entirety of the company's endpoint fleet relies on Windows 11 Pro (version 22H2), which has already been flagged as "end of support" [@Microsoft2023] by Microsoft themselves (within approximately 9 months). This has a huge impact on future updates and security patches. Even generic configurations of system settings via the Control Panel could lead to vulnerabilities [@DMCXBlueRedTeam2022] being brought to fruition. An over-dependence on Microsoft services only could lead to prominent security gaps. There are also issues in accommodating BYOD (Bring Your Own Device) schemes to be flexible for different company employees for various preferences to productivity lifestyles, such as the recent rise of remote working.

### 2.2.3 Network components

Since network segmentation details are not explicitly mentioned due to the sensitivity of the information, not much assessment can be made of its current effectiveness. However, given the implementation Research and Development (R&D) dedicated networking segment, the company may benefit from the introduction of VPNs and externally facing gateways.

In general, however, basic network security concepts still apply. If the company has most of its technology components connected via wireless over ethernet, this not only increases the attack surface for endpoints and cloud services but compromises network traffic confidentiality [@Arbaugh2003]. Without proper authentication, encryption, access logging, and monitoring controls, a network's CIA (Confidentiality, Integrity, and Availability) can be compromised.

In addition, although not directly security-related, thorough documentation that contains details about the network topology, external security access, and any wireless protection protocols should exist. This will help the network administrators keep a track record of any changes that do occur, and if so, proactively make any necessary changes.

## 2.3 Selection of risk assessment methodology – NIST TRM

The National Institute of Standards of Technology (NIST) Tiered Risk Management (TRM) approach has been chosen to be applied to this company under an information security assessment. This specific TRM however offers a four-tiered scalable method to evaluate an organisation's cybersecurity practices.

Key features of this four-tiered TRM approach [@nist2023] include:

- Tier 1: Partial implementation (prioritisation and scope focus)
- Tier 2: Risk-informed (evaluation of existing infrastructure)
- Tier 3: Repeatable (risk assessment process)
- Tier 4: Adaptive (ongoing risk monitoring)

However, the key benefits of this TRM offered by NIST have to be suitable with the company information security assessment, so there needs to be robust justification:

- Flexibility in a scalable, but adaptable program based on the company's technological resources.
- Promotes structure via the different tiers the TRM offers.
- Enables the progressive building of risk knowledge via each tier.
- Allows for the continuous evolution and improvement through each iterative TRM loop.
- Encourages and inspires confidence for buy-in and financial commitments over time.

The above aspects lead themselves well, in terms of suitability for the organisation's objectives. A tiered progression path will help strike a balance between security optimisation and capacity-related constraints.

## 2.4 NIST Tiered Risk Management (TRM) approach

The TRM methodology selected, NIST, will now be applied to evaluate the cyber risks of this organisation, across the defined tiers highlighted in 2.3.

### 2.4.1 Tier 1 – Partial implementation

The scope should be narrowed to only focus on the necessary parts of the organsiation. Daily operations and serving customers include the usage of Active Directory (AD) servers, Microsoft Exchange environment, and Oracle SaaS-based enterprise solutions. Verified asset categories consist of 460 Windows 11 endpoints, 12 servers, and cloud applications. Additionally, sensitive data such as user credentials, may be stored in the AD, employee personal information on the Microsoft Exchange Server, and financial records within Oracle's cloud application. These are categorised as "high-value information assets" [@Tatar2021], which require strict access controls.

### 2.4.2 Tier 2 – Risk-informed

See 2.2.

### 2.4.3 Tier 3 – Repeatable

Efficient threat modeling focused on devices running Windows 11 Pro can help to recognise ransomware, password dictionary attacks, and insider threats and will all be considered high-impact information security events. For the Azure-hosted Oracle cloud solution applications, unauthorised data processing actions and lack of awareness when handling data, in general, should alert the Cloud Security Alliance (CSA). There should be rigorous documentation addressing risk scenarios specific to the company's information security – any likelihood and magnitudes. The mapping of any risks will help realise what security aspects most of the company's attention is required for, and what mitigation strategies need to be put in place.

### 2.4.4 Tier 4 – Adaptive

This tier focuses on the ongoing tracking of information security risks through relevant key risk indicators (KRIs) to enable a quick response if needed [@Andersen2016]. Implementing a Security Information and Event Management (SIEM) platform [@Gonzalez2021] allowing the company to track critical risk metrics across Windows servers, endpoints, and Oracle Cloud assets. Setting up dashboards for information security admins with details on critical risks, reminders for patch delays, unathorised access attempts, and anomalous data transfers can prove to be beneficial in the long term for risk mitigation. This relies on the risk register (see 3) to be constantly updated with the latest threats. Any new infrastructure that the company decides to implement will undergo risk evaluations to see how it fits in with other technology used, and if it compromises any existing infrastructure. This will further demonstrate compliance with UK governmental agencies and any new future contract proposals.

# 3 Risk register

A risk register is a tool to document all identified threats and vulnerabilities that pose a problem to the organisation's commercial aims and technological resources, along with the corresponding risk parameters and what infrastructure targets are affected [@Prasanna2021]. This table, developed specifically for this company, maps various cyber risk scenarios that arose as a result of using the NIST TRM to the following parameters:

- $Impact$: refers to the severity of commercial or technological consequences if the risk ends up happening [@Prasanna2021].
- $Likelihood$: stands for the probability based on existing infrastructure security gaps [@Prasanna2021].
- $Inherent$ $risk$ $rating$: is the product of the $Impact$ and $Likelihood$ [@Prasanna2021].
- $Assets$ $affected$: are the specific components of the infrastructure that the risk targets [@Prasanna2021].

| Risk ID | Risk description                                                                                                                  | CVEs (if applicable)                                           | Impact | Likelihood | Inherent risk rating | Assets affected                     |
| :-----: | :-------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- | :----: | :--------: | :------------------: | :---------------------------------- |
|   R1    | Outdated Windows 11 Pro server OS exposes services to remote code execution and privilege escalation exploits (PVE)               | [@cve202335633]                                                |  High  |    High    |       Extreme        | AD servers, E-mail servers          |
|   R2    | Vulnerabilities in third-party apps like Oracle ERP Cloud applications enable backend server compromise, may allow for data theft | [@cve20212320], [@cve20212319], [@cve20212318], [@cve20212317] |  High  |   Medium   |         High         | Oracle ERP Cloud applications       |
|   R3    | Lack of endpoint encryption results in the breach of sensitive customer data if the device is lost or stolen                      | [@cve202328005]                                                | Medium |    High    |         High         | Windows 11 laptops and workstations |
|   R4    | Outdated antivirus definitions are unable to recognize the latest malware signatures, which may lead to ransomware attacks        | [@wndfav0000292023] (CVE ID not available)                     | Medium |    High    |         High         | Windows endpoints                   |
|   R5    | Weak administrator passwords allow brute force or dictionary attacks and enable backend takeover                                  | [@cve20221039] (For Linux hosts)                               |  High  |   Medium   |       Extreme        | Domain admin accounts               |
|   R6    | Unpatched network devices act as an entry point for accessing other servers hosting sensitive information                         | N/A, due to obscurity of network details                       | Medium |   Medium   |       Moderate       | Firewalls, Switches, VPN devices    |

# 4 Mitigation strategies

Effective mitigation strategies are a combination of introducing multiple security controls. The aim, given in mind the $Inherent$ $risk$ $rating$, would be to reduce the risk $Likelihood$ or the $Impact$ itself. Any thought of measures should efficiently address information security gaps within the existing infrastructure technology, as brought up by the risk assessment conducted. Within this section, the top three most high-priority risks will be explored further in detail.

## 4.1 R1 mitigation – Outdated Windows Server OS

This risk arises as a result of using an unsupported version of Microsoft Windows Server – still active within the organisation's infrastructure, meaning that it opens exposure to publicly available vulnerabilities where security patches are still necessary. This opens up a much-needed migration plan, in which an upgrade to the latest Windows Server OS (or a Linux equivalent) should be the main priority. Additionally, regular OS patches in the form of updates should be automated using in-build tools such as Windows Server Update Services (WSUS) rather than relying on system administrators to manually apply patches. Furthermore, legacy servers with any pending updates should be hardened and reviewed against credible benchmarking software, such as CIS. Finally, constant access reviews on the Active Directory can help minimise the attack surface.

## 4.2 R2 mitigation – Vulnerable Oracle Enterprise Cloud Solution

The cloud-based Oracle Enterprise Solution platform would benefit from a coordinated mitigation plan between the provider and the tenant. From the viewpoint of the tenant, any user accounts and their corresponding roles should be examined to ensure that any inactive identities and least privilege principles are promptly immobilised. Procedures involving data classification will swiftly categorise any sensitive financial information traversing within Oracle's data flow and prevent any data loss. It is also Oracle's responsibility to provide reliable assurance of their security certifications, vulnerability remediation measures, and patch deployments via clear documentation. Without this, the company should not announce a shift to using any Oracle services.

## 4.3 R5 mitigation – Weak administrator passwords

Multi-factor authentication (MFA) should be enforced for all accounts and interfaces provided administrative access including domain controller logins to provide additional proof. Provision Privileged Access Management (PAM) solutions can serve as a secure password vault for administrator accounts. There should also be continuous scans for all password hashes across all systems within the infrastructure to pinpoint any weak credentials in active use – used in conjunction with strict password policies enforced by the company. The attack surface can be further reduced by disabling Windows file share mappings, which can easily help an attacker traverse and map a data flow. Also limiting endpoint workstations that host developer tools, such as debuggers and compilers – attackers may potentially load exploits via those applications.

# 5 Future recommendations

While the mitigation strategies outlined in the previous section focus on addressing specific information security gaps and cyber risks identified in the risk assessment of the current state of the company's infrastructure, long-term information security management requires embracing evolving preventative measures as well. Implementing the following recommendations will facilitate greater data protection, improved threat visibility, and overall maturity in managing risks. This would be roadmaps across different areas in the organisation's infrastructure.

## 5.1 Adopting an information security framework

An Information Security Management System (ISMS) based on internationally well-known standards, such as ISO:27001 or the NIST cybersecurity framework can establish a structured approach to managing information risks with clear and defined policies, procedures, and controls. The ISMS is determined by factors such as the company's threat landscape and acceptable risk tolerance. This will promote security governance through industry best practices such as benchmarking, audits, and periodic gauging or security measures. An extensive documentation process will also help the organisation demonstrate maturity when it comes to information security.

## 5.2 Enhancing identity and access protections

Upgrading identity management and access controls through implementing additional safeguards like Privileged Access Management (PAM) [@Garbis2021] solutions and Multi-factor Authentication (MFA) [@Ometov2018]. The introduction of these two security mechanisms will help to limit the exposure of confidential data or critical system assets – in the case of stolen account credentials. Regular reviews of account privileges will assist in mapping specific application roles to certain job functions only to tighten access spans.

## 5.3 Instituting configuration hardening standards

Configuration baselines should be formalised, by utilising industry benchmarks to avoid data exposure. Templates outlining best system hardening recommendations, especially for platforms such as Windows, would be beneficial for those servers and endpoints, as it would guide IT teams in sunsetting vulnerable configurations. Compliance can then be tested against established criteria via automated tools.

## 5.4 Implementing SIEM-based security monitoring

Deploying a managed SIEM platform for correlating security event data using risk-based intelligence will provide constant visibility into anomalies, attempted data breaches, or incidents across the company's hybrid infrastructure [@Gonzalez2021]. Automated response workflows can help trigger the relevant security measures around detection based on the severity gauged by the risk register (see 3). Ongoing tuning of use case rules can help the organisation's infrastructure in proactive risk mitigation.

# 6 References
