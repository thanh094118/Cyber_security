# Network Reconnaissance & Vulnerability Assessment Lab

Dự án này trình bày chi tiết quá trình thực hành rà quét mạng, phân tích lưu lượng gói tin và dò tìm lỗ hổng bảo mật trên hệ thống mục tiêu thông qua việc phân tích thực tế các kịch bản tấn công/thăm dò.

## 🎯 Mục tiêu dự án
- **Phân tích lưu lượng:** Bắt và phân tích các gói tin (ARP, TCP SYN, TCP ACK) để làm rõ cơ chế hoạt động ẩn sau các kỹ thuật quét Nmap.
- **Thu thập thông tin (Reconnaissance):** Xác định các nút mạng đang hoạt động, hệ điều hành (OS Fingerprinting) và liệt kê các dịch vụ/cổng mở (Service Enumeration).
- **Đánh giá lỗ hổng (Vulnerability Research):** Ánh xạ các dịch vụ phát hiện được (FTP, IIS, RPC) với các lỗ hổng đã được công bố (CVE) như CVE-2009-3023, CVE-2017-7269.

## 🛠️ Công cụ sử dụng
- **Nmap:** Quét cổng, nhận diện OS và dịch vụ.
- **Wireshark:** Bắt và phân tích trực tiếp lưu lượng mạng.
- **Môi trường:** Máy tấn công và máy mục tiêu (Windows Server 2003 R2).

## 📂 Cấu trúc dự án
- `/reports`: Chứa báo cáo phân tích chi tiết từng kịch bản kèm hình ảnh minh họa.
- `/screenshots`: Ảnh chụp kết quả thực thi Nmap và filter lưu lượng trên Wireshark.
- `/pcaps`: Các tệp lưu lượng mạng gốc để kiểm chứng.

> *Lưu ý: Dự án được thực hiện trong môi trường Lab ảo hóa, khép kín nhằm mục đích học tập và nghiên cứu an toàn thông tin.*