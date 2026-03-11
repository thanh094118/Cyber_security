# DNS Cache Poisoning (Kaminsky Attack) Analysis

Repository này trình bày quá trình mô phỏng, phân tích lưu lượng và triển khai biện pháp phòng chống cuộc tấn công đầu độc bộ nhớ cache DNS (biến thể Dan Kaminsky) trên hệ thống Local DNS Server.

## 🎯 Trọng tâm bài Lab

**1. Mô phỏng cơ chế tấn công Kaminsky**
- Khai thác lỗ hổng bằng cách liên tục truy vấn các subdomain không tồn tại (random subdomains) để ép Local DNS Server tạo kết nối ra bên ngoài, tránh việc sử dụng cache cũ.
- Chế tạo (craft) và đẩy hàng loạt thông điệp DNS Response giả mạo bản ghi NS với các giá trị Query ID ngẫu nhiên nhằm thắng bước "Race Condition" trước DNS Server thực.

**2. Phân tích lưu lượng (Wireshark & Dig)**
- Theo dõi vòng đời của DNS Query/Response, xác định chính xác gói tin giả mạo lọt qua lớp xác thực (khớp Query ID và đến sớm nhất).
- Xác minh kết quả tấn công thông qua việc trích xuất bộ đệm (cache dump) và kiểm tra phân giải tên miền bằng lệnh `dig`.

**3. Triển khai phòng thủ (Mitigation)**
- Phân tích hiệu quả của kỹ thuật Source Port Randomization (Ngẫu nhiên hóa cổng nguồn).
- Cấu hình và dùng Wireshark chứng minh việc Attacker thất bại khi phải đoán đồng thời cả Query ID và Source Port.

## 📂 Cấu trúc Repository
- `/report`: Báo cáo chi tiết kịch bản tấn công, phân tích nguyên nhân và hậu quả.
- `/images` & `/pcaps`: Ảnh chụp thực tế kết quả hệ thống, lưu lượng mạng và tệp capture gốc.