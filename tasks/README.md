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
| ID | User Story | Priority | Trạng thái | Acceptance Criteria (AC) |
| :--- | :--- | :---: | :---: | :--- |
| **US01** | **Đăng ký tài khoản** | P0 | 📝 To Do | - Form: Username, Password (6-8 kí tự).<br>- Flow: Đăng ký thành công chuyển hướng sang Login. |
| **US02** | **Đăng nhập hệ thống** | P0 | 📝 To Do | - Input: Username, Password.<br>- Flow: Đăng nhập thành công chuyển hướng về Dashboard. |
| **US03** | **Đăng nhập Social** | P1 | 📝 To Do | - Hỗ trợ: Facebook, Google, Github. |
| **US04** | **Đăng xuất** | P0 | 📝 To Do | - Flow: Xóa session và chuyển về Login. |
| **US05** | **Quên mật khẩu** | P1 | 📝 To Do | - Flow: Gửi mật khẩu random 8 ký tự qua email. |
| **US06** | **Kích hoạt tài khoản** | P1 | 📝 To Do | - Flow: Gửi email active tài khoản sau khi đăng ký. |
| **US07** | **Đổi mật khẩu** | P1 | 📝 To Do | - Form: Mật khẩu cũ, Mật khẩu mới, Xác nhận mật khẩu. |
| **US08** | **Xóa tài khoản** | P2 | 📝 To Do | - Flow: Xóa sạch dữ liệu liên quan và yêu cầu xác nhận. |
| **US09** | **Cập nhật Profile** | P2 | 📝 To Do | - Cập nhật: Ảnh đại diện, Số điện thoại. |

### 💳 Epic 2: Quản lý Ví (Wallet Core)
| ID | User Story | Priority | Trạng thái | Acceptance Criteria (AC) |
| :--- | :--- | :---: | :---: | :--- |
| **US10** | **Thêm ví mới** | P0 | 📝 To Do | - Popup: Icon, Tên ví, Số tiền, Loại tiền tệ, Mô tả. |
| **US11** | **Sửa thông tin ví** | P1 | 📝 To Do | - Form: Icon, Tên ví, Số tiền, Loại tiền tệ, Mô tả. |
| **US12** | **Xóa ví** | P1 | 📝 To Do | - Flow: Xóa ví và toàn bộ giao dịch liên quan. |
| **US13** | **Chia sẻ ví** | P2 | 📝 To Do | - Flow: Share ví qua email tài khoản khác. |
| **US14** | **Xóa quyền share** | P2 | 📝 To Do | - Flow: Xóa tài khoản đã được share ví trước đó. |
| **US15** | **Phân quyền ví** | P2 | 📝 To Do | - Quyền: Viewer (Chỉ xem), Owner (Toàn quyền). |
| **US16** | **Chọn ví chi tiêu** | P0 | 📝 To Do | - Flow: Chọn ví hiện tại trên thanh điều hướng. |
| **US17** | **Chuyển tiền nội bộ** | P1 | 📝 To Do | - Flow: Chuyển tiền từ ví A sang ví B. |
| **US18** | **Lưu trữ ví** | P2 | 📝 To Do | - Flow: Khóa ví (Read-only) và các giao dịch liên quan. |
| **US19** | **Xem danh sách ví** | P0 | 📝 To Do | - Hiển thị: Icon, Tên ví, Tổng nạp, Số tiền hiện có. |
| **US20** | **Xem tổng tài sản** | P0 | 📝 To Do | - Hiển thị tổng số dư của tất cả các ví tại trang chủ. |

### 💰 Epic 3: Giao dịch (Transaction Engine)
| ID | User Story | Priority | Trạng thái | Acceptance Criteria (AC) |
| :--- | :--- | :---: | :---: | :--- |
| **US21** | **Nạp tiền vào ví** | P0 | 📝 To Do | - Form: Số tiền, Ghi chú, Ví nhận. |
| **US22** | **Ghi lại khoản chi** | P0 | 📝 To Do | - Form: Số tiền, Danh mục, Ví chi, Ghi chú, Thời gian. |
| **US23** | **Sửa khoản chi** | P1 | 📝 To Do | - Form: Số tiền, Danh mục, Ví chi, Ghi chú, Thời gian. |
| **US24** | **Xóa khoản chi** | P1 | 📝 To Do | - Flow: Xóa giao dịch và hoàn tiền lại ví. |

