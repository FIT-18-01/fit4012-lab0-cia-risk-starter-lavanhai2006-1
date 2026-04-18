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

- Sự cố A -> Availability
- Sự cố B -> Integrity
- Sự cố C -> Confidentiality

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

Nếu là quản trị viên hệ thống, em sẽ ưu tiên xử lý sự cố C (lộ danh sách điểm) trước.
Lý do là dữ liệu đã bị rò rỉ ra ngoài và ảnh hưởng trực tiếp đến quyền riêng tư của sinh viên.
Sau đó em sẽ xử lý sự cố B để đảm bảo tính toàn vẹn dữ liệu điểm không bị sửa trái phép.
Tiếp theo là củng cố tính sẵn sàng để giảm tình trạng sinh viên không đăng nhập được vào thời điểm quan trọng.
Qua bài này em hiểu rõ hơn cách ưu tiên xử lý rủi ro theo mức độ ảnh hưởng trong thực tế.

---

## 5. Bonus Flag

`FIT4012{A-?-B-?-C-?}`

Flag của em: FIT4012{A-A-B-I-C-C}
