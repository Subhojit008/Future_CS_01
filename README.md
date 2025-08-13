# 🛡️ Future_CS_01 – Web Application Security Testing

**Author:** Manne Subhojit  
**Date:** 13/08/2025  

## 📌 About the Project
This project was completed as part of the **Future Interns Cybersecurity Task 1**.  
The goal was to perform **Web Application Vulnerability Assessment** on a test application and identify potential security issues following the **OWASP Top 10** framework.  

The findings were documented in a **Professional Security Assessment Report** with evidence and mitigation steps.

---

## 🎯 Objectives
- Identify vulnerabilities in a web application.
- Test for **SQL Injection**, **Cross-Site Scripting (XSS)**, and **Authentication Flaws**.
- Use ethical hacking tools to simulate real-world attacks.
- Provide fixes for each vulnerability.

---

## 🛠 Tools Used
- **SQLMap** – Automated SQL Injection exploitation tool.
- **Burp Suite (Community Edition)** – Web proxy and testing toolkit.
- **Web Browser** – Manual testing and verification.
- **Linux Terminal** – Command execution environment.

---

## 🔍 Testing Methodology
1. **Target Selection** – Chose `test.vuln.com` (intentionally vulnerable).
2. **SQL Injection Test** – Used SQLMap to enumerate databases, tables, and columns, and dump sensitive data.
3. **XSS Test** – Injected JavaScript payload `<script>alert('XSS')</script>` into search fields to trigger alerts.
4. **Authentication Bypass Test** – Used Burp Suite to intercept and manipulate authentication requests.

---

## 📊 Findings

| Vulnerability            | OWASP ID   | Risk Level | Evidence                                | Fix Recommendation |
|--------------------------|------------|-----------|-----------------------------------------|--------------------|
| SQL Injection            | A03:2021   | High      | `SQLMAP injection screenshot`           | Use prepared statements & parameterized queries. |
| Cross-Site Scripting(XSS)| A07:2021   | Medium    | JavaScript alert pop-up on search field | Implement input sanitization & output encoding. |
| Authentication Flaws     | A01:2021   | High      | `Authentication flaws.png`              | Use strong authentication, rate-limiting, and secure session handling. |

---

## 📄 Deliverables
- **[Future_CS_01_Security_Report.pdf](Future_CS_01_Security_Report.pdf)** – Detailed report with screenshots and recommendations.
- **Evidence Screenshots:**
  - SQLMAP injection proof
  - XSS proof
  - Authentication bypass proof

---

## ✅ Conclusion
The testing revealed **critical vulnerabilities** that could lead to data breaches and account compromise if left unpatched.  
Immediate remediation is recommended to enhance the security posture of the application.

---

## 📚 References
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- SQLMap Documentation
- Burp Suite Community Edition

---
**Disclaimer:** This assessment was conducted on an authorized test environment for educational purposes only.
