
# 🛡️ TryHackMe Jr Penetration Tester Learning Path and Hack the Box challange

# 👨‍💻 Cybersecurity Learning Log

Welcome to my cybersecurity learning log! This repository showcases hands-on labs, challenges, and core concepts I've completed through **TryHackMe** and other sources, with a focus on developing and demonstrating my skills as an aspiring penetration tester. Each entry reflects real-world techniques, tools, and methodologies—including reconnaissance, exploitation, and post-exploitation—aligned with industry best practices and certification standards.

🌐 This repo serves as a living portfolio of my progress and passion for ethical hacking, technical problem-solving, and continuous learning in the field of cybersecurity.


## ✅ Completed Modules

Here are the modules I've completed so far:

- 🔍 **Passive Reconnaissance** – Leveraging OSINT to gather intel without touching targets directly.
- 🎯 **Active Reconnaissance** – Probing live systems using tools like Nmap and Gobuster.
- 🌐 **Content Discovery** – Discovering hidden files and directories in web applications.
- 🌎 **Subdomain Enumeration** – Mapping a broader attack surface via subdomain discovery.
- 🔓 **Authentication Bypass** – Exploiting weak authentication mechanisms to gain unauthorized access.
- 🔄 **Insecure Direct Object Reference (IDOR)** – Accessing unintended resources through insecure parameter handling.
- 🗂️ **File Inclusion** – Exploiting local and remote file inclusion vulnerabilities.
- 🌐 **Intro to SSRF (Server-Side Request Forgery)** – Forcing servers to make internal HTTP requests.
- 💉 **SQL Injection** – Manipulating backend SQL queries to extract or modify database contents.
- **Net Sec Challange**: demenstrated passive and active reconnaissance, service and protocol enumeration ,credential brute-forcing and network-based exploitation methodology


## Hack the box challange:

🧠 Scenario
As part of KPMG’s Hack the Box challenge, I performed a targeted white-box penetration test on a newly developed Windows-based web application designed for Covid QR-code result tracking. The engagement, scoped by a formal Rules of Engagement (RoE), aimed to simulate real-world attack scenarios without impacting operational continuity.The assessment involved manual and automated testing techniques to identify critical vulnerabilities in both infrastructure and application layers. The target environment included Apache HTTPD 2.4.46 running PHP/7.3.27, and the test incorporated reconnaissance, authentication bypass, and input validation checks under strict no-DoS constraints.

🛠️ Skills Demonstrated
🔍 Reconnaissance & Enumeration

-Performed active reconnaissance using Nmap and Curl
-Identified open ports, running services, and fingerprinted OS (Windows)

🧪 Web Application Testing & Exploitation
-Used Burp Suite to intercept and analyze HTTP POST login requests
-Employed SQLmap to confirm and exploit Boolean-based and time-based blind SQL injection vulnerabilities
-Achieved admin-level access via injection on the login interface

🛡️ Security Validation & Analysis
-Evaluated session management practices; identified missing HttpOnly flag on PHPSESSID
-Attempted Cross-Site Scripting (XSS) on search, login, and user form fields—result: application not vulnerable
-Analyzed plaintext HTTP transmissions, flagging potential for MITM attacks

🧠 Tool Proficiency
-Demonstrated skilled use of Nmap, SQLmap, Curl, and Burp Suite in a real-world engagement context
-Integrated manual inspection with automated payload crafting to validate vulnerabilities

📝 Reporting & Remediation Insight
-Documented CVSS scores and provided actionable recommendations for each vulnerability
-Aligned findings with ethical guidelines and client remediation priorities

📈 Future Recommendations
To improve the application’s security posture, I recommend the customer enforce robust input sanitization—especially against SQL injection vectors—and utilize parameterized queries across all database interactions. Implementing secure cookie attributes, including HttpOnly and Secure flags, would harden session management. Traffic should be rerouted through HTTPS with a valid SSL/TLS certificate, and HTTP Strict Transport Security (HSTS) headers should be deployed to enforce encryption at the browser level. Additional layers such as a Web Application Firewall (WAF) and security headers (e.g. X-Content-Type-Options, X-Frame-Options) are vital for defending against injection and clickjacking threats. Long-term, integrating penetration testing into CI/CD workflows and adopting DevSecOps practices will drive scalable and sustainable improvements in security assurance.

📄 [Download Executive Summary](docs/Executive_Summary_KPMG.pdf)
