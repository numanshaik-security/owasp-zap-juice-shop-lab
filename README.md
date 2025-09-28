# OWASP ZAP Juice Shop Lab

This repo contains my 3rd lab where I used **OWASP ZAP** to scan the **OWASP Juice Shop** application for vulnerabilities. The goal was to practice running automated scans, analyzing results, and documenting the findings.

---

## Setup
- **OS:** Kali Linux (VirtualBox)  
- **Target app:** OWASP Juice Shop (`http://localhost:3000`)  
- **Tool:** OWASP ZAP 2.16.1  

I ran Juice Shop locally and connected ZAP to scan it.

---

## What I Did
1. Opened OWASP ZAP and set the target URL to `http://localhost:3000`.
2. Used the **Spider** and **Ajax Spider** to crawl the application.
3. Ran an **Active Scan** to test for vulnerabilities.
4. Checked the results in:
   - History tab  
   - Alerts tab  
   - WebSockets tab  
5. Exported the full scan report as HTML.

---

## Findings
- ZAP detected several issues, including:
  - Open Redirect
  - CSP Header Not Set
  - Cross-Domain Misconfiguration
  - Session ID in URL Rewrite
  - Vulnerable JS Library  
- I was also able to solve Juice Shop challenges like:
  - Accessing a confidential document  
  - Triggering error handling flaws  

---

## Repo Contents
- **Owasp-Zap-Report-.html** → Full ZAP scan report  
- **/screenshots** → Contains important screenshots from ZAP and Juice Shop during the test  
- **README.md** → This file  

---

## References
- [OWASP ZAP](https://www.zaproxy.org/)  
- [OWASP Juice Shop](https://owasp.org/www-project-juice-shop/)  
