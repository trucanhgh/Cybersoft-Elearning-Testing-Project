# Test Cases – Cybersoft Capstone (Trúc Anh)

## Tổng quan

| Test Case ID | Title | Pre-Conditions | Test Steps | Test Data | Expected Results | Execution Status | Actual Results | Bug Priority | Notes |
|---|---|---|---|---|---|---|---|---|---|
| TC_01 | Xác minh hiển thị trang Thông tin cá nhân | - Đã đăng nhập thành công | 1. Truy cập trang: https://demo2.cybersoft.edu.vn<br>2. Click vào avatar người dùng ở góc trên bên phải |  | 2. - Trang Thông tin cá nhân hiển thị đúng với URL chuyển sang trang cá nhân.<br>- Hiển thị đầy đủ các thành phần: Navbar, Header, left sidebar, tab bar, nội dung thông tin và Footer | Pass |  |  |  |
| TC_02 | Xác minh hiển thị Navbar | - Đã đăng nhập thành công<br>- Đang ở trang Thông tin cá nhân | 1. Quan sát Navbar trên cùng |  | 1. Navbar hiển thị đúng với đầy đủ: Logo, Thanh tìm kiếm, Dánh mục, Khóa học, Blog, Sự kiện, Thông tin và ảnh đại diện người dùng ở góc phải | Pass |  |  |  |
| TC_03 | Xác minh hiển thị Header |  | 1. Quan sát Header màu vàng bên dưới navbar |  | 1. Hiển thị tiêu đề chính "THÔNG TIN CÁ NHÂN" và tiêu đề phụ "THÔNG TIN HỌC VIÊN" với chữ trắng trên nền vàng đúng theo thiết kế | Pass |  |  |  |
| TC_04 | Xác minh hiển thị left sidebar Giới thiệu người dùng |  | 1. Quan sát left sidebar Giới thiệu người dùng |  | 1. Left sidebar hiển thị đúng với:<br>- Ảnh đại diện người dùng<br>- Họ và tên người dùng<br>- Vị trí công việc<br>- Button [Hồ sơ cá nhân]<br>(Dữ liệu khớp với thông tin tài khoản đang đăng nhập) | Fail | 1. Họ và tên người dùng ở bên dưới ảnh đại diện là tên mặc định (Robert Nguyễn) thay vì Họ và tên thực tế | Low |  |
| TC_05 | Xác minh hiển thị [Thông tin cá nhân] |  | 1. Quan sát mục [Thông tin cá nhân] |  | 1. Mục [Thông tin cá nhân] hiển thị đúng với:<br>- Email<br>- Họ tên<br>- Số điện thoại<br>- Tài khoản<br>- Nhóm<br>- Đối tượng<br>(Dữ liệu khớp với thông tin tài khoản đang đăng nhập) | Pass |  |  |  |
| TC_06 | Xác minh hiển thị [KỸ NĂNG CỦA TÔI] |  | 1. Quan sát mục [KỸ NĂNG CỦA TÔI] |  | 1. Mục [KỸ NĂNG CỦA TÔI] hiển thị đúng với:<br>- Danh sách các kỹ năng phù hợp với vị trí và progress bar hiện đúng tiến độ | Pass |  |  |  |
| TC_07 | Xác minh hiển thị Footer |  | 1. Quan sát phần Footer |  | 1. Footer hiển thị đầy đủ các thành phần: logo, thông tin liên hệ, các đường dẫn và thông tin bản quyền theo đúng thiết kế | Pass |  |  |  |
| TC_08 | Xác minh hiển thị left sidebar Giới thiệu người dùng responsive trên Mobile (Width < 768px) | - Đã đăng nhập thành công<br>- Đang ở trang Thông tin cá nhân | 1. Chọn màn hình có Width < 768px | Màn hình: Width = 375px (iPhone SE) | 1. Left sidebar Giới thiệu người dùng ẩn hoặc thu gọn, không tràn ra ngoài viewport. Nội dung hiển thị gọn gàng, không bị che khuất | Pass |  |  |  |
| TC_09 | Xác minh hiển thị left sidebar Giới thiệu người dùng responsive trên Tablet (768px <= Width < 1024px) |  | 1. Chọn màn hình có 768px <= Width < 1024px | Màn hình: Width = 768px (iPad Mini) | 1. Left sidebar Giới thiệu người dùng hiển thị hoặc thu gọn phù hợp với kích thước tablet. Không bị tràn nội dung, layout cân đối | Pass |  |  |  |
| TC_10 | Xác minh hiển thị [Thông tin cá nhân] responsive trên Mobile (Width < 768px) |  | 1. Chọn màn hình có Width < 768px | Màn hình: Width = 375px (iPhone SE) | 1. Mục [Thông tin cá nhân] hiển thị đúng ở mobile: nội dung không bị cắt, các trường xếp theo chiều dọc, không có scroll ngang | Pass |  |  |  |
| TC_11 | Xác minh hiển thị [Thông tin cá nhân] responsive trên Tablet (768px <= Width < 1024px) |  | 1. Chọn màn hình có 768px <= Width < 1024px | Màn hình: Width = 768px (iPad Mini) | 1. Mục [Thông tin cá nhân] hiển thị đúng ở tablet: layout phù hợp, nội dung hiển thị đầy đủ không bị cắt | Pass |  |  |  |
| TC_12 | Xác minh hiển thị [Kỹ năng của tôi] responsive trên Mobile (Width < 768px) |  | 1. Chọn màn hình có Width < 768px | Màn hình: Width = 375px (iPhone SE) | 1. Mục [Kỹ năng của tôi] hiển thị đúng ở mobile: nội dung không bị cắt, không có scroll ngang | Pass |  |  |  |
| TC_13 | Xác minh hiển thị [Kỹ năng của tôi] responsive trên Tablet (768px <= Width < 1024px) |  | 1. Chọn màn hình có 768px <= Width < 1024px | Màn hình: Width = 768px (iPad Mini) | 1. Mục [Kỹ năng của tôi] hiển thị đúng ở tablet: layout phù hợp, nội dung hiển thị đầy đủ | Pass |  |  |  |

