# Network Reconnaissance & Man-in-the-Middle Lab

Repository này lưu trữ báo cáo và minh chứng cho bài thực hành An toàn mạng, bao gồm hai giai đoạn: rà quét thông tin hệ thống và tấn công/phòng thủ phân giải địa chỉ MAC.

## 🎯 Trọng tâm bài Lab

**1. Thu thập thông tin & Rà quét lỗ hổng (Nmap)**
- Phân tích lưu lượng thăm dò mạng qua các kỹ thuật: ARP Ping, TCP SYN, TCP ACK Scan.
- Fingerprinting hệ điều hành mục tiêu (Windows Server 2003 R2) và liệt kê dịch vụ (FTP, IIS, RPC).
- Ánh xạ dịch vụ phát hiện được với các lỗ hổng đã công bố (CVE-2009-3023, CVE-2017-7269,...).

**2. Tấn công ARP Cache Poisoning & MITM (Wireshark)**
- Phân tích pcap làm rõ cơ chế giả mạo gói tin ARP Reply/Request trong mạng Container (User - Attacker - Server).
- Thực thi Man-in-the-Middle: Chặn bắt và sửa đổi trực tiếp payload thông điệp (chuyển chữ thường thành chữ hoa) trên đường truyền.
- Triển khai biện pháp phòng thủ bằng cách thiết lập bảng ánh xạ ARP tĩnh (`arp -s`).

## 📂 Cấu trúc Repository
- `/01_Nmap_Recon_and_Vuln`: Báo cáo phân tích Nmap, nhận diện OS/Dịch vụ và thông tin CVE.
- `/02_ARP_Poisoning_MITM`: Báo cáo phân tích Wireshark, ảnh minh chứng đầu độc ARP, sửa payload và file `.pcap`.