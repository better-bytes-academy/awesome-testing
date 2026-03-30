# Security Testing Tools

> Tổng hợp các công cụ kiểm thử bảo mật.

---

## 📌 Mục lục

- [Web Application Security](#web-application-security)
- [Network Security](#network-security)
- [Vulnerability Scanners](#vulnerability-scanners)
- [Penetration Testing](#penetration-testing)
- [OWASP Resources](#owasp-resources)

---

## Web Application Security

| Công cụ | Giá | Mô tả | Link |
|---------|-----|-------|------|
| **OWASP ZAP** | Free | Intercepting proxy, security scanning | [zaproxy.org](https://www.zaproxy.org/) |
| **Burp Suite** | Free/Paid | Web security testing platform | [portswigger.net](https://portswigger.net/burp) |
| **Nikto** | Free | Web server scanner | [github.com/sullo/nikto](https://github.com/sullo/nikto) |
| **SQLMap** | Free | Automated SQL injection tool | [sqlmap.org](https://sqlmap.org/) |
| **w3af** | Free | Web application attack and audit framework | [w3af.org](http://w3af.org/) |

---

## Network Security

| Công cụ | Giá | Mô tả | Link |
|---------|-----|-------|------|
| **Nmap** | Free | Network discovery và security auditing | [nmap.org](https://nmap.org/) |
| **Wireshark** | Free | Network protocol analyzer | [wireshark.org](https://www.wireshark.org/) |
| **Aircrack-ng** | Free | WiFi security assessment | [aircrack-ng.org](https://www.aircrack-ng.org/) |
| **Netcat** | Free | Networking utility, "Swiss army knife" | Built-in Linux/macOS |

---

## Vulnerability Scanners

| Công cụ | Giá | Mô tả | Link |
|---------|-----|-------|------|
| **Nessus** | Free/Paid | Vulnerability scanner | [tenable.com/nessus](https://www.tenable.com/products/nessus) |
| **OpenVAS** | Free | Open-source vulnerability scanner | [openvas.org](https://www.openvas.org/) |
| **Nuclei** | Free | Fast, customizable vulnerability scanner | [nuclei.projectdiscovery.io](https://nuclei.projectdiscovery.io/) |
| **Snyk** | Free/Paid | Developer-first security, dependency scanning | [snyk.io](https://snyk.io/) |
| **Trivy** | Free | Container & IaC vulnerability scanner | [aquasecurity.github.io/trivy](https://aquasecurity.github.io/trivy/) |

---

## Penetration Testing

| Công cụ | Giá | Mô tả | Link |
|---------|-----|-------|------|
| **Metasploit** | Free/Paid | Penetration testing framework | [metasploit.com](https://www.metasploit.com/) |
| **Kali Linux** | Free | Security-focused Linux distribution | [kali.org](https://www.kali.org/) |
| **Parrot OS** | Free | Security & pen testing Linux distro | [parrotsec.org](https://www.parrotsec.org/) |
| **John the Ripper** | Free | Password cracking tool | [openwall.com/john](https://www.openwall.com/john/) |
| **Hashcat** | Free | Advanced password recovery | [hashcat.net](https://hashcat.net/hashcat/) |
| **BeEF** | Free | Browser exploitation framework | [beefproject.com](http://beefproject.com/) |

---

## OWASP Resources

### OWASP Top 10 (2021)

| # | Vulnerability | Mô tả |
|---|-------------|-------|
| 1 | **Broken Access Control** | Kiểm soát truy cập không đúng |
| 2 | **Cryptographic Failures** | Lỗi mã hóa |
| 3 | **Injection** | SQL, NoSQL, OS command injection |
| 4 | **Insecure Design** | Thiết kế không an toàn |
| 5 | **Security Misconfiguration** | Cấu hình bảo mật sai |
| 6 | **Vulnerable Components** | Sử dụng thành phần có lỗ hổng |
| 7 | **Authentication Failures** | Lỗi xác thực |
| 8 | **Software & Data Integrity** | Lỗi toàn vẹn dữ liệu |
| 9 | **Security Logging Failures** | Ghi log bảo mật không đủ |
| 10 | **SSRF** | Server-Side Request Forgery |

### OWASP Testing Guide
- [OWASP Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/)

---

## 📚 Tham khảo

- [OWASP Foundation](https://owasp.org/)
- [PortSwigger Web Security Academy](https://portswigger.net/web-security) — Free học security testing
- [HackTheBox](https://www.hackthebox.com/) — Practice hacking
