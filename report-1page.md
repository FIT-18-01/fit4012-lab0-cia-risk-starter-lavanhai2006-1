# FIT4012 - Report 1 Page

## Lab 01 - CIA & Risk: Hệ thống lưu điểm

### 1. Mục tiêu bài lab

- Nhận diện tài sản cần bảo vệ trong một hệ thống thông tin đơn giản.
- Phân biệt Confidentiality, Integrity, Availability.
- Xác định threat, vulnerability, mitigation.
- Thực hành workflow GitHub cơ bản để nhận và nộp bài.

### 2. Cách làm

- Đọc bối cảnh và xác định các thành phần quan trọng của hệ thống.
- Phân tích từng sự cố theo bộ ba CIA.
- Chọn sự cố B để phân tích sâu hơn theo threat - vulnerability - mitigation.
- Hoàn thiện bài làm trong repo và commit/push lên GitHub.

### 3. Kết quả chính

**Assets:**

- Dữ liệu điểm sinh viên (điểm số, thông tin cá nhân)
- Tài khoản đăng nhập của giảng viên/sinh viên

**CIA mapping:**

- Sự cố A -> Availability
- Sự cố B -> Integrity
- Sự cố C -> Confidentiality

**Phân tích sự cố B:**

- Threat: Hacker hoặc người dùng chỉnh sửa điểm trái phép
- Vulnerability:
  Không có phân quyền rõ ràng
  Không kiểm tra/ghi log thay đổi dữ liệu
- Mitigation:
  Áp dụng phân quyền người dùng (RBAC)
  Ghi log và theo dõi thay đổi dữ liệu
  Kiểm tra dữ liệu đầu vào
  Sao lưu dữ liệu định kỳ

### 4. Kết luận ngắn

Qua bài lab, em hiểu rõ hơn về mô hình CIA trong bảo mật hệ thống thông tin. Phần phân tích threat, vulnerability và mitigation giúp em biết cách tìm ra nguyên nhân và giải pháp phù hợp. Khó nhất là phân biệt các sự cố theo Confidentiality, Integrity và Availability vẫn phân biệt sai các sự cố
