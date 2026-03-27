# Capstone Testing Project – CyberSoft E-Learning Platform

> **Manual Testing & API Testing** | CyberSoft Academy – Testing 14

## Tổng quan dự án

| Mục tiêu | Chi tiết |
|---|---|
| **Ứng dụng kiểm thử** | CyberSoft E-Learning Platform |
| **URL** | https://demo2.cybersoft.edu.vn |
| **Phạm vi** | Module Thông tin cá nhân (UI + API) |
| **Loại kiểm thử** | Manual Testing, API Testing (REST) |
| **Công cụ** | Browser DevTools, Postman, Jira |
| **Tester** | Trúc Anh |

---

## Tài liệu dự án

Các thành phần chi tiết của dự án được tổ chức như sau:

* [Phân tích yêu cầu (Requirements Analysis)](./docs/RequirementsAnalysis.md) - Chi tiết về chức năng và yêu cầu phi chức năng.
* [Danh sách Test Case chi tiết](./resources/TestCases.xlsx) - Tập tin chứa 96 test cases đầy đủ.
* [Báo cáo lỗi (Bug Reports)](../issues) - Tổng hợp toàn bộ bug từ Jira.

---

## Kết quả kiểm thử (Test Execution Summary)

### Thống kê chung

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

### Phân loại Bug theo Priority

| High | Medium | Low |
|:---:|:---:|:---:|
| 2 | 24 | 9 |

---

## Các lỗi nghiêm trọng (Key Bugs)

| ID | Mô tả lỗi | Priority |
|---|---|:---:|
| TC_88 | API cho phép cập nhật thông tin tài khoản người khác (HTTP 200) | **High** |
| TC_89 | Học viên tự nâng quyền thành Giảng viên qua API | **High** |
| TC_39 | Họ tên chỉ chứa khoảng trắng vẫn được lưu thành công | Medium |
| TC_58 | SĐT 10 chữ số hợp lệ bị báo lỗi sai định dạng | Medium |
| TC_76 | API lưu email rỗng thành công (HTTP 200) | Medium |

---

## Kỹ năng thể hiện

* Phân tích yêu cầu nghiệp vụ từ hệ thống thực tế.
* Kiểm thử giao diện (UI): Layout, Responsive, Validation.
* Kiểm thử API (REST): Thực thi GET/PUT/DELETE, kiểm tra Authentication & Authorization.
* Tư duy bảo mật: Phát hiện lỗi leo thang đặc quyền và truy cập dữ liệu trái phép.
