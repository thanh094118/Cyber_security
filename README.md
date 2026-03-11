# Skill + Tools + Tech

<p align="left">
  <a href="https://www.linux.org"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" width="40" height="40" title="Linux"/></a>
  <a href="https://ubuntu.com/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/ubuntu/ubuntu-plain.svg" width="40" height="40" title="Ubuntu"/></a>
  <a href="https://www.virtualbox.org/"><img src="https://cdn.simpleicons.org/virtualbox/183A61" width="40" height="40" title="VirtualBox"/></a>
  <a href="https://www.wireshark.org"><img src="https://www.vectorlogo.zone/logos/wireshark/wireshark-icon.svg" width="40" height="40" title="Wireshark"/></a>
  <a href="https://www.kali.org"><img src="https://cdn.simpleicons.org/kalilinux/557C94" width="40" height="40" title="Kali Linux"/></a>
  <a href="https://nmap.org/"><img src="https://cdn.simpleicons.org/nmap/000000" width="40" height="40" title="Nmap"/></a>
  <a href="https://portswigger.net/burp"><img src="https://cdn.simpleicons.org/burpsuite/FF6633" width="40" height="40" title="Burp Suite"/></a>
  <a href="https://www.mysql.com/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" width="40" height="40" title="MySQL"/></a>
  <a href="https://www.php.net/"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/php/php-original.svg" width="40" height="40" title="PHP"/></a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" width="40" height="40" title="JavaScript"/></a>
</p>

# Network & Web Security Lab

Repo tổng hợp các kỹ thuật từ các bài lab an toàn thông tin, triển khai trên môi trường ảo hóa khép kín. Dự án mô phỏng thực tế các kịch bản tấn công (Red Team) và phân tích phòng thủ (Blue Team/SOC).



## Tổng quan Kịch bản & Hoạt động

- **Pentest Activities (Red Team):**
  - **Reconnaissance:** Quét mạng, dò tìm hệ điều hành, ánh xạ dịch vụ và CVE bằng Nmap.
  - **Network Exploitation:** Khai thác lỗ hổng phân giải giao thức (ARP Cache Poisoning, DNS Cache Poisoning/Kaminsky) để thực thi Man-in-the-Middle (MITM).
  - **Availability Attacks:** Triển khai DoS/DDoS (Ping of Death, TCP SYN Flood, DNS Amplification).
  - **Web Exploitation:** Khai thác các lỗ hổng ứng dụng web phổ biến (SQL Injection, XSS, CSRF) để bypass xác thực và trích xuất dữ liệu.
- **SOC & Defense Activities (Blue Team):**
  - **Traffic Analysis:** Giám sát, bắt gói tin và phân tích sâu (Deep Packet Inspection) bằng Wireshark để truy vết IP giả mạo và dấu hiệu tấn công.
  - **System Monitoring:** Đánh giá mức độ cạn kiệt tài nguyên (CPU, RAM, Bandwidth) bằng `top` và `iftop` dưới áp lực của DDoS.
  - **Mitigation:** Triển khai các chốt chặn an ninh mạng như bảng ARP tĩnh, ngẫu nhiên hóa cổng nguồn (Source Port Randomization) và phân tích các cơ chế lọc đầu vào (Input Sanitization).

## Summary of Skills & Technologies

- **Security Domains:** Network Recon, L2/L7 MITM, Reflection/Amplification DDoS, Web Application Security (OWASP Top 10).
- **Tools used:** Nmap, Wireshark, Burp Suite, CSRFTester, `dig`, `top`, `iftop`.
- **Networking Protocols:** TCP/IP, UDP, ICMP, ARP, DNS, HTTP/HTTPS.
- **OS & Infrastructure:** Linux (Ubuntu/Xubuntu), Windows Server, Oracle VirtualBox (NAT, Host-only Networking), Apache, MySQL, PHP.