## Tab bar/ [Khóa học]

| Test Case ID | Title | Pre-Conditions | Test Steps | Test Data | Expected Results | Execution Status | Actual Results | Bug Priority | Notes |
|---|---|---|---|---|---|---|---|---|---|
| TC_14 | Xác minh hiển thị tab bar [Thông tin cá nhân]/[Khóa học] | - Đã đăng nhập thành công<br>- Đang ở trang Thông tin cá nhân | 1. Quan sát phần tab bar |  | 1. Tab bar hiển thị đúng 2 tab:<br>- Tab [Thông tin cá nhân]: đang active (được highlight)<br>- Tab [Khóa học]: không active<br>- Hover: con trỏ bàn tay | Pass |  |  |  |
| TC_15 | Xác minh khi chuyển tab [Thông tin cá nhân]/[Khóa học] |  | 1. Click vào [Khóa học] trên tab bar |  | 1. Trang chuyển sang hiển thị nội dung tab [Khóa học]<br>- Tab [Khóa học] được highlight là active<br>- Tab [Thông tin cá nhân] không còn active | Pass |  |  |  |
| TC_16 | Xác minh hiển thị tab [Khóa học] | - Đã đăng nhập thành công<br>- Đang ở tab [Khóa học] của trang Thông tin cá nhân | 1. Quan sát tab [Khóa học] |  | 1. Tab [Khóa học] hiển thị:<br>- Ô [Tìm kiếm] khóa học<br>- Danh sách khóa học đã đăng ký (hoặc thông báo trống nếu chưa đăng ký) | Pass |  |  |  |
| TC_17 | Xác minh hiển thị Danh sách khóa học | - Đã đăng nhập thành công<br>- Đang ở tab [Khóa học] của trang Thông tin cá nhân<br>- Đã đăng ký khóa học | 1. Quan sát Danh sách khóa học |  | 1. Danh sách khóa học hiển thị đúng:<br>- Các khóa học đã đăng ký được liệt kê<br>- Mỗi khóa học hiển thị đầy đủ thông tin | Pass |  |  |  |
| TC_18 | Xác minh hiển thị Khóa học |  | 1. Quan sát từng Khóa học trong danh sách |  | 1. Mỗi khóa học trong danh sách hiển thị đầy đủ:<br>- Ảnh khóa học<br>- Tên khóa học<br>- Tên giảng viên<br>- Button [HỦY KHÓA HỌC] | Pass |  |  |  |
| TC_19 | Xác minh hiển thị tab [Khóa học] Responsive trên Mobile (Width < 768px) | - Đã đăng nhập thành công<br>- Đang ở trang Thông tin cá nhân | 1. Chuyển sang tab [Khóa học]<br>2. Chọn màn hình có Width < 768px | Màn hình: Width = 375px (iPhone SE) | 1. Tab [Khóa học] và nội dung bên trong hiển thị đúng trên mobile: không tràn, danh sách khóa học xếp gọn theo chiều dọc | Pass |  |  |  |
| TC_20 | Xác minh hiển thị tab [Khóa học] Responsive trên Tablet (768px <= Width < 1024px) |  | 1. Chuyển sang tab [Khóa học]<br>2. Chọn màn hình có 768px <= Width < 1024px | Màn hình: Width = 768px (iPad Mini) | 1. Tab [Khóa học] và nội dung bên trong hiển thị đúng trên tablet: layout cân đối, không bị cắt nội dung | Pass |  |  |  |
| TC_21 | Xác minh khi chọn [Hủy khóa học] | - Đã đăng nhập thành công<br>- Đang ở tab [Khóa học] của trang Thông tin cá nhân<br>- Đã ghi danh vào khóa học: .100 | 1. Click vào avatar người dùng ở góc trên bên phải<br>2. Click vào [Khóa học] trên tab bar<br>3. Click button [HỦY KHÓA HỌC] của khóa học: ".100" | Tài khoản: trucanh<br>Khóa học: .100 | 3. - Hệ thống hiển thị popup xác nhận hủy khóa học ".100".<br>- Sau khi xác nhận: khóa học ".100" bị xóa khỏi danh sách, hệ thống thông báo hủy thành công | Fail | 3. Hệ thống hủy khóa học ngay sau khi click button [HỦY KHÓA HỌC] mà không có popup xác nhận | Medium |  |
| TC_22 | Xác minh khi nhấn Enter trên [Tìm kiếm] | - Đã đăng nhập thành công<br>- Đang ở tab [Khóa học] của trang Thông tin cá nhân<br>- Đã ghi danh vào khóa học: Javascript nâng cao mới | 1. Gõ vào ô [Tìm kiếm]: "Javascript nâng cao mới"<br>2. Nhấn Enter |  | 2. Hệ thống không thực hiện tìm kiếm khi nhấn Enter (hoặc không có sự kiện tìm kiếm được bind cho phím Enter). Giao diện giữ nguyên | Fail | 3. Khi nhấn Enter trân thanh tìm kiếm, người dùng bị đẩy về tab [Thông tin cá nhân] | Low |  |
| TC_23 | Xác minh khi nhập tên khóa học chính xác vào [Tìm kiếm] |  | 1. Gõ vào ô [Tìm kiếm]: "Javascript nâng cao mới" |  | 1. Danh sách lọc và hiển thị đúng khóa học có tên "Javascript nâng cao mới" | Pass |  |  |  |
| TC_24 | Xác minh khi nhập khoảng trắng vào trước và sau từ khóa [Tìm kiếm] |  | 1. Gõ vào ô [Tìm kiếm]: "  Javascript nâng cao mới   " |  | 1. Hệ thống tự động trim khoảng trắng, hiển thị đúng kết quả khóa học "Javascript nâng cao mới" | Pass |  |  |  |
| TC_25 | Xác minh khi nhập vào [Tìm kiếm] theo từ khóa khớp một phần |  | 1. Gõ vào ô [Tìm kiếm]: "Jav" |  | 1. Danh sách hiển thị tất cả khóa học có tên chứa "Jav", bao gồm "Javascript nâng cao mới" | Pass |  |  |  |
| TC_26 | Xác minh tìm kiếm không phân biệt hoa/thường |  | 1. Gõ vào ô [Tìm kiếm]: "javascript" |  | 1. Tìm kiếm không phân biệt hoa/thường: kết quả vẫn hiển thị "Javascript nâng cao mới" | Pass |  |  |  |
| TC_27 | Xác minh tìm kiếm bằng tiếng Việt có dấu |  | 1. Gõ vào ô [Tìm kiếm]: "Javascript nâng cao mới" |  | 1. Kết quả hiển thị đúng khóa học "Javascript nâng cao mới", hệ thống hỗ trợ tìm kiếm tiếng Việt có dấu | Pass |  |  |  |
| TC_28 | Xác minh khi xóa từ khóa tìm kiếm |  | 1. Gõ vào ô [Tìm kiếm]: "Javascript nâng cao mới"<br>2. Xóa từng chữ cái |  | 2. - Khi xóa dần từng ký tự, danh sách kết quả cập nhật realtime theo từ khóa còn lại.<br>- Khi xóa hết, hiển thị toàn bộ danh sách khóa học | Pass |  |  |  |

