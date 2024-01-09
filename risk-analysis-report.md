---
title: "Risk Analysis Report"
author: "2242090"
bibliography: references.bib
toc: true
toc-title: Table of Contents
toc-depth: 3
fontsize: 10
geometry: "left=1.25cm, right=1.25cm, top=1.25cm, bottom=1.25cm"
csl: harvard-imperial-college-london.csl
---

# 1 Introduction

A tech company with approximately 400 employees in its workforce, has recently been awarded a major UK government contract along with a bonus of 30% of revenue. This project is now considered with the utmost importance and requires significant focus.

As the company doesn't work with any UK government already, its existing information security policies are highly unlikely to meet governmental standards. This means that it is mandatory to implement robust security regulations to adhere to UK government vendors.

This risk analysis report aims to analyse the company's current security mindset, identify any vulnerabilities within the infrastructure, and outline any outstanding actions to address security gaps, all via a credible framework. Based on this, recommendations will also be provided to help safeguard against threats and sustainably comply with any protocols or laws defined by the UK government.

# 2 Evaluation of organisational risk posture

## 2.1 Standards, controls, and policies

Given that the company looks to diversify into UK governmental territory, is it crucial that the information security policies are aligned with the relevant regulations.

### 2.1.1 UK governmental policies – Security Policy Framework (SPF)

This is a framework that provides 14 guidelines across various categories, including physical, personnel, and cybersecurity that third-party suppliers must comply with when handling information assets relating to the public [@UKGov2022].

### 2.1.2 ISO/IEC standards – 27001:2013

An internationally recognised standard for security published by ISO and IEC. Serves as a set of requirements for information security management via criteria of technical security mechanisms [@Nunn2021]. A valid certification proves secure information security practices.

### 2.1.3 Cloud security guidance – CSA Cloud Controls Matrix (CCM)

Guidance for cloud-based services and technologies, adapted for security controls and general cyber resilience [@Skoutaris2020]. Refers to best industry practices by adopting well-known frameworks such as to help evaluate risks and assess security obligations within a cloud context.

### 2.1.4 End user device guidelines – EUD Security Guidance

Published by the UK National Cyber Security Centre (NCSC), it is the risk treatment when considering deployment on end-user or personal devices to mitigate any remote vulnerabilities that could be exploited by malicious actors [@ncsc2021].

## 2.2 Assessment of the current IT infrastructure

Although the infrastructure devices use modern and widely adopted enterprise solutions to be suitable for mainstream support, there are still inherent vulnerabilities that need to be addressed. This may include large attack surface areas being exposed, posing a variety of problems from an information security standpoint.

### 2.2.1 Server infrastructure

Looking more in-depth at the server landscape, 12 servers consist of Microsoft Server 2022 (specifically build 10.0.20348.1787), whilst the rest host Linux Ubuntu 22.04 LTS. Both are critical to the key services of the company's computing environment, for functions such as Active Directory (AD), e-mail, website hosting, DNS, and Oracle Cloud ERP services.

Even though the more up-to-date version of Windows may be more secure, malicious entities work tirelessly to develop exploits, so routine and timely patching is required. Additionally, third-party providers such as Oracle present their own set of unique problems, where vulnerability mitigation requires a coordinated response from both companies.

Specifically, the Research and Development (R&D) Engineering network segment indicates the presence of data flows to other environments, which may be intercepted in transmission [@Zou2013]. If there is an obvious lack of visibility of common server hardening practices that meet typical industrial baselines, the entire company's technological infrastructure could be exposed. This therefore makes these servers less trustworthy.

### 2.2.2 Endpoints

The entirety of the company's endpoint devices rely on Windows 11 Pro (version 22H2), which has already been flagged as "end of support" [@Microsoft2023] by Microsoft themselves (within approximately 9 months at the time of writing). Even generic configurations of system settings via the Control Panel can lead to vulnerabilities [@DMCXBlueRedTeam2022].

### 2.2.3 Network components

Since network segmentation details are not explicitly mentioned due to the sensitivity of the information, not much assessment can be made of its current effectiveness. However, given the Research and Development's (R&D) dedicated networking segment, the company may benefit from VPNs and externally facing gateways.

In general, basic network security concepts still apply. If the company has most of its technology components connected via wireless over ethernet, this not only increases the attack surface for endpoints and cloud services but compromises network confidentiality [@Arbaugh2003]. Without proper authentication, encryption, access logging, and monitoring controls, a network's CIA can be compromised.

## 2.3 Selection of risk assessment methodology – NIST TRM

The National Institute of Standards of Technology (NIST) Tiered Risk Management (TRM) approach will be applied to this company under an information security assessment. This specific TRM offers a four-tiered scalable method to evaluate an organisation's cybersecurity practices.

