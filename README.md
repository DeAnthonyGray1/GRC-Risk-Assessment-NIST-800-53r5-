# Enterprise Risk Assessment – (NIST 800-53 Based Analysis)

## 📌 Overview
This project presents an **Access Controls Risk Assessment** focused on the **Principle of Least Privilege (AC-6)** in a simulated enterprise environment (DWFinancial LLC) based on the NIST 800-53 framework.

The assessment was conducted through structured interviews with organizational stakeholders to evaluate how access control policies are implemented, enforced, and monitored within a cloud-based environment (Microsoft Azure AD).

---

## 🎯 Objectives
- Evaluate implementation of least privilege (AC-6)
- Identify risks related to privileged account usage
- Assess role-based access control (RBAC) effectiveness
- Detect privilege creep and access control gaps
- Recommend remediation strategies aligned with best practices

---

## 🧠 Methodology
1. Conducted stakeholder interviews (CISO & IT Manager)
2. Mapped responses to NIST 800-53 AC-6 controls
3. Identified control weaknesses and gaps
4. Assessed risk level based on likelihood and impact
5. Provided actionable security recommendations

---

## 🏢 Environment
- Identity Platform: Microsoft Azure AD
- Access Control Model: Role-Based Access Control (RBAC)
- Logging: Azure Activity Logs
- External Access: Azure B2B Guest Accounts

---

## 🔍 Key Findings

### 🔴 High Risk
- **Privileged Account Misuse (AC-6(2))**
  - Admin users operate with elevated privileges at all times
  - No separation between standard and privileged accounts
  - Increases risk of credential compromise and insider misuse
    
<img width="975" height="328" alt="image" src="https://github.com/user-attachments/assets/88a097f2-213e-4502-9ffc-ba6fb99fef34" />

---

### 🟠 Medium Risk
- **Privilege Creep (AC-6(7))**
  - 2 out of 10 users retained admin access after role changes
  - Indicates lack of strict access review enforcement

<img width="975" height="311" alt="image" src="https://github.com/user-attachments/assets/7390ce4e-5b3b-447a-b25c-5294b3b3e22f" />

---

### 🟢 Low Risk / Strong Controls
- RBAC enforced using Azure AD
- Network segmentation implemented across departments
- Privileged activity logging enabled
- External users restricted from privileged access
- Standard users blocked from admin-level actions

---

## 📊 Risk Summary

| Risk | Likelihood | Impact | Risk Level |
|------|-----------|--------|-----------|
| Admin Privilege Misuse | High | High | Critical |
| Privilege Creep | Medium | Medium | Moderate |

---

## 🛠️ Recommendations

### 1. Enforce Privileged Access Separation
- Require admins to use:
  - Standard accounts for daily tasks
  - Privileged accounts only for admin functions

---

### 2. Implement Just-In-Time (JIT) Access
- Use temporary privilege elevation
- Reduce standing administrative permissions

---

### 3. Strengthen Access Reviews
- Automate periodic access reviews
- Immediately revoke unnecessary privileges

---

### 4. Enhance Monitoring & Alerting
- Integrate logs into a SIEM
- Alert on abnormal privileged activity

---

## 📚 Framework Alignment
- NIST 800-53 Rev. 5 (AC-6)
- Principle of Least Privilege
- Zero Trust Security Model

---

## 💡 Scenario Context
This project simulates a **mid-sized financial organization in a cloud-based Azure environment**, assessing risks related to identity and access management practices.

---

## 📎 Project Files Included
- [Risk Assessment Report](https://drive.google.com/file/d/1HLhxNpapLyLcUZk7JzA5lcI6NtcF1aZf/view?usp=sharing)
- [Full Risk Assessment Summary](https://docs.google.com/spreadsheets/d/1zHSlKP0AMgpbTST3KnfPR8FpNikLTHO4/edit?usp=sharing&ouid=100885669222029425588&rtpof=true&sd=true)
- [Risk Register](https://docs.google.com/spreadsheets/d/1IlQL6vAVhxLdiG7OTHtAEmCQJCvtM-qe/edit?usp=sharing&ouid=100885669222029425588&rtpof=true&sd=true)
- [Interview Notes (Audit Evidence)](https://docs.google.com/document/d/1tWOVj9zdE9HisH21zs718cHpE8PcIh7i/edit?usp=sharing&ouid=100885669222029425588&rtpof=true&sd=true)

---

## 🚀 Skills Demonstrated
- GRC Risk Assessment
- NIST Control Mapping
- Access Control Analysis
- Risk Identification & Prioritization
- Security Recommendations