## [Chỉnh sửa thông tin cá nhân]

| Test Case ID | Title | Pre-Conditions | Test Steps | Test Data | Expected Results | Execution Status | Actual Results | Bug Priority | Notes |
|---|---|---|---|---|---|---|---|---|---|
| TC_29 | Xác minh hiển thị popup [Chỉnh sửa thông tin cá nhân] | - Đã đăng nhập thành công<br>- Đang ở trang Thông tin cá nhân | 1. Click button [CẬP NHẬT] |  | 1. Popup [Chỉnh sửa thông tin cá nhân] hiển thị với:<br>- Tiêu đề "Chỉnh sửa thông tin cá nhân"<br>- Các trường nhập liệu: Họ và tên, Mật khẩu, Email, Số điện thoại<br>- Button [Hoàn thành], [Đóng] và nút [X] | Pass |  |  |  |
| TC_30 | Xác minh hiển thị các trường nhập liệu | - Đã đăng nhập thành công<br>- Đang ở trang Thông tin cá nhân<br>- Đã mở popup [Chỉnh sửa thông tin cá nhân] | 1. Quan sát các trường nhập liệu |  | 1. Hiển thị đầy đủ các trường:<br>- [Họ và tên]: textbox, có placeholder, hiển thị dữ liệu hiện tại<br>- [Mật khẩu]: input type password<br>- [Email]: textbox, hiển thị email hiện tại<br>- [Số điện thoại]: textbox, hiển thị số điện thoại hiện tại | Pass |  |  |  |
| TC_31 | Xác minh hiển thị các button hành động |  | 1. Quan sát các button: [Hoàn thành], [Đóng] |  | 1. Hiển thị đúng 2 button:<br>- Button [Hoàn thành]: màu nổi bật, có thể click<br>- Button [Đóng]: có thể click<br>Cả 2 button hiển thị đúng text theo thiết kế | Pass |  |  |  |
| TC_32 | Xác minh hiển thị nút đóng [X] |  | 1. Quan sát button [X] ở góc trên bên phải |  | 1. Nút [X] hiển thị ở góc trên bên phải của popup, có thể nhận click | Pass |  |  |  |
| TC_33 | Xác minh hiển thị popup [Chỉnh sửa thông tin cá nhân] đóng khi click nút [X] |  | 1. Điền thông tin vào các trường<br>2. Click nút [X] ở góc trên bên phải của popup |  | 2. - Popup đóng lại<br>- Dữ liệu chưa lưu không được cập nhật<br>- Thông tin cá nhân vẫn giữ nguyên như trước khi mở popup | Pass |  |  |  |
| TC_34 | Xác minh khi chỉnh sửa thông tin cá nhân với dữ liệu hợp lệ |  | 1. Điền các field với dữ liệu hợp lệ: <thongtin><br>2. Click button [Hoàn thành] |  | 2. - Thông tin cá nhân được cập nhật thành công.<br>- Hệ thống hiển thị thông báo thành công.<br>- Dữ liệu mới hiển thị đúng trên trang Thông tin cá nhân ngay lập tức mà không cần tải lại trang | Pass |  |  |  |
| TC_35 | Xác minh khi để trống [Họ và tên] |  | 1. Để trống textbox [Họ và tên]<br>2. Click ra ngoài textbox |  | 2. - Hiển thị thông báo lỗi: "Tên không được để trống". | Pass |  |  |  |
| TC_36 | Xác minh khi nhập ký tự đặc biệt vào [Họ và tên] | - Đã đăng nhập thành công<br>- Đang ở trang Thông tin cá nhân<br>- Đã mở popup [Chỉnh sửa thông tin cá nhân] | 1. Nhập vào textbox [Họ và Tên]: "#"<br>2. Click ra ngoài textbox |  | 2. Hiển thị thông báo lỗi: "Chỉ nhập kí tự chữ". | Pass |  |  |  |
| TC_37 | Xác minh khi nhập ký tự số vào [Họ và tên] |  | 1. Nhập vào textbox [Họ và Tên]: "1"<br>2. Click ra ngoài textbox |  | 2. Hiển thị thông báo lỗi: "Chỉ nhập kí tự chữ". | Pass |  |  |  |
| TC_38 | Xác minh khi nhập khoảng cách ở đầu vào [Họ và tên] |  | 1. Nhập vào textbox [Họ và Tên]: " Trúc Anh"<br>2. Nhập các thông tin còn lại hợp lệ: <thongtin><br>3. Click button [Hoàn thành] |  | 3. - Hệ thống tự động trim khoảng trắng đầu<br>- Lưu thành công với giá trị không có khoảng trắng đầu | Pass |  |  |  |
| TC_39 | Xác minh khi chỉ nhập chuỗi dấu cách vào [Họ và tên] |  | 1. Nhập vào textbox [Họ và Tên]: "           "<br>2. Nhập các thông tin còn lại hợp lệ: <thongtin><br>3. Click button [Hoàn thành] |  | 3. Hệ thống coi chuỗi dấu cách là trống, hiển thị thông báo lỗi: "Tên không được để trống" | Fail | 3. Hệ thống không báo lỗi và lưu tên người dùng là khoảng trắng sau khi submit | Medium |  |
| TC_40 | Xác minh khi để trống [Mật khẩu] |  | 1. Để trống textbox [Mật khẩu]<br>2. Click ra ngoài textbox |  | 2. Hiển thị thông báo lỗi: "Mật khẩu không được để trống" | Fail | 2. Hiển thị sai thông báo lỗi: "Tài khoản không được để trống"<br>(Thông báo đúng: "Mật khẩu không được để trống") | Low |  |
| TC_41 | Xác minh khi nhập 7 ký tự vào [Mật khẩu] |  | 1.  Nhập vào textbox [Mật khẩu]: Abc123@<br>2. Click ra ngoài textbox |  | 2. Hiển thị thông báo lỗi: "Mật khẩu phải ít nhất 8 tự gồm chữ hoa, chữ thường, số, và kí tự đặc biệt" | Fail | 2. Hệ thống yêu cầu mật khẩu phải có cả chữ hoa và chữ thường, nhưng câu thông báo lỗi hiện tại chỉ yêu cầu chung chung là "chữ" | Low |  |
| TC_42 | Xác minh khi nhập 8 ký tự vào [Mật khẩu] |  | 1.  Nhập vào textbox [Mật khẩu]: Abcd123@<br>2. Click ra ngoài textbox |  | 2. Hệ thống không hiện thông báo lỗi | Pass |  |  |  |
| TC_43 | Xác minh khi nhập 9 ký tự vào [Mật khẩu] |  | 1.  Nhập vào textbox [Mật khẩu]: Abcd1234@<br>2. Click ra ngoài textbox |  | 2. Hệ thống không hiện thông báo lỗi | Pass |  |  |  |
| TC_44 | Xác minh [Mật khẩu] phải gồm chữ |  | 1. Nhập vào textbox [Mật khẩu]: "12345678@"<br>2. Click ra ngoài textbox |  | 2. Hiển thị thông báo lỗi: "Mật khẩu phải ít nhất 8 tự gồm chữ hoa, chữ thường, số, và kí tự đặc biệt" | Fail | 2. Hệ thống yêu cầu mật khẩu phải có cả chữ hoa và chữ thường, nhưng thông báo lỗi hiện tại chỉ yêu cầu chung chung là "chữ" | Low |  |
| TC_45 | Xác minh [Mật khẩu] phải gồm số |  | 1. Nhập vào textbox [Mật khẩu]: "Abcdefgh@"<br>2. Click ra ngoài textbox |  |  | Fail |  | Low |  |
| TC_46 | Xác minh [Mật khẩu] phải gồm ký tự đặc biệt |  | 1. Nhập vào textbox [Mật khẩu]: "Abcd1234"<br>2. Click ra ngoài textbox |  |  | Fail |  | Low |  |
| TC_47 | Xác minh [Mật khẩu] phải gồm chữ in hoa | - Đã đăng nhập thành công<br>- Đang ở trang Thông tin cá nhân<br>- Đã mở popup [Chỉnh sửa thông tin cá nhân] | 1. Nhập vào textbox [Mật khẩu]: "abcd1234@"<br>2. Click ra ngoài textbox |  |  | Fail |  | Low |  |
| TC_48 | Xác minh [Mật khẩu] phải gồm chữ thường |  | 1. Nhập vào textbox [Mật khẩu]: "ABCD1234@"<br>2. Click ra ngoài textbox |  |  | Fail |  | Low |  |
| TC_49 | Xác minh khi để trống [Emai] |  | 1. Để trống textbox [Email]<br>2. Click ra ngoài textbox |  | 2. Hiển thị thông báo lỗi: "Email không được để trống" | Pass |  |  |  |
| TC_50 | Xác minh [Email] phải gồm "@" |  | 1. Nhập vào textbox [Email]: "abcgmail.com"<br>2. Click ra ngoài textbox |  | 2. Hiển thị thông báo lỗi: "Email không hợp lệ" | Pass |  |  |  |
| TC_51 | Xác minh [Email] phải gồm "." |  | 1. Nhập vào textbox [Email]: "abc@gmailcom"<br>2. Click ra ngoài textbox |  | 2. Hiển thị thông báo lỗi: "Email không hợp lệ" | Pass |  |  |  |
| TC_52 | Xác minh khi nhập khoảng trắng vào [Email] |  | 1. Nhập vào textbox [Email]: "ab c@gmail.com"<br>2. Click ra ngoài textbox |  | 2. Hiển thị thông báo lỗi: "Email không hợp lệ" | Pass |  |  |  |
| TC_53 | Xác minh khi nhập ký tự đặc biệt vào [Email] |  | 1. Nhập vào textbox [Email]: "abc#@gmail.com"<br>2. Click ra ngoài textbox |  | 2. Hiển thị thông báo lỗi: "Email không hợp lệ" | Pass |  |  |  |
| TC_54 | Xác minh khi nhập Email liên kết với tài khoản khác |  | 1. Nhập vào textbox [Email]: email đã liên kết tài khoản khác<br>2. Điền các thông tin còn lại hợp lệ<br>3. Click button [Hoàn thành] |  | 3. Hệ thống hiển thị thông báo lỗi: "Email đã tồn tại". Không lưu thông tin | Pass |  |  |  |
| TC_55 | Xác minh khi để trống [Số điện thoại] |  | 1. Để trống textbox [Số điện thoại]<br>2. Click ra ngoài textbox |  | 2. Hiển thị thông báo lỗi: "Số điện thoại không được để trống" | Pass |  |  |  |
| TC_56 | Xác minh số [Số điện thoại] phải bắt đầu bằng "0" |  | 1. Nhập vào textbox [Số điện thoại]: "11234567890"<br>2. Click ra ngoài textbox |  | 2. Hiển thị thông báo lỗi: "Số điện thoại chưa đúng định đạng" | Pass |  |  |  |
| TC_57 | Xác minh khi nhập 9 chữ số vào [Số điện thoại] |  | 1. Nhập vào textbox [Số điện thoại]: "012345678901"<br>2. Click ra ngoài textbox |  | 2. Hiển thị thông báo lỗi: "Số điện thoại chưa đúng định đạng" | Pass |  |  |  |
| TC_58 | Xác minh khi nhập 10 chữ số vào [Số điện thoại] |  | 1. Nhập vào textbox [Số điện thoại]: "0123456789"<br>2. Click ra ngoài textbox |  | 2. Hệ thống chấp nhận 10 chữ số bắt đầu bằng "0". Không hiển thị lỗi | Fail | 2. Hệ thống không chấp nhận input hợp lệ gồm số điện thoại bắt đầu bằng "0" và gồm 10 chữ số, vẫn báo lỗi: "Số điện thoại chưa đúng định đạng" | Medium |  |
| TC_59 | Xác minh khi nhập 11 chữ số vào [Số điện thoại] |  | 1. Nhập vào textbox [Số điện thoại]: "01234567890"<br>2. Click ra ngoài textbox |  | 2. Hệ thống chấp nhận 11 chữ số bắt đầu bằng "0". Không hiển thị lỗi | Pass |  |  |  |
| TC_60 | Xác minh khi nhập 12 chữ số vào [Số điện thoại] |  | 1. Nhập vào textbox [Số điện thoại]: "012345678901"<br>2. Click ra ngoài textbox |  | 2. Hiển thị thông báo lỗi: "Số điện thoại chưa đúng định đạng" | Pass |  |  |  |