### 📊 Epic 4: Thống kê & Báo cáo (Analytics)
| ID | User Story | Priority | Trạng thái | Acceptance Criteria (AC) |
| :--- | :--- | :---: | :---: | :--- |
| **US25** | **Thống kê theo thời gian** | P1 | 📝 To Do | - Lọc theo khoảng thời gian bắt đầu/kết thúc. |
| **US26** | **Thống kê trong ngày** | P0 | 📝 To Do | - Hiển thị danh sách thu chi ngày hôm nay. |
| **US27** | **Thống kê ví theo time** | P1 | 📝 To Do | - Lọc thu chi của từng ví theo khoảng thời gian. |
| **US28** | **Thống kê ví trong ngày** | P1 | 📝 To Do | - Lọc thu chi của từng ví trong ngày hôm nay. |
| **US29** | **Xuất file báo cáo** | P2 | 📝 To Do | - Xuất thống kê ra định dạng Excel, PDF. |
| **US30** | **Báo cáo qua Email** | P2 | 📝 To Do | - Tự động gửi báo cáo ngày/tuần/tháng về email. |

### 🏷️ Epic 5: Danh mục & Ngân sách (Budgeting)
| ID | User Story | Priority | Trạng thái | Acceptance Criteria (AC) |
| :--- | :--- | :---: | :---: | :--- |
| **US31** | **Xem danh mục tiêu dùng** | P1 | 📝 To Do | - Hiển thị các danh mục chi tiêu mặc định và tùy chỉnh. |
| **US32** | **Thêm danh mục mới** | P1 | 📝 To Do | - Form: Tên danh mục, Ghi chú. |
| **US33** | **Sửa danh mục** | P1 | 📝 To Do | - Form: Tên danh mục, Ghi chú. |
| **US34** | **Xóa danh mục** | P1 | 📝 To Do | - Chỉ xóa được danh mục tự tạo, không xóa mục mặc định. |
| **US35** | **Xem giao dịch theo mục** | P1 | 📝 To Do | - Hiển thị danh sách giao dịch thuộc 1 danh mục cụ thể. |
| **US36** | **Thêm ngân sách (Budget)** | P2 | 📝 To Do | - Đặt hạn mức chi tiêu cho 1 danh mục. Cảnh báo khi vượt. |
| **US37** | **Sửa ngân sách** | P2 | 📝 To Do | - Thay đổi số tiền hạn mức ban đầu. |
| **US38** | **Thống kê ngân sách tháng** | P2 | 📝 To Do | - Xem số tiền còn lại và danh sách giao dịch trong ngân sách. |
| **US39** | **Xóa ngân sách** | P2 | 📝 To Do | - Hủy bỏ hạn mức chi tiêu của một danh mục. |
| **US40** | **Xem giao dịch ngân sách** | P2 | 📝 To Do | - Hiển thị danh sách giao dịch thuộc 1 ngân sách cụ thể. |

### 🔍 Epic 6: Tìm kiếm & Tùy chỉnh (Search & UX)
| ID | User Story | Priority | Trạng thái | Acceptance Criteria (AC) |
| :--- | :--- | :---: | :---: | :--- |
| **US41** | **Tìm theo thể loại** | P1 | 📝 To Do | - Lọc giao dịch theo category. |
| **US42** | **Tìm theo ngày** | P1 | 📝 To Do | - Lọc giao dịch theo 1 ngày cụ thể. |
| **US43** | **Tìm theo ví bất kỳ** | P1 | 📝 To Do | - Lọc giao dịch của 1 ví bất kỳ. |
| **US44** | **Lọc theo khoảng tiền** | P1 | 📝 To Do | - Lọc giao dịch theo khoảng số tiền (Min - Max). |
| **US45** | **Định dạng tiền tệ** | P2 | 📝 To Do | - Cài đặt dấu phân cách số tiền (dấu phẩy/dấu chấm). |
| **US46** | **Cài đặt đơn vị tiền tệ** | P2 | 📝 To Do | - Chọn đơn vị hiển thị: VND, USD, Euro... |
| **US47** | **Định dạng ngày tháng** | P2 | 📝 To Do | - Chọn định dạng: DD/MM/YYYY, MM/DD/YYYY, v.v. |
| **US48** | **Đa ngôn ngữ** | P2 | 📝 To Do | - Hỗ trợ chuyển đổi Tiếng Anh và Tiếng Việt. |

### 💬 Epic 7: Tính năng bổ trợ (Social/Chat)
| ID | User Story | Priority | Trạng thái | Acceptance Criteria (AC) |
| :--- | :--- | :---: | :---: | :--- |
| **US49** | **Gửi file qua chat** | P3 | 📝 To Do | - Chức năng gửi tài liệu/ảnh trong khung chat. |
| **US50** | **Video Call** | P3 | 📝 To Do | - Tích hợp gọi video cho bạn bè trong ứng dụng. |

---
*Cập nhật lần cuối: 2026-05-02*
*Bởi: Senior Product Owner Agent*
