
# 📧 Web Mail Ảo - Temporary Email Service

[![Version](https://img.shields.io/badge/version-2.0.0-brightgreen.svg)](https://github.com/tuquangnam07/Web-mail-ao)
[![Deploy](https://img.shields.io/badge/deploy-pages.dev-blue.svg)](https://web-mail-ao.pages.dev/)
[![License](https://img.shields.io/badge/license-MIT-orange.svg)](https://opensource.org/licenses/MIT)
[![Made with](https://img.shields.io/badge/Made%20with-❤️-red.svg)](https://github.com/tuquangnam07)

> Dịch vụ email tạm thời miễn phí, bảo mật và tiện lợi. Tạo hộp thư ảo ngay lập tức, nhận email mà không cần đăng ký tài khoản cá nhân.

🌐 **Live Demo**: [https://web-mail-ao.pages.dev/](https://web-mail-ao.pages.dev/)

---

## 📋 Mục lục

- [Tổng quan](#-tổng-quan)
- [Tính năng nổi bật](#-tính-năng-nổi-bật)
- [Công nghệ sử dụng](#-công-nghệ-sử-dụng)
- [Cài đặt & Chạy local](#-cài-đặt--chạy-local)
- [Hướng dẫn sử dụng](#-hướng-dẫn-sử-dụng)
- [Cấu trúc dự án](#-cấu-trúc-dự-án)
- [API & Tích hợp](#-api--tích-hợp)
- [Đóng góp](#-đóng-góp)
- [Giấy phép](#-giấy-phép)
- [Tác giả](#-tác-giả)

---

## 🚀 Tổng quan

**Web Mail Ảo** là một ứng dụng web cho phép người dùng tạo địa chỉ email tạm thời một cách nhanh chóng và hoàn toàn miễn phí. Ứng dụng được xây dựng với mục đích bảo vệ thông tin cá nhân, tránh spam và giúp người dùng nhận email xác minh từ các dịch vụ trực tuyến mà không cần tiết lộ địa chỉ email thật.

### 🎯 Mục đích sử dụng
- ✅ Nhận email xác minh tài khoản
- ✅ Nhận mã OTP (One-Time Password)
- ✅ Đăng ký dùng thử dịch vụ
- ✅ Tránh spam và bảo vệ quyền riêng tư
- ✅ Kiểm tra email nhanh chóng, không cần đăng nhập phức tạp

---

## ✨ Tính năng nổi bật

### 📬 Quản lý hộp thư
- **Tạo email tạm thời**: Chọn tên miền và tạo địa chỉ email ngay lập tức
- **Tự động tạo mật khẩu**: Hệ thống tự tạo mật khẩu an toàn hoặc người dùng có thể tự nhập
- **Lưu phiên đăng nhập**: Tự động lưu token để duy trì trạng thái đăng nhập
- **Xóa tài khoản**: Xóa vĩnh viễn hộp thư và tất cả dữ liệu

### 📨 Quản lý email
- **Hiển thị danh sách email**: Giao diện trực quan với thông tin người gửi, tiêu đề và thời gian
- **Xem chi tiết email**: Hiển thị đầy đủ nội dung HTML và plain text
- **Đánh dấu đã đọc**: Tự động đánh dấu email đã xem
- **Xóa email**: Xóa từng email hoặc toàn bộ danh sách hiển thị
- **Tự động làm mới**: Tự kiểm tra email mới mỗi 30 giây

### 🔍 Phát hiện thông minh
- **Tự động phát hiện OTP**: Nhận diện mã xác minh trong nội dung email (4-8 chữ số)
- **Trích xuất link xác minh**: Tìm và hiển thị các link quan trọng (verify, confirm, activate...)
- **Copy nhanh**: Sao chép OTP và link chỉ với một cú click
- **Nhắc nhở OTP**: Thông báo nổi bật khi phát hiện mã OTP

### 🎨 Giao diện
- **Thiết kế hiện đại**: Glassmorphism với gradient màu sắc tinh tế
- **Responsive**: Tương thích với mọi thiết bị (PC, tablet, mobile)
- **Dark mode**: Tông màu tối bảo vệ mắt, hiển thị nổi bật
- **Hiệu ứng mượt mà**: Animation và transition tạo trải nghiệm thân thiện

---

## 🛠 Công nghệ sử dụng

| Công nghệ | Mô tả |
|-----------|-------|
| **HTML5** | Cấu trúc và nội dung trang web |
| **CSS3** | Thiết kế giao diện, animation, responsive |
| **JavaScript (Vanilla)** | Logic ứng dụng, xử lý sự kiện, API calls |
| **Mail.tm API** | Cung cấp dịch vụ email tạm thời |
| **Cloudflare Pages** | Nền tảng hosting và deploy |
| **GitHub** | Quản lý mã nguồn và phiên bản |

---

## 💻 Cài đặt & Chạy local

### Yêu cầu
- Trình duyệt web hiện đại (Chrome, Firefox, Edge, Safari)
- Kết nối internet

### Cách 1: Sử dụng trực tiếp (không cần cài đặt)
1. Truy cập: [https://web-mail-ao.pages.dev/](https://web-mail-ao.pages.dev/)
2. Trang chủ sẽ tự động chuyển đến phiên bản mới nhất

### Cách 2: Chạy local
```bash
# Clone repository
git clone https://github.com/tuquangnam07/Web-mail-ao.git

# Di chuyển vào thư mục dự án
cd Web-mail-ao

# Mở file index.html bằng trình duyệt
# Hoặc sử dụng live server (VS Code)
```

### Cách 3: Deploy lên Cloudflare Pages
```bash
# Fork repository về tài khoản GitHub của bạn
# Truy cập Cloudflare Pages > Create project > Connect to GitHub
# Chọn repository và deploy
```

---

## 📖 Hướng dẫn sử dụng

### 1️⃣ Tạo hộp thư
1. Chọn tên miền từ danh sách (mặc định là miền đầu tiên)
2. (Tùy chọn) Nhập tên đăng nhập và mật khẩu
3. Click **"🚀 Tạo hộp thư"**
4. Hộp thư sẽ được tạo và tự động đăng nhập

### 2️⃣ Nhận và xem email
1. Sau khi tạo hộp thư, địa chỉ email sẽ hiển thị ở bên trái
2. Sử dụng email này để đăng ký/đăng nhập trên các dịch vụ khác
3. Email mới sẽ tự động xuất hiện trong danh sách
4. Click vào email để xem nội dung chi tiết

### 3️⃣ Sử dụng OTP và link xác minh
1. Khi xem email, hệ thống tự động phát hiện:
   - **Mã OTP**: Hiển thị nổi bật với nút copy
   - **Link xác minh**: Hiển thị danh sách với nút mở link
2. Click **"Copy mã"** để sao chép OTP
3. Click **"🔗"** để mở link xác minh trong tab mới

### 4️⃣ Quản lý hộp thư
- **Làm mới**: Click nút 🔄 hoặc **"Kiểm tra"** để cập nhật email mới
- **Xóa email**: Click **"🗑️ Xóa email"** trong chi tiết email
- **Xóa danh sách**: Click **"🗑️ Xóa hiển thị"** để xóa danh sách email đang hiển thị
- **Xóa tài khoản**: Click **"🗑️ Xóa tài khoản"** để xóa vĩnh viễn hộp thư

---

## 📁 Cấu trúc dự án

```
Web-mail-ao/
├── index.html                     # Trang giới thiệu (landing page)
├── Version_1.0.0/
│   └── index.html                 # Ứng dụng chính
├── Version_2.0.0/
│   └── index.html                 # Ứng dụng chính ( Hiện Tại )
├── README.md                      # Tài liệu hướng dẫn
└── LICENSE                        # Giấy phép MIT
```

---

## 🔌 API & Tích hợp

### Mail.tm API Endpoints

| Endpoint | Method | Mô tả |
|----------|--------|-------|
| `/domains` | GET | Lấy danh sách tên miền hỗ trợ |
| `/accounts` | POST | Tạo tài khoản email mới |
| `/token` | POST | Lấy token xác thực |
| `/me` | GET | Lấy thông tin tài khoản hiện tại |
| `/messages` | GET | Lấy danh sách email |
| `/messages/{id}` | GET | Lấy chi tiết email |
| `/messages/{id}` | PATCH | Cập nhật trạng thái email (seen) |
| `/messages/{id}` | DELETE | Xóa email |
| `/accounts/{id}` | DELETE | Xóa tài khoản |

### Ví dụ gọi API
```javascript
// Tạo tài khoản
const account = await fetch('https://api.mail.tm/accounts', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({
        address: 'user@example.com',
        password: 'secure_password'
    })
});

// Lấy token
const token = await fetch('https://api.mail.tm/token', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({
        address: 'user@example.com',
        password: 'secure_password'
    })
});

// Lấy danh sách email
const messages = await fetch('https://api.mail.tm/messages', {
    headers: { 'Authorization': `Bearer ${token}` }
});
```

---

## 🤝 Đóng góp

Chúng tôi rất hoan nghênh sự đóng góp từ cộng đồng! Dưới đây là cách bạn có thể đóng góp:

### Các cách đóng góp
- 🐛 **Báo lỗi**: Tạo issue khi phát hiện lỗi
- 💡 **Đề xuất tính năng**: Chia sẻ ý tưởng mới
- 📝 **Cải thiện tài liệu**: Sửa lỗi chính tả, thêm hướng dẫn
- 🔧 **Sửa lỗi**: Tạo pull request để fix bug
- ✨ **Thêm tính năng**: Phát triển và gửi pull request

### Quy trình đóng góp
1. Fork repository
2. Tạo branch mới (`git checkout -b feature/AmazingFeature`)
3. Commit thay đổi (`git commit -m 'Add some AmazingFeature'`)
4. Push lên branch (`git push origin feature/AmazingFeature`)
5. Mở Pull Request

---

## 📄 Giấy phép

Dự án được phân phối dưới giấy phép **MIT**. Xem file [LICENSE](LICENSE) để biết thêm chi tiết.

```
MIT License

Copyright (c) 2026 tuquangnam07

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions...
```

---

## 👨‍💻 Tác giả

**tuquangnam07**

- 🔗 GitHub: [@tuquangnam07](https://github.com/tuquangnam07)
- 🌐 Website: [https://web-mail-ao.pages.dev/](https://web-mail-ao.pages.dev/)
- 📧 Email: (Liên hệ qua GitHub)
- 🔗 Facebook: [@tuquangnam07](https://facebook.com/tuquangnam07)
---

## 🙏 Lời cảm ơn

- [Mail.tm](https://mail.tm) - Cung cấp API email tạm thời miễn phí
- [Cloudflare Pages](https://pages.cloudflare.com/) - Nền tảng hosting
- Cộng đồng mã nguồn mở - Nguồn cảm hứng và hỗ trợ

---

## ⭐ Star History

Nếu bạn thấy dự án này hữu ích, hãy cho chúng tôi một ⭐ trên GitHub!

---

## 📞 Hỗ trợ

- **GitHub Issues**: [Tạo issue mới](https://github.com/tuquangnam07/Web-mail-ao/issues)
- **GitHub Discussions**: [Thảo luận chung](https://github.com/tuquangnam07/Web-mail-ao/discussions)

---

<p align="center">
  Made with ❤️ by tuquangnam07
</p>
```

---
