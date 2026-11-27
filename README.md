# 🔐 EncyPass — Zero-Knowledge Password Manager PWA (AES-GCM 256-bit)

**EncyPass** is a lightweight, offline-first **Zero-Knowledge Password Manager Progressive Web App (PWA)** built with native **Web Crypto API (AES-GCM 256-bit & PBKDF2)** and **Firebase**.  
**EncyPass** là trình quản lý mật khẩu hoạt động ngoại tuyến (**Offline-First PWA**) ứng dụng kiến trúc bảo mật **Zero-Knowledge** với mã hóa đầu cuối **AES-GCM 256-bit** và **PBKDF2** ngay trên trình duyệt.

[![Live App](https://img.shields.io/badge/Live_App-encypass.web.app-2563eb?style=for-the-badge&logo=firebase&logoColor=white)](https://encypass.web.app/)
[![Download Latest Release](https://img.shields.io/badge/Download-Latest_Release-16a34a?style=for-the-badge&logo=github&logoColor=white)](https://github.com/encypass/encypass.github.io/releases)
[![Deployment Guide](https://img.shields.io/badge/Docs-Self--Hosting_Guide-0284c7?style=for-the-badge&logo=readthedocs&logoColor=white)](https://encypass.web.app/deployment-guide)

> **Lưu ý / Notice:** Repository này chỉ lưu trữ tài liệu giới thiệu và phân phối gói cài đặt chính thức tại trang **[GitHub Releases](https://github.com/encypass/encypass.github.io/releases)**. Ứng dụng web chính thức duy nhất được vận hành tại **[EncyPass Official Web App (encypass.web.app)](https://encypass.web.app/)**.

---

## 🌐 Ứng dụng chính thức & Tài liệu kỹ thuật (Official Links & Docs)

| Chuyên mục / Section | Đường dẫn tối ưu / Direct Resource Link | Mô tả nội dung / Description |
| :--- | :--- | :--- |
| 🚀 **Ứng dụng chính thức** | **[EncyPass Web App — Trình quản lý mật khẩu PWA](https://encypass.web.app/)** | Truy cập trực tiếp trình quản lý mật khẩu mã hóa đầu cuối trên trình duyệt. |
| 📦 **Tải gói mã nguồn** | **[EncyPass Releases — Tải bản phát hành mới nhất](https://github.com/encypass/encypass.github.io/releases)** | Tải tệp `.zip` mã nguồn sạch mới nhất để tự lưu trữ (Self-Hosted). |
| 🛠️ **Hướng dẫn cài đặt** | **[EncyPass Deployment Guide — Tự triển khai lên Firebase](https://encypass.web.app/deployment-guide)** | Tài liệu từng bước cấu hình Firebase Hosting, Firestore và Authentication. |
| ℹ️ **Kiến trúc bảo mật** | **[EncyPass Security Architecture — Cơ chế Zero-Knowledge](https://encypass.web.app/about)** | Chi tiết cơ chế dẫn xuất khóa PBKDF2, DEK và bảo vệ bộ nhớ RAM. |
| ❓ **Hỏi đáp (FAQ)** | **[EncyPass FAQ — Câu hỏi thường gặp về bảo mật & sao lưu](https://encypass.web.app/faq)** | Giải đáp về khôi phục mật khẩu chính, đồng bộ đám mây và chế độ ngoại tuyến. |
| 📋 **Nhật ký cập nhật** | **[EncyPass Changelog — Lịch sử nâng cấp tính năng](https://encypass.web.app/changelog)** | Theo dõi các cải tiến bảo mật và tính năng mới qua từng đợt phát hành. |

---

## 🛡️ Kiến trúc bảo mật Zero-Knowledge & Tính năng cốt lõi

### 🇻🇳 Tiếng Việt
* **Mã hóa đầu cuối phía khách hàng (Client-Side Encryption):** Toàn bộ dữ liệu được mã hóa cục bộ bằng **Web Crypto API** chuẩn trình duyệt với thuật toán **AES-GCM 256-bit** trước khi lưu vào IndexedDB hoặc đồng bộ lên Cloud Firestore.
* **Dẫn xuất khóa PBKDF2 & Bảo vệ RAM:** Mật khẩu chính (Master Password) không bao giờ rời khỏi thiết bị. Khóa giải mã dữ liệu (DEK) chỉ tồn tại tạm thời trong bộ nhớ RAM và tự động xóa sạch khi khóa ứng dụng hoặc không thao tác.
* **Hoạt động ngoại tuyến (Offline-First PWA):** Cài đặt trực tiếp lên điện thoại (Android/iOS) và máy tính như ứng dụng gốc; tra cứu mật khẩu ngay cả khi mất kết nối Internet nhờ Service Worker.
* **Sao lưu & Khôi phục độc lập:** Hỗ trợ xuất/nhập tệp sao lưu đã mã hóa (`EncyPass_*.json`), không phụ thuộc hoàn toàn vào máy chủ đám mây.
* **Hỗ trợ đa ngôn ngữ:** Giao diện chuyển đổi mượt mà giữa Tiếng Việt, Tiếng Anh và nhiều ngôn ngữ quốc tế khác.

### 🇺🇸 English Overview
* **Client-Side End-to-End Encryption:** Vault records are encrypted locally inside your browser using native **Web Crypto API (AES-GCM 256-bit)** before local persistence or cloud synchronization.
* **PBKDF2 Key Derivation & RAM-Only Lifecycle:** Your Master Password never leaves your device. Decryption keys remain strictly in volatile RAM during active sessions and are wiped automatically upon lock or inactivity.
* **Installable Offline-First PWA:** Works seamlessly offline across mobile and desktop devices using Service Workers and IndexedDB.
* **Cloud Sync & Encrypted JSON Backups:** Optional multi-device synchronization via Firebase alongside portable encrypted JSON backup exports.

---

## 🚀 Tự triển khai mã nguồn (Self-Hosting Quick Start)

1. Truy cập trang **[EncyPass GitHub Releases](https://github.com/encypass/encypass.github.io/releases)** và tải tệp mã nguồn đóng gói (`.zip`) ở bản phát hành mới nhất nằm trên cùng.
2. Làm theo hướng dẫn cấu hình dự án Firebase và triển khai lên hosting riêng tại **[EncyPass Self-Hosting Deployment Guide](https://encypass.web.app/deployment-guide)**.

---

## ❓ Câu hỏi thường gặp (FAQ)

**EncyPass có lưu mật khẩu chính (Master Password) trên máy chủ không?**  
Không. Theo kiến trúc **Zero-Knowledge**, mật khẩu chính chỉ dùng để dẫn xuất khóa cục bộ trên trình duyệt của bạn. Máy chủ chỉ lưu trữ các chuỗi dữ liệu đã được mã hóa. Xem thêm tại **[EncyPass FAQ](https://encypass.web.app/faq)**.

**Tôi có thể dùng EncyPass khi mất mạng Internet không?**  
Có. EncyPass được xây dựng theo chuẩn **Offline-First PWA**, lưu đệm toàn bộ giao diện và kho dữ liệu mã hóa ngay trên thiết bị để sử dụng mọi lúc mọi nơi.

**Làm sao để cập nhật phiên bản mới khi tự triển khai (Self-Hosted)?**  
Bạn chỉ cần tải gói `.zip` mới nhất tại **[GitHub Releases](https://github.com/encypass/encypass.github.io/releases)** và làm theo mục cập nhật trong **[Deployment Guide](https://encypass.web.app/deployment-guide)**.

---

## 👤 Tác giả / Author

* **Hoàng Đợi** — Phát triển và vận hành tại **[encypass.web.app](https://encypass.web.app/)**
