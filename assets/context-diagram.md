# Context Diagram (Mô tả ngữ cảnh)

```mermaid
flowchart LR
    GV[Giảng viên] -->|Nhập điểm| HT[Hệ thống lưu điểm]
    SV[Sinh viên] -->|Đăng nhập / Xem điểm| HT
    HT --> DB[(Cơ sở dữ liệu điểm)]
    HT --> LOG[(Nhật ký hệ thống)]
```

## Gợi ý đọc sơ đồ
- **Giảng viên** là tác nhân có quyền nhập điểm.
- **Sinh viên** là tác nhân có quyền xem điểm.
- **Hệ thống lưu điểm** là nơi xử lý đăng nhập, truy vấn và hiển thị dữ liệu.
- **Cơ sở dữ liệu điểm** lưu thông tin cần bảo vệ.
- **Nhật ký hệ thống** hỗ trợ kiểm tra, truy vết sự cố.
