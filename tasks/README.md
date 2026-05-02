# 🚀 Money Tracker - Product Backlog

## 🎯 Tầm nhìn Sản phẩm (Product Vision)
Xây dựng một ứng dụng quản lý tài chính cá nhân thông minh, giúp người dùng kiểm soát dòng tiền, lập kế hoạch ngân sách và đạt được tự do tài chính thông qua việc theo dõi thu chi chi tiết và báo cáo phân tích trực quan.

---

## 🏗️ Danh sách Epic

1.  **IAM (Identity & Access Management)**: Quản lý danh tính và bảo mật tài khoản.
2.  **Wallet Core**: Hệ thống quản lý ví và tài sản đa tiền tệ.
3.  **Transaction Engine**: Xử lý các nghiệp vụ thu, chi và chuyển khoản.
4.  **Analytics & Intelligence**: Hệ thống báo cáo, thống kê và thông báo tự động.
5.  **Budgeting & Taxonomy**: Quản lý hạn mức chi tiêu và phân loại danh mục.
6.  **Advanced Search & UX**: Công cụ tìm kiếm, lọc và tùy biến trải nghiệm người dùng.
7.  **Collaboration (Social)**: Các tính năng tương tác và hỗ trợ (Chat/Video).

---

## 📋 Chi tiết Product Backlog

### 🔐 Epic 1: Quản lý Tài khoản (IAM)
*Bảo mật và cá nhân hóa thông tin người dùng.*

| ID | User Story | Priority | Trạng thái | Acceptance Criteria (AC) |
| :--- | :--- | :---: | :---: | :--- |
| **US01** | **Đăng ký tài khoản** | P0 | 📝 To Do | - Form: Username, Password (6-8 kí tự).<br>- Validation: Báo lỗi nếu trùng username hoặc sai định dạng.<br>- Flow: Đăng ký thành công chuyển hướng sang Login. |
| **US02** | **Đăng nhập hệ thống** | P0 | 📝 To Do | - Input: Username, Password.<br>- Flow: Đăng nhập thành công chuyển hướng về Dashboard (Trang chủ). |
| **US03** | **Đăng nhập Social** | P1 | 📝 To Do | - Hỗ trợ: Facebook, Google, Github.<br>- Flow: Lấy thông tin email/profile từ bên thứ 3 để tạo phiên đăng nhập. |
| **US04** | **Đăng xuất** | P0 | 📝 To Do | - Xóa session/token hiện tại.<br>- Flow: Chuyển hướng về trang Login. |
| **US05** | **Quên mật khẩu** | P1 | 📝 To Do | - Flow: Nhập email -> Hệ thống gửi mật khẩu mới (Random 8 ký tự, bao gồm chữ hoa, thường, số). |
| **US06** | **Kích hoạt tài khoản** | P1 | 📝 To Do | - Gửi email chứa link kích hoạt sau khi đăng ký.<br>- User chỉ được login sau khi đã click link kích hoạt. |
| **US07** | **Đổi mật khẩu** | P1 | 📝 To Do | - Xác thực mật khẩu cũ.<br>- Nhập mật khẩu mới và xác nhận mật khẩu mới. |
| **US08** | **Xóa tài khoản** | P2 | 📝 To Do | - Xóa sạch dữ liệu liên quan (Ví, Giao dịch, Danh mục) của User.<br>- Yêu cầu xác nhận (Confirmation Dialog) trước khi xóa. |
| **US09** | **Cập nhật Profile** | P2 | 📝 To Do | - Cập nhật được: Ảnh đại diện (Avatar), Số điện thoại. |

### 💳 Epic 2: Quản lý Ví (Wallet Core)
*Nền tảng quản lý nguồn tiền.*

| ID | User Story | Priority | Trạng thái | Acceptance Criteria (AC) |
| :--- | :--- | :---: | :---: | :--- |
| **US10** | **Thêm ví mới** | P0 | 📝 To Do | - Popup/Form: Icon, Tên ví, Số dư ban đầu, Tiền tệ (VND, USD...), Mô tả.<br>- Validation: Tên ví không được để trống. |
| **US11** | **Sửa thông tin ví** | P1 | 📝 To Do | - Cho phép sửa: Icon, Tên, Tiền tệ, Mô tả.<br>- Cập nhật UI ngay lập tức sau khi lưu. |
| **US12** | **Xóa ví** | P1 | 📝 To Do | - Xóa ví đồng thời xóa toàn bộ giao dịch thuộc ví đó.<br>- Cảnh báo người dùng về việc mất dữ liệu giao dịch. |
| **US13** | **Chia sẻ ví (Share)** | P2 | 📝 To Do | - Share qua email tài khoản khác.<br>- Gửi thông báo email cho người được share. |
| **US14** | **Quản lý quyền share** | P2 | 📝 To Do | - Quyền: `Viewer` (Chỉ xem), `Owner` (Toàn quyền). |
| **US15** | **Hủy share ví** | P2 | 📝 To Do | - Chủ ví có quyền xóa tài khoản đã được share khỏi danh sách truy cập. |
| **US16** | **Chọn ví mặc định** | P0 | 📝 To Do | - Chọn ví hiện tại trên Navbar để thực hiện các giao dịch nhanh. |
| **US17** | **Chuyển tiền giữa các ví** | P1 | 📝 To Do | - Form: Ví nguồn, Ví đích, Số tiền, Ghi chú.<br>- Logic: Số dư ví nguồn >= Số tiền chuyển. |
| **US18** | **Lưu trữ ví (Archive)** | P2 | 📝 To Do | - Chuyển trạng thái ví sang Read-only.<br>- Khóa các tính năng thêm/sửa/xóa trên ví này. |
| **US19** | **Xem danh sách ví** | P0 | 📝 To Do | - Hiển thị tại Dashboard: Icon, Tên, Tổng nạp, Số dư hiện tại. |
| **US20** | **Xem tổng tài sản** | P0 | 📝 To Do | - Tính tổng số dư của tất cả các ví (quy đổi về tiền tệ mặc định). |

