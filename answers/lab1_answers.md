# Lab 01 Answers

## CIA & Risk: Hệ thống lưu điểm

**Họ và tên:** La Văn Hải

**MSSV:** 1871020215

**Lớp/Nhóm:** CNTT 18-01

---

## 1. Assets

Liệt kê ít nhất 2 assets cần bảo vệ.

- Asset 1: Dữ liệu người dùng (tên đăng nhập, mật khẩu, thông tin cá nhân)
- Asset 2: Dữ liệu điểm số của sinh viên
- Asset 3: Hệ thống website/ứng dụng quản lý điểm

---

## 2. Mapping CIA

Ghép từng sự cố với CIA.

- Sự cố A -> Confidentiality
- Sự cố B -> Integrity
- Sự cố C -> Availability

---

## 3. Phân tích sự cố B

- Threat:
  Hacker tấn công và chỉnh sửa dữ liệu
  Người dùng nhập sai hoặc cố tình sửa dữ liệu
- Vulnerability:
  Không kiểm tra dữ liệu đầu vào (input validation yếu)
  Không phân quyền rõ ràng giữa người dùng và quản trị viên
  Thiếu cơ chế ghi log hoặc kiểm tra thay đổi dữ liệu
- Mitigation:
  Kiểm tra và xác thực dữ liệu đầu vào (validation)
  Áp dụng phân quyền (role-based access control)
  Ghi log hoạt động để theo dõi thay đổi
  Sao lưu dữ liệu định kỳ (backup)

---

## 4. Reflection

Qua bài này, em hiểu được tầm quan trọng của việc bảo vệ hệ thống thông tin. Ba yếu tố Confidentiality, Integrity và Availability đều cần thiết để hệ thống hoạt động ổn định. Nếu thiếu một trong ba yếu tố, hệ thống có thể gặp rủi ro nghiêm trọng. Việc xác định threat, vulnerability và mitigation giúp em biết cách phòng tránh các sự cố. Điều này rất hữu ích khi xây dựng các hệ thống đơn giản trong thực tế.

---

## 5. Bonus Flag

`FIT4012{A-?-B-?-C-?}`

Flag của em: FIT4012{A-C-B-I-C-A}
