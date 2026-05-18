# TryHackMe – OWASP Juice Shop Walkthrough Summary

## 🧾 Overview

The OWASP Juice Shop room is a deliberately vulnerable web application designed to demonstrate common web security flaws listed in the OWASP Top 10. The exercise focuses on hands-on exploitation of vulnerabilities such as information disclosure, SQL injection, and broken authentication mechanisms.

---

## 🔑 Key Findings

### 🔎 1. Information Disclosure

* Sensitive information was exposed through normal application features such as product reviews and search functionality.
* Administrator email addresses and internal references were accessible without authentication.

### 🔍 2. Insecure Search Functionality

* The search feature used a visible URL parameter (`q`) that could be analyzed directly from the browser.
* This revealed backend query behavior and indicated possible injection points.

### 🔓 3. Broken Authentication

* The login system was vulnerable to SQL Injection.
* Authentication could be bypassed using crafted SQL payloads that always evaluated as true.

### 💉 4. SQL Injection Vulnerability

* User input was not properly sanitized before being processed by the backend database.
* This allowed attackers to manipulate SQL queries and gain unauthorized access, including administrator-level access.

---

## ⚠️ Security Impact

### 🚨 Unauthorized Access

Attackers could bypass authentication and access privileged user accounts without valid credentials.

### 📂 Data Breach Risk

Sensitive user information and application data could be exposed or extracted from the database.

### ⬆️ Privilege Escalation

Administrative access provided attackers with full control over application functionality and user management.

### 🏢 Reputation Damage

Exploitation of these vulnerabilities could damage organizational credibility and reduce user trust.

### 🛠️ System Integrity Threats

Attackers could potentially modify, delete, or manipulate database records, leading to corruption or permanent data loss.

---

## 🛡️ Remediation Recommendations

### 🔧 1. Input Validation & Sanitization

* Validate and sanitize all user input properly.
* Use allowlists instead of blocklists whenever possible.

### 🔐 2. Use Parameterized Queries

* Replace dynamic SQL queries with prepared statements or parameterized queries.
* Treat all user input strictly as data.

### 👤 3. Secure Authentication Mechanisms

* Implement secure authentication frameworks and best practices.
* Avoid embedding raw user input directly into database queries.

### ⚠️ 4. Improve Error Handling

* Do not expose detailed system or database errors to users.
* Use generic error messages to reduce information leakage.

### 🧪 5. Regular Security Testing

* Perform regular penetration testing and vulnerability assessments.
* Integrate SAST and DAST tools into the development pipeline.

---

## 📌 Conclusion

The OWASP Juice Shop lab demonstrates how improper input handling and insecure authentication mechanisms can lead to critical vulnerabilities such as SQL injection and unauthorized access. The exercise highlights the importance of secure coding practices, proper validation, and continuous security testing to protect modern web applications.
