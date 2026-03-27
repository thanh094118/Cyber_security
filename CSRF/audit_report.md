# Cross-Site Request Forgery (CSRF) Testing Lab
  ewdwd
Repository này tập trung vào việc mô phỏng và kiểm thử lỗ hổng CSRF, minh họa cách thức kẻ tấn công ép buộc trình duyệt của người dùng hợp lệ thực hiện các hành động không mong muốn.

## 🎯 Trọng tâm bài thực hành
- **Cơ chế CSRF:** Phân tích cách kẻ tấn công lợi dụng cơ chế tự động gửi Cookie xác thực của trình duyệt để mạo danh người dùng (ví dụ: chuyển tiền, đổi mật khẩu).
- **Kịch bản khai thác:** Chế tạo các payload HTML độc hại (sử dụng thẻ `<a>`, `<img>` hoặc form tự động submit) ẩn mình dưới dạng các liên kết vô hại để lừa nạn nhân nhấp vào.
- **Công cụ hỗ trợ:** Sử dụng **CSRFTester** (OWASP) và **Burp Suite** để phân tích các HTTP Request hợp lệ, từ đó xây dựng các trang web giả mạo phục vụ tấn công.
- **Phòng chống:** Tìm hiểu các biện pháp ngăn chặn CSRF (như Anti-CSRF Tokens, SameSite Cookies).

## 📂 Cấu trúc Repository
- `/reports`: Phân tích chi tiết kịch bản lừa nạn nhân và quá trình khai thác.
- `/tools`: Công cụ CSRFTester hỗ trợ sinh mã tấn công.
- `/images`: Minh chứng sự thay đổi trạng thái (chuyển tiền thành công) và mã HTML giả mạo.