Key features of this four-tiered TRM approach [@nist2023] include:

- Tier 1: Partial implementation (prioritisation and scope focus)
- Tier 2: Risk-informed (evaluation of existing infrastructure)
- Tier 3: Repeatable (risk assessment process)
- Tier 4: Adaptive (ongoing risk monitoring)

However, the key benefits of this TRM offered by NIST have to be suitable with the company information security assessment, so there needs to be robust justification:

- Flexibility in a scalable, but adaptable program based on the company's technological resources.
- Promotes structure via the different tiers the TRM offers.
- Enables the progressive building of risk knowledge via each tier.
- Allows for continuous improvement at each tier.
- Encourages and inspires confidence for buy-in and financial commitments over time.

## 2.4 NIST Tiered Risk Management (TRM) approach

The TRM methodology selected, NIST, will now be applied to evaluate the cyber risks of this organisation, across the defined tiers highlighted in [2.3](#23-selection-of-risk-assessment-methodology-–-nist-trm).

### 2.4.1 Tier 1 – Partial implementation

The scope should be narrowed to only focus on the necessary parts of the organisation. Daily operations and serving customers include the usage of Active Directory (AD) servers, Microsoft Exchange environment, and Oracle SaaS-based enterprise solutions. Verified asset categories consist of 460 Windows 11 endpoints, 12 servers, and cloud applications. Additionally, sensitive data such as user credentials, may be stored in the AD, employee personal information on the Microsoft Exchange Server, and financial records within Oracle's cloud application. These are categorised as "high-value information assets" [@Tatar2021], requiring strict access controls.

### 2.4.2 Tier 2 – Risk-informed

See [2.2](#22-assessment-of-the-current-it-infrastructure).

### 2.4.3 Tier 3 – Repeatable

Efficient threat modeling focused on devices running Windows 11 Pro can help to recognise ransomware, password dictionary attacks, and insider threats and be considered as high-impact information security events. For the Azure-hosted Oracle cloud solution applications, unauthorised data processing actions and lack of awareness when handling data, in general, should alert the Cloud Security Alliance (CSA). There should be rigorous documentation addressing risk scenarios specific to the company's information security – any likelihood and magnitudes. The mapping of risks will help realise what security aspects most of the company's attention is required for, and what mitigation strategies are required.

### 2.4.4 Tier 4 – Adaptive

This tier focuses on the ongoing tracking of security risks through relevant key risk indicators (KRIs) for quick responses [@Andersen2016]. Implementing a Security Information and Event Management (SIEM) platform [@Gonzalez2021] allows the company to track risk metrics across Windows servers, endpoints, and Oracle Cloud assets. Setting up dashboards for information security admins with details on critical risks, unathorised access attempts, and anomalous data transfers can prove to be beneficial. This relies on the risk register (see [3](#3-risk-register)) to be constantly updated with the latest threats. Any new infrastructure the company decides to implement will undergo risk evaluations to see whether it compromises any existing infrastructure.

# 3 Risk register

A risk register is a tool to document all identified threats and vulnerabilities that pose a problem to the organisation's commercial aims and technological resources, along with the corresponding risk parameters and what infrastructure targets are affected [@Prasanna2021]. This table maps various cyber risk scenarios that arose as a result of using the NIST TRM to the following parameters:

- $Impact$: refers to the severity of commercial or technological consequences if the risk ends up happening [@Prasanna2021].
- $Likelihood$: stands for the probability based on existing infrastructure security gaps [@Prasanna2021].
- $Risk$ $rating$: is the product of the $Impact$ and $Likelihood$ [@Prasanna2021].
- $Assets$ $affected$: are the specific components of the infrastructure that the risk targets [@Prasanna2021].

| Risk description                                                                            | Impact | Likelihood | Rating  |                  Assets affected |
| :------------------------------------------------------------------------------------------ | :----: | :--------: | :-----: | -------------------------------: |
| R1: Outdated Windows OS leads to remote code execution and privilege escalation exploits    |  High  |    High    | Extreme |       AD servers, E-mail servers |
| R2: Vulnerabilities in Oracle ERP Cloud allow for data theft                                |  High  |    Mid     |  High   |    Oracle ERP Cloud applications |
| R3: Without endpoint encryption, losing or stealing a device compromises sensitive data     |  Mid   |    High    |  High   |             Windows workstations |
| R4: Outdated antivirus don't have updated malware signatures, leading to ransomware attacks |  Mid   |    High    |  High   |                Windows endpoints |
| R5: Weak admin passwords allows for brute force or dictionary attacks                       |  High  |    Mid     | Extreme |                  Domain accounts |
| R6: Unpatched network devices act as entry points to access sensitive information           |  Mid   |    Mid     |   Mid   | Firewalls, switches, VPN devices |

## 3.1 CVEs (if applicable) for identified risks

| Risk ID | CVEs (if applicable)                                                                                                   |
| :-----: | :--------------------------------------------------------------------------------------------------------------------- |
|   R1    | CVE-2023-35633 [@cve202335633]                                                                                         |
|   R2    | CVE-2021-2320 [@cve20212320], CVE-2021-2319 [@cve20212319], CVE-2021-2318 [@cve20212318], CVE-2021-2317 [@cve20212317] |
|   R3    | CVE-2023-28005 [@cve202328005]                                                                                         |
|   R4    | WNDF-AV-000029 [@wndfav0000292023] – CVE ID not available                                                              |
|   R5    | CVE-2022-1039 [@cve20221039] – For Linux hosts                                                                         |
|   R6    | N/A, due to obscurity of network details                                                                               |

# 4 Mitigation strategies

Effective mitigation strategies introduce multiple security controls. The aim, given in mind the $Risk$ $rating$, would be to reduce the risk $Likelihood$ or the $Impact$ itself. Any measures should efficiently address information security gaps within the infrastructure technology, as highlighted by the risk assessment. Within this section, the top three most high-priority risks will be explored.

## 4.1 R1 mitigation – Outdated Windows Server OS

This risk arises as a result of using an unsupported version of Windows Server – still active within the organisation's infrastructure, meaning that it opens exposure to publicly available vulnerabilities where security patches are still pending. This opens up a migration plan, in which an upgrade to the latest Windows Server OS (or a Linux equivalent) is the main priority. Additionally, regular OS patches should be automated using built-in tools such as Windows Server Update Services (WSUS) rather than manual patches. Furthermore, legacy servers with any pending updates should be hardened against credible benchmarking software, such as CIS.

## 4.2 R2 mitigation – Vulnerable Oracle Enterprise Cloud Solution

The cloud-based Oracle Enterprise Solution platform would benefit from a coordinated mitigation plan between both companies. Any user accounts and their corresponding roles should be examined to ensure that any inactive identities and user privileges are dealt with. Data classification procedures will categorise any sensitive financial information traversing within Oracle's data flow. It is also Oracle's responsibility to provide reliable assurance of their security certifications, vulnerability remediation measures, and patch deployments via clear documentation. Without this, the company should not announce a shift to using any Oracle services.

## 4.3 R5 mitigation – Weak administrator passwords

Multi-factor authentication (MFA) should be enforced for all interfaces providing administrative access including domain controller logins. Provision Privileged Access Management (PAM) solutions can serve as a secure password vault for administrator accounts. There should also be continuous scans for all password hashes across all systems to pinpoint any weak credentials in active use. Also limiting endpoint workstations that host developer tools, such as debuggers and compilers – attackers may potentially load exploits via those applications.

# 5 Future recommendations

While the mitigation strategies outlined in the previous section focus on addressing the cyber risks identified in the risk assessment of the current company's infrastructure, long-term information security management requires embracing preventative measures as well. Implementing the following recommendations will allow greater data protection, improved threat visibility, and overall maturity in managing risks.

## 5.1 Adopting an information security framework

An Information Security Management System (ISMS) based on internationally well-known standards, such as ISO:27001 or the NIST cybersecurity framework can establish a structured approach to managing information risks with clear and defined policies and controls. The ISMS is determined by factors such as the company's threat landscape and acceptable risk tolerance. This will promote security governance through industry best practices such as benchmarking, audits, and periodic gauging or security measures. An extensive documentation process will also help the organisation demonstrate maturity when it comes to information security.

## 5.2 Enhancing identity and access protections

Upgrading identity management and access controls through implementing additional safeguards like Privileged Access Management (PAM) [@Garbis2021] solutions and Multi-factor Authentication (MFA) [@Ometov2018]. The introduction of these two security mechanisms will help to limit the exposure of confidential data or critical system assets – in the case of stolen account credentials. Regular reviews of account privileges will assist in mapping specific application roles to certain job functions only to tighten access spans.

## 5.3 Instituting configuration hardening standards

Configuration baselines should be formalised, by utilising industry benchmarks. Templates outlining best system hardening recommendations, especially for platforms such as Windows, would be beneficial for servers and endpoints, as they would guide IT teams in sunsetting vulnerable configurations.

## 5.4 Implementing SIEM-based security monitoring

Deploying a managed SIEM platform for security events using risk-based data will provide constant visibility into anomalies, attempted data breaches, or incidents across the company's hybrid infrastructure [@Gonzalez2021]. Automated response workflows can help trigger the relevant security measures around detection based on the severity indicated by the risk register (see [3](#3-risk-register)).

# 6 References
