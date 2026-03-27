# Phân tích yêu cầu kiểm thử (Requirements Analysis)

Tài liệu này trình bày các tiêu chuẩn và yêu cầu kỹ thuật làm căn cứ để thiết kế Test Case cho module **Thông tin cá nhân** của hệ thống CyberSoft E-Learning.

## 1. Yêu cầu chức năng (Functional Requirements)

### 1.1. Hiển thị giao diện (UI Display)
* **Thành phần chung:** Hiển thị đầy đủ Navbar, Header, Left Sidebar, Tab bar và Footer.
* **Left Sidebar:** Hiển thị Avatar học viên, Họ tên, Vị trí công việc và nút Hồ sơ cá nhân.
* **Thông tin cá nhân:** Hiển thị các trường Email, Họ tên, SĐT, Tài khoản, Nhóm, Đối tượng.
* **Kỹ năng:** Danh sách kỹ năng kèm thanh tiến độ (Progress bar).

### 1.2. Quản lý khóa học (Tab Khóa học)
* **Hiển thị:** Danh sách các khóa học đã đăng ký (Ảnh, Tên khóa học, Giảng viên).
* **Tìm kiếm:** Tìm kiếm theo tên khóa học (Partial match, không phân biệt hoa thường, hỗ trợ tiếng Việt).
* **Hủy khóa học:** Phải có Popup xác nhận (Confirmation) trước khi thực hiện xóa khóa học khỏi danh sách.

### 1.3. Chỉnh sửa thông tin cá nhân
* **Trường dữ liệu:** Cho phép sửa Họ tên, Mật khẩu, Email, Số điện thoại.
* **Ràng buộc dữ liệu (Validation):**
    * Các trường thông tin không được để trống.
    * **Mật khẩu:** Tối thiểu 8 ký tự, gồm chữ hoa, chữ thường, số và ký tự đặc biệt.
    * **Số điện thoại:** Bắt đầu bằng "0", độ dài từ 10 đến 11 chữ số.
    * **Email:** Đúng định dạng email tiêu chuẩn.

### 1.4. Yêu cầu API
* `GET /ThongTinTaiKhoan`: Lấy thông tin tài khoản hiện tại.
* `PUT /CapNhatThongTinNguoiDung`: Cập nhật dữ liệu người dùng.
* `DELETE /HuyGhiDanh`: Thực hiện hủy đăng ký khóa học.

## 2. Yêu cầu phi chức năng (Non-Functional Requirements)

### 2.1. Tính tương thích và Khả năng hiển thị (Compatibility & Usability)
* **Responsive Design:** Giao diện phải tương thích với các độ phân giải phổ biến (Mobile < 768px, Tablet 768px-1024px, Desktop > 1024px).
* **Cross-browser:** Hoạt động ổn định trên Chrome, Edge, Firefox và Safari.
* **UI/UX Consistency:** Màu sắc, font chữ và kích thước nút bấm phải đồng nhất với Design System của CyberSoft. Thông báo lỗi phải hiển thị rõ ràng, dễ hiểu cho người dùng.

### 2.2. Bảo mật và Phân quyền (Security & Authorization)
* **Kiểm soát truy cập (Access Control):** Chỉ người dùng có Token hợp lệ mới được truy cập các API liên quan đến thông tin cá nhân.
* **Tính riêng tư (Data Privacy):** Không được phép xem hoặc chỉnh sửa dữ liệu của tài khoản khác thông qua việc thay đổi ID/Tài khoản trong request.
* **Phân quyền (Privilege):** Đảm bảo người dùng có Role "Học viên" không thể thực hiện các hành động hoặc nâng cấp quyền hạn của Role "Giảng viên" hoặc "Quản trị".

### 2.3. Ràng buộc dữ liệu (Data Validation)
* **Phòng chống tấn công cơ bản:** Hệ thống cần xử lý các ký tự đặc biệt để ngăn chặn các lỗi bảo mật cơ bản (như Script Injection qua các trường nhập liệu).
* **Định dạng dữ liệu:** Kiểm tra nghiêm ngặt định dạng Email, Số điện thoại và độ phức tạp của Mật khẩu ở cả phía Client và Server.

## 3. Môi trường thực hiện
* **Hệ thống:** CyberSoft Elearning Demo 2.
* **Công cụ:** Postman, Chrome DevTools, Jira.
