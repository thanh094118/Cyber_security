# Cross-Site Scripting (XSS) Testing Lab

Repository này lưu trữ tài liệu, mã nguồn và báo cáo kết quả thực hành kiểm thử lỗ hổng XSS thuộc bộ môn An toàn Thông tin. Mục tiêu là phân tích cơ chế, khai thác và phòng chống các kịch bản XSS phổ biến.

## 🎯 Trọng tâm bài thực hành
- **Phân loại XSS:** Phân tích sự khác biệt và mức độ nguy hiểm giữa Reflected XSS, Stored XSS và DOM-based XSS.
- **Kỹ thuật kiểm thử (Black-box):** Sử dụng các payload Javascript để xác định điểm yếu (vd: `<script>alert(1)</script>`).
- **Kỹ thuật vòng tránh (Bypass):** Vượt qua các bộ lọc đầu vào bằng cách đổi kiểu chữ, sử dụng HTML Entities, mã Unicode (`fromCharCode`), Hexa Encoding và chèn ký tự đặc biệt (null byte, tab).
- **Công cụ hỗ trợ:** Sử dụng **Burp Suite** (Intercept, Repeater) để đánh chặn và chỉnh sửa các HTTP Request (GET/POST) nhằm vượt qua các giới hạn form ở client.

## 📂 Cấu trúc Repository
- `/environments`: Mã nguồn các bài lab XSS (DVWA và custom lab).
- `/reports`: Báo cáo chi tiết các kịch bản khai thác XSS thành công.
- `/images`: Minh chứng thực thi mã độc Javascript và cấu trúc request bị can thiệp.