# DoS & DDoS Attacks Analysis Lab

Dự án này mô phỏng, phân tích lưu lượng và đánh giá tác động của các hình thức tấn công Từ chối dịch vụ (DoS/DDoS) lên tài nguyên hệ thống mạng, đồng thời đề xuất biện pháp phòng vệ.

## 🎯 Trọng tâm dự án
- **Giám sát tài nguyên:** Sử dụng lệnh `top` và `iftop` (Linux) để đo lường mức độ cạn kiệt CPU, RAM và Băng thông mạng trước và trong khi bị tấn công.
- **Ping of Death:** Phân tích kỹ thuật khai thác lỗ hổng phân mảnh gói tin (IP Fragmentation) bằng các gói ICMP vượt quá kích thước MTU.
- **TCP SYN Flooding:** Phân tích sự cạn kiệt bảng trạng thái kết nối do hàng loạt gói TCP SYN giả mạo IP nguồn (Spoofing) và cơ chế phòng chống (SYN Cookies).
- **DNS Amplification:** Làm rõ cơ chế tấn công phản xạ/khuếch đại (Reflection/Amplification Attack) lợi dụng máy chủ DNS để làm ngập lụt băng thông nạn nhân.

## 🛠️ Công cụ sử dụng
- **Phân tích gói tin:** Wireshark.
- **Giám sát hệ thống:** `top`, `iftop` trên môi trường Linux/Container.

## 📂 Cấu trúc Repository
- `/report`: Báo cáo phân tích chuyên sâu nguyên lý, hậu quả và cách phòng chống.
- `/images`: Ảnh chụp thực tế kết quả giám sát CPU/RAM, Băng thông và gói tin.
- `/pcaps`: Các tệp lưu lượng mạng gốc để kiểm chứng.