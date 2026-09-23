# EncyPass – Trình quản lý mật khẩu

**EncyPass** là ứng dụng web hiện đại (PWA) giúp bạn lưu trữ và quản lý mật khẩu an toàn. Được xây dựng dựa trên kiến trúc **Zero-Knowledge**, toàn bộ dữ liệu của bạn sẽ được mã hóa trực tiếp trên thiết bị trước khi đồng bộ lên đám mây. Điều này đảm bảo không một ai — kể cả nhà phát triển — có thể giải mã và đọc được thông tin của bạn.

🌐 **Trải nghiệm ngay tại:** [https://encypass.github.io/](https://encypass.github.io/)

## ✨ Tính năng nổi bật

- 🔐 **Bảo mật tối đa:** Dữ liệu được mã hóa bằng thuật toán AES-GCM 256-bit kết hợp với Khóa bảo vệ dữ liệu (DEK).
- 📶 **Hoạt động ngoại tuyến (Offline):** Thoải mái xem, thêm, sửa hoặc xóa mật khẩu ngay cả khi mất kết nối mạng. Ứng dụng sẽ tự động đồng bộ mọi thay đổi ngay khi có mạng trở lại.
- ☁️ **Đồng bộ đám mây thông minh:** Dữ liệu mã hóa được lưu trữ an toàn qua hệ thống Firebase. Bạn có thể dễ dàng quản lý, tải về hoặc khôi phục các bản sao lưu đồng bộ xuyên suốt các thiết bị cá nhân.
- 📱 **Trải nghiệm liền mạch (PWA):** Cài đặt trực tiếp lên màn hình chính của iOS, Android và Desktop để sử dụng mượt mà, tiện lợi như một ứng dụng gốc (native app).
- 🛠 **Bộ công cụ tích hợp:** Hỗ trợ tạo mật khẩu ngẫu nhiên có độ khó cao. Sao lưu và khôi phục dữ liệu cục bộ (file JSON) được đính kèm các thông tin trực quan như phiên bản và tổng số tài khoản.
- 🛡 **Chống truy cập trái phép:** Hệ thống sẽ tự động khóa và hiển thị đếm ngược thời gian chờ nếu phát hiện người lạ cố tình nhập sai Mật khẩu chính nhiều lần.

## 🛠 Công nghệ sử dụng

- **Giao diện (Frontend):** HTML5, JavaScript (ES6+), Tailwind CSS, Lucide Icons
- **Hệ thống (Backend & DB):** Firebase Auth (Đăng nhập Google), Firebase Firestore, Firebase Cloud Storage
- **Nền tảng (PWA):** Service Worker (Xử lý Offline), Web App Manifest
- **Bảo mật:** Web Crypto API

## ⚠️ Lưu ý bảo mật quan trọng

- Hệ thống **TUYỆT ĐỐI KHÔNG** lưu trữ *Mật khẩu chính (Master Password)* của bạn. 
- Nếu quên Mật khẩu chính, bạn sẽ **mất vĩnh viễn quyền truy cập** vào kho dữ liệu của mình. Hãy chắc chắn rằng bạn đã ghi nhớ thật kỹ hoặc lưu giữ mật khẩu này ở một nơi an toàn trước khi sử dụng.

## 👨‍💻 Tác giả

Phát triển bởi **Hoàng Đợi**.