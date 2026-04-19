# Bài Thực Hành 5: Kiểm thử lỗ hổng SQL Injection

Repository này lưu trữ tài liệu, mã nguồn và báo cáo kết quả thực hành kiểm thử lỗ hổng SQL Injection (SQLi) thuộc bộ môn An toàn Thông tin. Mục tiêu nhằm hiểu rõ cơ chế, phương pháp phát hiện, khai thác và phòng chống lỗ hổng SQLi trên ứng dụng Web.
đắ
## 🎯 Trọng tâm bài thực hành
- **Triển khai môi trường:** Cài đặt và cấu hình máy ảo Linux (Ubuntu 32-bit) trên VirtualBox, thiết lập Web Server (Apache/PHP/MySQL) với mã nguồn chứa lỗ hổng chủ đích.
- **Sử dụng công cụ:** Làm quen và ứng dụng **Burp Suite** (Intercepting Proxy, Repeater, Decoder) để bắt, chỉnh sửa và phân tích các HTTP Request/Response phục vụ kiểm thử hộp đen.
- **Kỹ thuật kiểm thử SQLi:** - Phân tích tham số đầu vào (GET, POST, Header, Cookie) và phán đoán kiểu truy vấn (SELECT, INSERT).
    - Thực hiện các kỹ thuật khai thác: Error-based, Tautology-based, UNION-based, Order By, và Blind SQL Injection (Boolean-based, Time-based).
    - Thử nghiệm các kỹ thuật vòng tránh (Bypass) bộ lọc đầu vào (URL Encoding, Hexa Encoding, Null byte, Char function).

## 📂 Cấu trúc Repository
- `/docs`: Tài liệu hướng dẫn thực hành.
- `/environments`: Database script (`webvul.sql`) và mã nguồn bài lab.
- `/reports`: Báo cáo chi tiết các bước kiểm thử trên mục tiêu `http://webvul.bkcs.vn` (hoặc localhost) kèm giải thích.
- `/images`: Ảnh chụp màn hình minh chứng kết quả truy vấn, thông báo lỗi và giao diện công cụ.