## API TC

## 1. API GET – Lấy thông tin tài khoản (ThongTinTaiKhoan)

**CURL_01**

```bash
curl --location 'https://elearningnew.cybersoft.edu.vn/api/QuanLyNguoiDung/ThongTinTaiKhoan' \
--header 'tokencybersoft: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0ZW5Mb3AiOiJUZXN0aW5nIDE0IiwiSGV0SGFuU3RyaW5nIjoiMTUvMTAvMjAyNiIsIkhldEhhblRpbWUiOiIxNzkyMDIyNDAwMDAwIiwibmJmIjoxNzY3ODkxNjAwLCJleHAiOjE3OTIxNzAwMDB9.DLVjgmwvBK8rzcWWgQA7dYOQuJZ55Vm5MThmUNcx8As' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoidHJ1Y2FuaCIsImh0dHA6Ly9zY2hlbWFzLm1pY3Jvc29mdC5jb20vd3MvMjAwOC8wNi9pZGVudGl0eS9jbGFpbXMvcm9sZSI6IkhWIiwibmJmIjoxNzc0MTc1OTg5LCJleHAiOjE3NzQxNzk1ODl9.r9-s8yrTz1Q29mVKuFsoWQ_1oIvsnuU7wx5-htI74yc' \
--data '{
    "taiKhoan": "trucanh"
}'
```

