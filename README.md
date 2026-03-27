[Cybersoft Capstone] Kiểm thử hệ thống quản lý khóa học Cybersoft (Manual & API Testing)

# Capstone Testing Project – CyberSoft E-Learning Platform

> **Manual Testing & API Testing** | CyberSoft Academy – Testing 14

---

## Tổng quan dự án

| | |
|---|---|
| **Ứng dụng kiểm thử** | CyberSoft E-Learning Platform |
| **URL** | https://demo2.cybersoft.edu.vn |
| **Phạm vi kiểm thử** | Trang Thông tin cá nhân (UI + API) |
| **Loại kiểm thử** | Manual Testing, API Testing (REST) |
| **Công cụ** | Browser DevTools, Postman |
| **Tester** | Trúc Anh |

---

## Phân tích yêu cầu

CyberSoft E-Learning là nền tảng học lập trình trực tuyến. Phạm vi capstone tập trung vào module **Thông tin cá nhân** của học viên, bao gồm:

### Yêu cầu chức năng (Functional Requirements)

**1. Hiển thị giao diện (UI Display)**
- Trang Thông tin cá nhân hiển thị đầy đủ: Navbar, Header, left sidebar, tab bar, nội dung và Footer
- Left sidebar hiển thị avatar, họ tên, vị trí công việc và nút Hồ sơ cá nhân
- Mục Thông tin cá nhân hiển thị: Email, Họ tên, SĐT, Tài khoản, Nhóm, Đối tượng
- Mục Kỹ năng hiển thị danh sách kỹ năng với progress bar

**2. Tab Khóa học**
- Hiển thị danh sách khóa học đã đăng ký với đầy đủ thông tin (ảnh, tên, giảng viên)
- Chức năng tìm kiếm khóa học: partial match, case-insensitive, tiếng Việt có dấu, realtime
- Chức năng Hủy khóa học có popup xác nhận trước khi thực hiện

**3. Chỉnh sửa thông tin cá nhân (Popup)**
- Popup chỉnh sửa với các trường: Họ và tên, Mật khẩu, Email, Số điện thoại
- Validation đầy đủ cho từng trường (bắt buộc, định dạng, độ dài)
- Mật khẩu tối thiểu 8 ký tự, gồm chữ hoa, chữ thường, số và ký tự đặc biệt
- Số điện thoại bắt đầu bằng "0", độ dài 10–11 chữ số

**4. API**
- `GET /ThongTinTaiKhoan` – Lấy thông tin tài khoản
- `PUT /CapNhatThongTinNguoiDung` – Cập nhật thông tin cá nhân
- `DELETE /HuyGhiDanh` – Hủy ghi danh khóa học

### Yêu cầu phi chức năng (Non-Functional Requirements)
- Responsive trên Mobile (< 768px) và Tablet (768px–1024px): không tràn layout, không scroll ngang
- API phân quyền đúng: không cho phép cập nhật tài khoản người khác hoặc tự nâng quyền

---

## Kết quả kiểm thử

### Tổng quan

| Tổng TC | Pass | Fail | Tỉ lệ Pass |
|:---:|:---:|:---:|:---:|
| 96 | 61 | 35 | 63.5% |

### Kết quả theo module

| Module | Pass | Fail | Tổng |
|---|:---:|:---:|:---:|
| Tổng quan (UI Display) | 12 | 1 | 13 |
| Tab bar / Khóa học | 13 | 2 | 15 |
| Chỉnh sửa thông tin cá nhân | 23 | 9 | 32 |
| API Testing | 10 | 23 | 33 |
| **Tổng** | **58** | **35** | **96** |

### Bug theo mức độ ưu tiên

| 🔴 High | 🟠 Medium | 🟡 Low |
|:---:|:---:|:---:|
| 2 | 24 | 9 |

---

## Bug nổi bật

> Toàn bộ bug được quản lý và tracking trên Jira; một số bug tiêu biểu đã được log lại dưới dạng GitHub Issues để minh họa quy trình làm việc thực tế.

| TC | Mô tả | Priority |
|---|---|:---:|
| TC_21 | Hủy khóa học không có popup xác nhận | Medium |
| TC_39 | Họ tên chỉ là khoảng trắng vẫn được lưu thành công | Medium |
| TC_58 | SĐT 10 chữ số hợp lệ nhưng bị báo lỗi sai định dạng | Medium |
| TC_88 | API cho phép cập nhật thông tin tài khoản người khác (HTTP 200) | **High** |
| TC_89 | Học viên (HV) tự nâng quyền thành Giảng viên (GV) qua API | **High** |
| TC_69 | API trả về 200 khi mật khẩu rỗng, không cập nhật nhưng không báo lỗi | Medium |
| TC_76 | API lưu email rỗng thành công (HTTP 200) | Medium |

---

## File đính kèm

| File | Mô tả |
|---|---|
| [`TestCases.xlsx`](./TestCases.xlsx) | Toàn bộ test case chi tiết |

---

## Kỹ năng thể hiện

- Phân tích yêu cầu và thiết kế test case từ giao diện thực tế
- Kiểm thử UI: layout, responsive, validation
- Kiểm thử API: REST API với cURL (GET / PUT / DELETE), kiểm tra authentication, authorization, boundary value
- Phát hiện lỗi bảo mật: leo thang đặc quyền, truy cập trái phép dữ liệu người dùng khác
- Viết báo cáo lỗi rõ ràng với actual result vs expected result
