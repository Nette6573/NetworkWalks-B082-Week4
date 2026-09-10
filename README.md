# 🔐 NetworkWalks B082 — Week 4

## Mediroza General Hospital — Authorized Black-Box Penetration Testing

This repository documents my Week 4 penetration testing project completed as
part of the **NetworkWalks Cybersecurity Internship — Batch B082**.

The assessment was conducted within the authorized NetworkWalks training
environment against the assigned Mediroza General Hospital target.

The project covered reconnaissance, web application assessment,
authentication testing, protected-document recovery, sensitive-data exposure
analysis, evidence collection, risk assessment, remediation planning, and
professional security reporting.

---

## 🎯 Project Objectives

The assessment consisted of four milestones:

| Milestone | Objective | Status |
|---|---|---|
| M1 | Retrieve three confidential patient PDF laboratory reports | ✅ Completed |
| M2 | Recover access to all three protected PDF reports | ✅ Completed |
| M3 | Identify employee salary and shareholder information | ✅ Completed |
| M4 | Produce a professional penetration testing report | ✅ Completed |

### Final Result

**4/4 Milestones Completed**

---

## 🔎 M1 — Initial Access

The assessment began with reconnaissance, web application mapping and
authentication analysis.

The Patient Portal was identified as a relevant application entry point.
Authentication responses were examined and multiple testing approaches were
used.

An earlier constrained automated SQL injection test did not identify the
successful condition. Further manual analysis of the authentication behavior
led to identification and validation of an authentication-bypass SQL
injection within the authorized training environment.

Following successful authentication, three confidential patient PDF reports
were retrieved.

### Evidence

Sanitized evidence demonstrates:

- Patient Portal discovery
- Authentication testing
- Authentication weakness validation
- Successful authenticated access
- Retrieval of three PDF reports

---

## 🔐 M2 — PDF Password Recovery

The three retrieved PDF reports were individually assessed.

PDF hashes were extracted using the NetworkWalks Hash Calculator and
dictionary-based password recovery was performed using the NetworkWalks
Password Cracker.

Successful recovery was achieved for all three documents and each document
was subsequently opened and validated.

### Evidence

Sanitized evidence demonstrates:

- PDF hash extraction
- Successful password recovery for PDF 1
- Successful password recovery for PDF 2
- Successful password recovery for PDF 3
- Successful opening of all three PDFs

Passwords, hashes, patient identities and medical information have been
redacted.

---

## 🚨 M3 — Critical Data Exposure

An SQL database backup was identified in a web-accessible location.

The backup was retrieved and examined within the authorized assessment
environment.

Analysis identified database structures containing sensitive staff and
shareholder information.

The exposed information included categories such as:

- Employee identity information
- Job and department information
- Contact information
- National identification information
- Salary-related information
- Shareholder information
- Ownership and share-class structures

Sensitive values have been removed from this public repository.

---

## 📄 M4 — Professional Security Report

The final milestone was the preparation of a professional penetration
testing report documenting the assessment.

The report includes:

- Executive summary
- Scope and authorization
- Assessment objectives
- Methodology
- Tools and techniques
- Chronological testing narrative
- Findings and risk ratings
- Evidence register
- Remediation recommendations
- Testing limitations
- Lessons learned
- Evidence handling and redaction
- Conclusion

The final report is available in the `Report/` directory.

---

## 🛠️ Tools & Techniques

Tools evidenced during the assessment included:

- WHOIS
- nslookup
- WhatWeb
- curl
- WAFW00F
- DNSRecon
- theHarvester
- Gobuster
- Browser/Firefox
- HTML inspection
- SQLMap
- Hydra
- NetworkWalks Hash Calculator
- NetworkWalks Password Cracker
- Manual authentication testing
- Evidence preservation and sanitization

---

## 💡 Key Lessons Learned

### Manual analysis matters

Automated testing is valuable, but a negative automated result does not
necessarily demonstrate that an application is secure.

### Penetration testing is not always linear

M3 was completed before M1 and M2. The assessment demonstrated that findings
can emerge in different stages of an investigation.

### Evidence matters

Successful security testing requires clear evidence demonstrating how a
finding was identified, validated and documented.

### Security weaknesses can compound

Authentication weaknesses and exposed sensitive resources can combine to
create significantly greater security impact.

### Responsible handling is part of security work

Sensitive evidence must be carefully reviewed and sanitized before being
shared publicly.

---

## 🔐 Evidence Sanitization

This repository contains **sanitized portfolio evidence only**.

The following have been removed or redacted:

- Credentials
- Recovered passwords
- Password hashes
- Patient names and identifiers
- Medical and clinical information
- Employee personal information
- National identification numbers
- Salary values
- Shareholder values
- Sensitive infrastructure information
- Other unnecessary confidential information

The original chronological evidence workbook is retained separately.

---

## ⚠️ Authorized Training Environment

All testing documented in this repository was performed within the
authorized NetworkWalks training environment for educational purposes.

The techniques described in this repository are dual-use and must only be
applied to systems, accounts and files for which explicit authorization
exists.

---

## 📁 Repository Structure

```text
NetworkWalks-B082-Week4/
│
├── README.md
├── SECURITY-NOTICE.md
│
├── M1-Initial-Access/
│   ├── README.md
│   └── Screenshots/
│
├── M2-PDF-Recovery/
│   ├── README.md
│   └── Screenshots/
│
├── M3-Critical-Data-Exposure/
│   ├── README.md
│   └── Screenshots/
│
└── Report/
    └── Antoinette-Thompson-Mediroza-Week4-Pentest-Report.pdf

```



👩🏽‍💻 Author

Antoinette Thompson

NetworkWalks Cybersecurity Internship
Batch B082

Cybersecurity | Information Technology | Security+
