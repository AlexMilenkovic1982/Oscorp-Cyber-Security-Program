# Oscorp GRC Cybersecurity Assessment

This repository documents a governance, risk, and compliance (GRC) assessment conducted at Oscorp. It’s structured around the NIST Cybersecurity Framework and highlights both the current state of security controls and a practical set of improvements. The intent is to simulate the role of a Cyber Security Consultant stepping into a mid-sized organisation where foundational cyber practices are in place but not formalised.

---

## 🏢 About Oscorp

Oscorp is a research-led organisation with strong physical security and a clear business strategy, but cyber security responsibilities have been historically rolled into the general IT function. The company uses Microsoft Azure cloud infrastructure and Office 365 services, and relies heavily on SaaS platforms for business operations.

### Team Structure

- **Cyber Security Analyst** – Generalist, responding reactively to cyber threats; reports to the IT Manager.
- **Network Engineer** – Manages the firewall estate; reports to the Network Team Leader.
- **Cyber Security Consultant (this role)** – Brought in to assess posture, identify risks, and formalise governance; reports to the IT Manager.

---

## 🔍 Current Cyber Security Posture (Key Observations)

The following observations were gathered from internal discussions and documentation reviews:

- **Governance**: No formal cyber security roles defined. Cyber security responsibilities fall informally under the IT team. No cyber strategy or formal oversight at the board level.
- **Asset Management**: Asset tracking exists as a spreadsheet with serials, model info, and warranty data. No classification of assets by sensitivity or business criticality.
- **Disaster Recovery**: Regular DR testing and backup routines are in place. Business continuity planning is documented.
- **Vulnerability Management**: Qualys is available but used sporadically. Vulnerabilities are piling up without a structured remediation cycle.
- **Risk Management**: Financial risk is handled separately. There is no framework in place for identifying, classifying, or managing cyber risk.
- **Third Party Risk**: No formal process exists. Contracts are reviewed by procurement and finance, with no input from IT or security.
- **Identity & Access Management**: Active Directory is in use, but there's no privileged access management. Shared admin credentials are common, and no MFA is implemented.
- **Network Security**: Palo Alto firewalls are maintained and updated regularly. The network is segmented with VLANs, and diagrams are current.
- **Physical Security**: Strong — including vetted staff, CCTV, and 24/7 monitoring in sensitive areas.
- **Data Security**: No DLP solution. Data lives in Office 365 and Azure. The key application is a SaaS solution from Horizon Labs.
- **Policy**: A generic IT policy exists. There's no overarching information security policy, no data classification framework, and no written governance.
- **Detection & Response**: No SIEM. Incident response is limited to antivirus alerts. No formal IR plan exists.
- **Security Awareness**: Employees complete a one-off induction module. There is no ongoing training or simulated phishing activity.

---

## 📊 NIST CSF Assessment

A structured assessment was conducted using the NIST Cybersecurity Framework. Each category was scored based on current maturity, with gaps identified across all five core functions (Identify, Protect, Detect, Respond, Recover).

You can view the detailed scoring and rationale in the Excel spreadsheet:

📄 [Oscorp NIST Cyber Security Assessment.xlsx](https://docs.google.com/spreadsheets/d/1Bvla_iRgkNlwBqxTB4T-ID766OeEFxgO/edit?usp=sharing&ouid=114160154605914535053&rtpof=true&sd=true)

The scores reflect a generally reactive security posture. Most controls are informal, undocumented, or inconsistently applied. Detect and Respond were the lowest scoring functions, reflecting the absence of SIEM and incident playbooks.

---

## ✅ Recommendations

Recommendations are prioritised based on risk, feasibility, and their impact on overall security maturity.

### 1. Cyber Security Governance

- Appoint a Cyber Security Manager or CISO-level equivalent.
- Clearly define roles and responsibilities for cyber security within the organisation.
- Draft and publish a formal Information Security Policy.
- Ensure policy endorsement and visibility at the senior leadership level.
- Build a dedicated security function with defined ownership.

### 2. Asset Management

- Classify assets by sensitivity and business criticality.
- Move away from basic spreadsheets — consider building a proper CMDB.
- Set a recurring process for verifying and updating asset records.

### 3. Risk Management

- Define and document a formal cyber risk management process.
- Prioritise risks by impact and likelihood.
- Establish a risk register and keep it actively maintained.
- Include cyber risk within internal audits and the remit of the risk committee.

### 4. Third Party Risk

- Inventory all third-party providers and classify them by importance.
- Assess third parties for security controls (questionnaires, certifications, etc.).
- Introduce security reviews during procurement stages.

### 5. Identity and Access Management

- Roll out Multi-Factor Authentication (MFA) as a top priority.
- Eliminate shared admin credentials.
- Implement Role-Based Access Control (RBAC) and review entitlements quarterly.
- Apply the principle of least privilege consistently.

### 6. Security Awareness

- Move beyond a single training module — make awareness continuous.
- Run phishing simulations at least quarterly.
- Build a culture of shared accountability for cyber security.

### 7. Data Protection and DLP

- Conduct data discovery and classify information based on sensitivity.
- Use Microsoft’s native labelling tools (e.g. AIP) within Office 365.
- Consider implementing a DLP solution — Microsoft’s may be a logical fit.
- Block USB usage by default and require business justification for temporary access.

### 8. Threat Detection and Response

- Procure a SIEM solution or engage a managed security provider (MSSP).
- Write incident response playbooks tailored to the top five expected attack types.
- Run tabletop exercises with the IT team and relevant business units.

---

## 🗂 Repo Structure


