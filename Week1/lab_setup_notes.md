# Week 1 – Lab Environment Setup Notes

## Environment Configuration

### Operating System
- Primary: Kali Linux (or WSL2 with Ubuntu on Windows)
- Reason: Pre-installed security tools, compatible with Python security libraries

### Python Environment
```bash
# Check Python version
python3 --version  # Should be 3.8+

# Install required libraries
pip install requests
pip install python-nmap
pip install colorama
pip install beautifulsoup4
pip install urllib3
```

### Network Testing Lab
- Set up a local virtual network using VirtualBox or VMware
- Installed Metasploitable2 as a vulnerable target VM
- Host-only network adapter configured (no internet exposure)
- Target IP: 192.168.56.101 (example, varies per setup)

### Tools Verified
| Tool | Version | Purpose |
|------|---------|---------|
| Python | 3.11+ | Scripting |
| nmap | 7.94 | Port scanning reference |
| Wireshark | 4.x | Packet analysis |
| Burp Suite Community | 2024 | Web proxy/scanner |
| OWASP WebGoat | Latest | Web vuln practice target |

## Security Fundamentals Reviewed

### Networking Concepts
- OSI Model layers and their relevance to security
- TCP Three-way Handshake (SYN → SYN-ACK → ACK)
- UDP vs TCP: connection-oriented vs connectionless
- Common ports: 21(FTP), 22(SSH), 23(Telnet), 25(SMTP), 53(DNS), 80(HTTP), 443(HTTPS), 3306(MySQL), 8080(HTTP-alt)

### OWASP Top 10 (2021) Summary
1. A01 - Broken Access Control
2. A02 - Cryptographic Failures
3. A03 - Injection (SQLi, XSS)
4. A04 - Insecure Design
5. A05 - Security Misconfiguration
6. A06 - Vulnerable and Outdated Components
7. A07 - Identification and Authentication Failures
8. A08 - Software and Data Integrity Failures
9. A09 - Security Logging and Monitoring Failures
10. A10 - Server-Side Request Forgery (SSRF)

## Resources Used
- TryHackMe: Pre-Security & Jr Penetration Tester paths
- PortSwigger Web Security Academy (free labs)
- Python Docs: socket module
- OWASP official documentation

---
*Week 1 Setup Complete*
