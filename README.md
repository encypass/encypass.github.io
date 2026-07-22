# EncyPass - Trình quản lý mật khẩu

**EncyPass** là một ứng dụng web dạng PWA (Progressive Web App) giúp bạn lưu trữ và quản lý mật khẩu an toàn. Ứng dụng áp dụng kiến trúc **Zero-Knowledge**, mã hóa toàn bộ dữ liệu ngay trên thiết bị trước khi đồng bộ lên đám mây, đảm bảo không ai (kể cả nhà phát triển) có thể xem được dữ liệu của bạn.

🌐 **Trải nghiệm ngay tại:** [https://encypass.github.io/](https://encypass.github.io/)

## ✨ Tính năng nổi bật

- 🔐 **Bảo mật cấp cao:** Mã hóa dữ liệu bằng chuẩn AES-GCM 256-bit với Data Encryption Key (DEK).
- 📶 **Hoạt động ngoại tuyến (Offline):** Hỗ trợ xem, thêm, sửa, xóa dữ liệu ngay cả khi không có kết nối mạng. Tự động đồng bộ khi có mạng trở lại.
- ☁️ **Đồng bộ đám mây:** Dữ liệu đã mã hóa được lưu trữ và đồng bộ an toàn qua Firebase.
- 📱 **Ứng dụng PWA:** Cài đặt trực tiếp lên màn hình chính (Home Screen) trên iOS, Android và Desktop mang lại trải nghiệm như app Native.
- 🛠 **Công cụ tiện ích:** Trình tạo mật khẩu ngẫu nhiên, sao lưu (Export) và khôi phục (Import) dữ liệu dưới dạng file JSON.
- 🛡 **Chống truy cập trái phép:** Tự động khóa bảo vệ hệ thống nếu nhập sai mật khẩu chính nhiều lần.

## 🛠 Công nghệ sử dụng

- **Frontend:** HTML5, JavaScript (ES6+), Tailwind CSS
- **Icons:** Lucide Icons
- **Backend & Database:** Firebase Auth (Google Login), Firebase Firestore
- **PWA:** Service Worker (Offline Support), Web App Manifest
- **Security:** Web Crypto API

## ⚠️ Lưu ý bảo mật quan trọng

- Hệ thống **TUYỆT ĐỐI KHÔNG** lưu trữ *Mật khẩu chính (Master Password)* của bạn. 
- Nếu bạn quên Mật khẩu chính, bạn sẽ **vĩnh viễn mất quyền truy cập** vào kho dữ liệu của mình. Vui lòng ghi nhớ Mật khẩu chính thật kỹ.

## 👨‍💻 Tác giả

Phát triển bởi **Hoàng Đợi**.