### 💰 Epic 3: Giao dịch (Transaction Engine)
*Xử lý biến động số dư.*

| ID | User Story | Priority | Trạng thái | Acceptance Criteria (AC) |
| :--- | :--- | :---: | :---: | :--- |
| **US21** | **Nạp tiền (Income)** | P0 | 📝 To Do | - Form: Số tiền, Ghi chú, Ví nhận.<br>- Cộng số dư vào ví tương ứng. |
| **US22** | **Ghi chép khoản chi** | P0 | 📝 To Do | - Form: Số tiền, Danh mục, Ví chi, Ghi chú, Thời gian.<br>- Trừ số dư ví tương ứng. |
| **US23** | **Sửa giao dịch** | P1 | 📝 To Do | - Cho phép sửa mọi thông tin giao dịch.<br>- Tự động tính toán lại số dư ví nếu thay đổi số tiền. |
| **US24** | **Xóa giao dịch** | P1 | 📝 To Do | - Xóa giao dịch và hoàn lại/khấu trừ tiền vào ví tương ứng. |

### 📊 Epic 4: Thống kê & Báo cáo (Analytics)
*Phân tích dữ liệu tài chính.*

| ID | User Story | Priority | Trạng thái | Acceptance Criteria (AC) |
| :--- | :--- | :---: | :---: | :--- |
| **US25** | **Thống kê theo thời gian** | P1 | 📝 To Do | - Lọc theo: Từ ngày -> Đến ngày.<br>- Hiển thị: Dạng bảng chi tiết giao dịch. |
| **US26** | **Thống kê trong ngày** | P0 | 📝 To Do | - Xem nhanh các giao dịch phát sinh trong ngày hôm nay. |
| **US27** | **Thống kê theo ví** | P1 | 📝 To Do | - Lọc giao dịch của 1 ví cụ thể trong 1 khoảng thời gian. |
| **US28** | **Báo cáo định kỳ (Email)** | P2 | 📝 To Do | - Gửi báo cáo tự động (Ngày/Tuần/Tháng).<br>- Nội dung: Tổng thu/chi, Số dư cuối kỳ, Top chi tiêu. |
| **US29** | **Xuất dữ liệu (Export)** | P2 | 📝 To Do | - Hỗ trợ định dạng: Excel, PDF. |

### 🏷️ Epic 5: Danh mục & Ngân sách (Budgeting)
*Phân loại và kiểm soát hạn mức.*

| ID | User Story | Priority | Trạng thái | Acceptance Criteria (AC) |
| :--- | :--- | :---: | :---: | :--- |
| **US31** | **Quản lý danh mục** | P1 | 📝 To Do | - Xem danh sách category (Ăn uống, Mua sắm...).<br>- Thêm/Sửa/Xóa category tùy chỉnh. |
| **US34** | **Bảo vệ danh mục hệ thống** | P1 | 📝 To Do | - Không cho phép xóa các danh mục mặc định của hệ thống. |
| **US36** | **Thiết lập ngân sách** | P2 | 📝 To Do | - Đặt hạn mức chi tiêu cho từng danh mục.<br>- Cảnh báo (Alert) khi chi tiêu vượt quá ngân sách. |
| **US38** | **Theo dõi ngân sách tháng** | P2 | 📝 To Do | - Biểu đồ so sánh Thực chi vs Ngân sách trong tháng. |

### 🔍 Epic 6: Tìm kiếm & Tùy chỉnh (Search & UX)
*Tối ưu hóa khả năng truy xuất.*

| ID | User Story | Priority | Trạng thái | Acceptance Criteria (AC) |
| :--- | :--- | :---: | :---: | :--- |
| **US41** | **Tìm kiếm đa năng** | P1 | 📝 To Do | - Tìm theo: Thể loại, Ngày, Ví, Khoảng tiền (Range slider). |
| **US45** | **Định dạng tiền tệ** | P2 | 📝 To Do | - Tùy chỉnh dấu phân cách (1.000.000 vs 1,000,000). |
| **US47** | **Định dạng ngày tháng** | P2 | 📝 To Do | - Hỗ trợ: DD/MM/YYYY, MM/DD/YYYY, YYYY/MM/DD. |
| **US48** | **Đa ngôn ngữ (i18n)** | P2 | 📝 To Do | - Hỗ trợ: Tiếng Anh (EN), Tiếng Việt (VI). |

### 💬 Epic 7: Tính năng bổ trợ (Social/Chat)
*Tăng cường tương tác.*

| ID | User Story | Priority | Trạng thái | Acceptance Criteria (AC) |
| :--- | :--- | :---: | :---: | :--- |
| **US49** | **Gửi file trong Chat** | P3 | 📝 To Do | - Gửi tài liệu/ảnh qua khung chat tích hợp. |
| **US50** | **Video Call** | P3 | 📝 To Do | - Tích hợp gọi video cho bạn bè/người được share ví. |

---
*Cập nhật lần cuối: 2026-05-02*
*Bởi: Senior Product Owner Agent*