| Test Case ID | Title | Pre-Conditions | Test Steps | Test Data | Expected Results | Execution Status | Actual Results | Bug Priority | Notes |
|---|---|---|---|---|---|---|---|---|---|
| TC_60 | Xác minh lấy thông tin tài khoản thành công |  | 1. Dùng CURL_01<br>2. Đổi tokencybersoft hợp lệ<br>3. Đổi Authorization: Bear token hợp lệ<br>4. Thực hiện gọi API |  | 4. - API trả về HTTP 200<br>- Response body chứa thông tin tài khoản: taiKhoan, hoTen, email, soDT, maLoaiNguoiDung |  |  |  |  |
| TC_61 | Xác minh lấy danh sách khóa học thành công |  |  |  | 4. - API trả về HTTP 200<br>- Response body chứa danh sách khóa học đã đăng ký của tài khoản "trucanh" |  |  |  |  |
| TC_62 | Xác minh API ThongTinTaiKhoan khi không có Authorization token |  | 1. Dùng CURL_01<br>2. Đổi tokencybersoft hợp lệ<br>3. Xóa header "Authorization"<br>4. Thực hiện gọi API |  | 4. - API trả về HTTP 401 (Unauthorized)<br>- Response body chứa thông báo lỗi xác thực |  |  |  |  |

