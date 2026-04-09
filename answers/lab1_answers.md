# Lab 01 Answers

## CIA & Risk: Hệ thống lưu điểm

**Họ và tên:** La Văn Hải

**MSSV:** 1871020215

**Lớp/Nhóm:** CNTT 18-01

---

## 1. Assets

Liệt kê ít nhất 2 assets cần bảo vệ.

- Asset 1:Dữ liệu người dùng (tên, mật khẩu)
- Asset 2:Hệ thống website/ứng dụng
- Asset 3 (nếu có):

---

## 2. Mapping CIA

Ghép từng sự cố với CIA.

- Sự cố A -> Confidentiality (lộ mật khẩu người dùng)
- Sự cố B -> Integrity (dữ liệu bị sửa sai)
- Sự cố C -> Availability (web bị sập, không truy cập được)

---

## 3. Phân tích sự cố B

- Threat: Hacker chỉnh sửa dữ liệu hoặc lỗi từ người dùng
- Vulnerability:
  Không kiểm tra dữ liệu nhập vào
  Không có phân quyền rõ ràng
- Mitigation:
  Kiểm tra dữ liệu đầu vào (validation)
  Phân quyền người dùng
  Sao lưu dữ liệu định kỳ

---

## 4. Reflection

Qua bài này, em hiểu được tầm quan trọng của việc bảo vệ hệ thống thông tin. Ba yếu tố Confidentiality, Integrity và Availability đều cần thiết để hệ thống hoạt động ổn định. Nếu thiếu một trong ba yếu tố, hệ thống có thể gặp rủi ro nghiêm trọng. Việc xác định threat, vulnerability và mitigation giúp em biết cách phòng tránh các sự cố. Điều này rất hữu ích khi xây dựng các hệ thống đơn giản trong thực tế.

---

## 5. Bonus Flag

`FIT4012{A-?-B-?-C-?}`

Flag của em: FIT4012{A-C-B-I-C-A}