## 2. API PUT – Cập nhật thông tin người dùng (CapNhatThongTinNguoiDung)

**CURL_02**

```bash
curl --location --request PUT 'https://elearningnew.cybersoft.edu.vn/api/QuanLyNguoiDung/CapNhatThongTinNguoiDung' \
--header 'tokencybersoft: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0ZW5Mb3AiOiJUZXN0aW5nIDE0IiwiSGV0SGFuU3RyaW5nIjoiMTUvMTAvMjAyNiIsIkhldEhhblRpbWUiOiIxNzkyMDIyNDAwMDAwIiwibmJmIjoxNzY3ODkxNjAwLCJleHAiOjE3OTIxNzAwMDB9.DLVjgmwvBK8rzcWWgQA7dYOQuJZ55Vm5MThmUNcx8As' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoidHJ1Y2FuaCIsImh0dHA6Ly9zY2hlbWFzLm1pY3Jvc29mdC5jb20vd3MvMjAwOC8wNi9pZGVudGl0eS9jbGFpbXMvcm9sZSI6IkhWIiwibmJmIjoxNzc0MTc1OTg5LCJleHAiOjE3NzQxNzk1ODl9.r9-s8yrTz1Q29mVKuFsoWQ_1oIvsnuU7wx5-htI74yc' \
--data-raw '{
    "taiKhoan": "trucanh",
    "matKhau": "Abcd1234@",
    "hoTen": "a",
    "email": "abc@g.c",
    "soDT": "01234567890",
    "maLoaiNguoiDung": "HV",
    "maNhom": "GP01"
}'
```

| Test Case ID | Title | Pre-Conditions | Test Steps | Test Data | Expected Results | Execution Status | Actual Results | Bug Priority | Notes |
|---|---|---|---|---|---|---|---|---|---|
| TC_63 | Xác minh khi chỉnh sửa thông tin cá nhân với dữ liệu hợp lệ |  | 1. Dùng CURL_02<br>2. Thực hiện gọi API |  | 2. - API trả về HTTP 200<br>- Response thông báo cập nhật thành công<br>- Gọi lại API ThongTinTaiKhoan để xác nhận dữ liệu đã được lưu đúng | Pass |  |  |  |
| TC_64 | Xác minh khi để trống họ tên |  | 1. Dùng CURL_02<br>2. Sửa request body "hoTen"<br>3. Thực hiện gọi API | "hoTen": "" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi yêu cầu nhập họ tên | Fail | 3. API trả về 200 và lưu dữ liệu hoTen không hợp lệ | Medium |  |
| TC_65 | Xác minh khi nhập ký tự đặc biệt vào họ tên |  |  | "hoTen": "#" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: họ tên không được chứa ký tự đặc biệt | Fail |  | Medium |  |
| TC_66 | Xác minh khi nhập ký tự số vào họ tên |  |  | "hoTen": "2" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: họ tên không được chứa số | Fail |  | Medium |  |
| TC_67 | Xác minh khi nhập khoảng cách ở đầu vào họ tên |  |  | "hoTen": " a" (có khoảng trắng đầu) | 3. - API trả về HTTP 400 hoặc tự động trim khoảng trắng<br>- Nếu trim: dữ liệu lưu là "a" (không có khoảng trắng đầu)<br>- Nếu không trim: trả về lỗi validation | Fail |  | Medium |  |
| TC_68 | Xác minh khi chỉ nhập chuỗi khoảng cách vào họ tên |  |  | "hoTen": "   " | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: họ tên không được là chuỗi khoảng trắng | Fail |  | Medium |  |
| TC_69 | Xác minh khi để trống mật khẩu |  | 1. Dùng CURL_02<br>2. Sửa request body "matKhau"<br>3. Thực hiện gọi API | "matKhau": "" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi yêu cầu nhập mật khẩu | Fail | 3.  - API trả về HTTP 200<br>- matKhau không được cập nhật | Medium |  |
| TC_70 | Xác minh khi nhập mật khẩu < 8 ký tự |  |  | "matKhau": "Abc123@" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: mật khẩu phải có ít nhất 8 ký tự | Fail | 3. API trả về 200 và lưu dữ liệu matKhau không hợp lệ | Medium |  |
| TC_71 | Xác minh mật khẩu phải gồm chữ |  |  | "matKhau": "12345678@" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: mật khẩu phải chứa chữ cái | Fail |  | Medium |  |
| TC_72 | Xác minh mật khẩu phải gồm số |  |  | "matKhau": "Abcdefgh@" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: mật khẩu phải chứa chữ số | Fail |  | Medium |  |
| TC_73 | Xác minh mật khẩu phải gồm ký tự đặc biệt |  |  | "matKhau": "1234Abcd" | 3. API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: mật khẩu phải chứa ký tự đặc biệt | Fail |  | Medium |  |
| TC_74 | Xác minh mật khẩu phải gồm chữ in hoa |  |  | "matKhau": "1234abcd@" | 3. API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: mật khẩu phải chứa chữ in hoa | Fail |  | Medium |  |
| TC_75 | Xác minh mật khẩu phải gồm chữ thường |  |  | "matKhau": "ABCD1234@" | 3. API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: mật khẩu phải chứa chữ thường | Fail |  | Medium |  |
| TC_76 | Xác minh khi để trống email |  | 1. Dùng CURL_02<br>2. Sửa request body "email"<br>3. Thực hiện gọi API | "email": "" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi yêu cầu nhập email | Fail | 3. API trả về 200 và lưu dữ liệu email không hợp lệ | Medium |  |
| TC_77 | Xác minh email phải gồm "@" |  |  | "email": "abcgmail.com" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: email không hợp lệ (thiếu "@") | Fail |  | Medium |  |
| TC_78 | Xác minh email phải gồm "." |  |  | "email": "abc@gmailcom" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: email không hợp lệ (thiếu ".") | Fail |  | Medium |  |
| TC_79 | Xác minh khi nhập khoảng trắng vào trường email |  |  | "email": "ab c@gmail.com" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: email không được chứa khoảng trắng | Fail |  | Medium |  |
| TC_80 | Xác minh khi nhập ký tự đặc biệt vào trường email |  |  | "email": "abc#@gmail.com" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: email không hợp lệ | Fail |  | Medium |  |
| TC_81 | Xác minh khi cập nhật tài khoản bằng email đã liên kết với tài khoản khác | - Đã có tài khoản khác liên kết với email: abc@gmail.com |  | "email" : "abc@gmail.com" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: "Email đã tồn tại!" | Pass |  |  |  |
| TC_82 | Xác minh khi để trống số điện thoại |  | 1. Dùng CURL_02<br>2. Sửa request body "soDT"<br>3. Thực hiện gọi API | "soDT": "" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi yêu cầu nhập số điện thoại | Fail | 3. API trả về 200 và lưu dữ liệu soDT không hợp lệ | Medium |  |
| TC_83 | Xác minh số điện thoại phải bắt đầu bằng "0" |  |  | "soDT": "11234567890" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: số điện thoại phải bắt đầu bằng "0" | Fail |  | Medium |  |
| TC_84 | Xác minh khi nhập < 11 chữ số vào trường số điện thoại |  |  | "soDT": "0123456789" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: số điện thoại không hợp lệ (cần đủ 10 hoặc 11 chữ số) | Fail |  | Medium |  |
| TC_85 | Xác minh khi nhập > 11 chữ số vào trường số điện thoại |  |  | "soDT": "012345678901" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: số điện thoại không hợp lệ (vượt quá 11 chữ số) | Fail |  | Medium |  |
| TC_86 | Xác minh API CapNhatThongTin khi không có Authorization token |  | 1. Dùng CURL_02<br>2. Xóa header "Authorization"<br>3. Thực hiện gọi API | Authorization: (bỏ trống header Authorization) | 3. - API trả về HTTP 401 (Unauthorized)<br>- Không cập nhật bất kỳ dữ liệu nào | Pass |  |  |  |
| TC_87 | Xác minh API CapNhatThongTin khi token hết hạn | - Có token đã hết hạn | 1. Dùng CURL_02<br>2. Thay Authorization bằng token hết hạn<br>3. Thực hiện gọi API | Authorization: Bearer <expired_token> | 3. - API trả về HTTP 401 (Unauthorized)<br>- Response body chứa thông báo token hết hạn | Pass |  |  |  |
| TC_88 | Xác minh API CapNhatThongTin khi cập nhật thông tin của tài khoản khác | - Đã tồn tại taiKhoan: "otheraccount" | 1. Dùng CURL_02<br>2. Sửa request body "taiKhoan" thành tài khoản khác<br>3. Thực hiện gọi API | "taiKhoan": "otheraccount" | 3. - API trả về HTTP 403 (Forbidden)<br>- Hệ thống từ chối cập nhật thông tin tài khoản khác<br>- Dữ liệu của "otheraccount" không bị thay đổi | Fail | 3. API trả về 200 và cập nhật dữ liệu của tài khoản khác thành công | High |  |
| TC_89 | Xác minh khi học viên tự thay đổi mã loại người dùng của bản thân | - Tài khoản có maLoaiNguoiDung là : HV | 1. Dùng CURL_02<br>2. Sửa request body "maLoaiNguoiDung" thành GV<br>3. Thực hiện gọi API | "maLoaiNguoiDung": "GV" | 3. - API trả về HTTP 403 (Forbidden)<br>- Hệ thống từ chối cập nhật thông tin tài khoản khác<br>- Response body chứa thông báo lỗi | Fail | 3. API trả về 200 và tài khoản HV đổi thành GV thành công | High |  |
| TC_90 | Xác minh khi nhập maLoaiNguoiDung không hợp lệ |  | 1. Dùng CURL_02<br>2. Sửa request body "maLoaiNguoiDung" thành mã không hợp lệ<br>3. Thực hiện gọi API | "maLoaiNguoiDung": "a" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: Loại người dùng không hợp lệ! | Pass |  |  |  |
| TC_91 | Xác minh khi nhập maNhom không hợp lệ |  | 1. Dùng CURL_02<br>2. Sửa request body "maNhom" thành mã không hợp lệ<br>3. Thực hiện gọi API | "maNhom": "a" | 3. - API trả về HTTP 400 (Bad Request)<br>- Response body chứa thông báo lỗi: Nhóm người dùng không hợp lệ! | Pass |  |  |  |

## 3. API DELETE – Hủy ghi danh khóa học (HuyGhiDanh)

**CURL_03**

```bash
curl --location 'https://elearningnew.cybersoft.edu.vn/api/QuanLyKhoaHoc/HuyGhiDanh' \
--header 'tokencybersoft: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0ZW5Mb3AiOiJUZXN0aW5nIDE0IiwiSGV0SGFuU3RyaW5nIjoiMTUvMTAvMjAyNiIsIkhldEhhblRpbWUiOiIxNzkyMDIyNDAwMDAwIiwibmJmIjoxNzY3ODkxNjAwLCJleHAiOjE3OTIxNzAwMDB9.DLVjgmwvBK8rzcWWgQA7dYOQuJZ55Vm5MThmUNcx8As' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJodHRwOi8vc2NoZW1hcy54bWxzb2FwLm9yZy93cy8yMDA1LzA1L2lkZW50aXR5L2NsYWltcy9uYW1lIjoidHJ1Y2FuaCIsImh0dHA6Ly9zY2hlbWFzLm1pY3Jvc29mdC5jb20vd3MvMjAwOC8wNi9pZGVudGl0eS9jbGFpbXMvcm9sZSI6IkhWIiwibmJmIjoxNzc0MTc1OTg5LCJleHAiOjE3NzQxNzk1ODl9.r9-s8yrTz1Q29mVKuFsoWQ_1oIvsnuU7wx5-htI74yc' \
--data '{
    "taiKhoan": "trucanh",
    "maKhoaHoc": ".100"
}'
```

| Test Case ID | Title | Pre-Conditions | Test Steps | Test Data | Expected Results | Execution Status | Actual Results | Bug Priority | Notes |
|---|---|---|---|---|---|---|---|---|---|
| TC_92 | Xác minh khi hủy khóa học thành công | - Đã ghi danh vào khóa học ".100" | 1. Dùng CURL_03<br>2. Thực hiện gọi API |  | 2. - API trả về HTTP 200<br>-. Response thông báo hủy ghi danh thành công<br>- Gọi lại API ThongTinTaiKhoan xác nhận khóa học ".100" đã bị xóa khỏi danh sách | Pass |  |  |  |
| TC_93 | Xác minh khi hủy một khóa học chưa ghi danh | - Chưa ghi danh vào khóa học ".100" | 1. Dùng CURL_03<br>2. Thực hiện gọi API |  | 2. - API trả về HTTP 400 hoặc HTTP 404<br>- Response body chứa thông báo lỗi: tài khoản chưa ghi danh vào khóa học này | Pass |  |  |  |
| TC_94 | Xác minh API HuyGhiDanh khi không có Authorization token |  | 1. Dùng CURL_03<br>2. Xóa header "Authorization"<br>3. Thực hiện gọi API |  | 3. - API trả về HTTP 401 (Unauthorized)<br>- Không thực hiện hủy ghi danh | Pass |  |  |  |
| TC_95 | Xác minh API HuyGhiDanh với maKhoaHoc không tồn tại |  | 1. Dùng CURL_03<br>2. Sửa request body "maKhoaHoc" thành mã không tồn tại<br>3. Thực hiện gọi API | "maKhoaHoc": "INVALID_COURSE" | 3. - API trả về HTTP 404 (Not Found)<br>- Response body chứa thông báo: không tìm thấy khóa học | Pass |  |  |  |
