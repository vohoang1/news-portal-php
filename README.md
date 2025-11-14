# news-portal-php
📰 A simple, responsive news website built with PHP and MySQL — perfect for learning, portfolio, or academic projects. 
# 📰 News Portal – Trang Tin Tức PHP

Một trang web tin tức đơn giản, hiện đại, được xây dựng bằng **PHP thuần** và **MySQL**, với giao diện responsive — phù hợp cho sinh viên công nghệ làm **đồ án học phần, portfolio cá nhân** hoặc luyện tập kỹ năng fullstack cơ bản.

---

## 🌟 Tính năng

- Giao diện **responsive**, hiển thị đẹp trên điện thoại & máy tính.
- Hiển thị tin theo **danh mục** (Thời sự, Thế giới, Khoa học, Giải trí, Thể thao, Quân sự…).
- Bài viết có **ảnh minh họa, tiêu đề, mô tả ngắn, ngày đăng**.
- Thanh điều hướng rõ ràng + thanh tìm kiếm + cột mạng xã hội.
- Kết nối cơ sở dữ liệu qua `mysqli` (PHP).
- Cấu trúc code rõ ràng: tách biệt header, footer, kết nối DB.

---

## 🛠 Công nghệ sử dụng

- **Backend**: PHP 7.4+
- **Database**: MySQL
- **Frontend**: HTML5, CSS3, Bootstrap 4 (nếu có), JavaScript cơ bản
- **Môi trường**: WAMP / XAMPP (localhost)

---

## 🗂 Cấu trúc dự án
news-demo/
├── index.php # Trang chủ
├── header.php # Phần đầu trang
├── footer.php # Phần chân trang
├── models/
│ └── db.php # Kết nối CSDL (database: be1)
├── single.php # Chi tiết bài viết
├── category.php # Tin theo danh mục
└── assets/ # Hình ảnh, CSS, JS


---

## ⚙️ Hướng dẫn cài đặt

1. **Clone hoặc tải mã nguồn** về thư mục `www` (WAMP) hoặc `htdocs` (XAMPP).
2. **Tạo database** tên `be1` trong phpMyAdmin.
   ```sql
   CREATE DATABASE be1 CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;

   Tuyệt! Dưới đây là nội dung đầy đủ cho file **`README.md`** — đã được **tối ưu cho GitHub**, kết hợp cả hình ảnh bạn đã upload, mô tả rõ ràng, và phù hợp với một dự án học tập bằng PHP như của bạn:

---

```markdown
# 📰 News Portal – Trang Tin Tức PHP

![Giao diện trang chủ](image.png)

Một trang web tin tức đơn giản, hiện đại, được xây dựng bằng **PHP thuần** và **MySQL**, với giao diện responsive — phù hợp cho sinh viên công nghệ làm **đồ án học phần, portfolio cá nhân** hoặc luyện tập kỹ năng fullstack cơ bản.

---

## 🌟 Tính năng

- Giao diện **responsive**, hiển thị đẹp trên điện thoại & máy tính.
- Hiển thị tin theo **danh mục** (Thời sự, Thế giới, Khoa học, Giải trí, Thể thao, Quân sự…).
- Bài viết có **ảnh minh họa, tiêu đề, mô tả ngắn, ngày đăng**.
- Thanh điều hướng rõ ràng + thanh tìm kiếm + cột mạng xã hội.
- Kết nối cơ sở dữ liệu qua `mysqli` (PHP).
- Cấu trúc code rõ ràng: tách biệt header, footer, kết nối DB.

---

## 🛠 Công nghệ sử dụng

- **Backend**: PHP 7.4+
- **Database**: MySQL
- **Frontend**: HTML5, CSS3, Bootstrap 4 (nếu có), JavaScript cơ bản
- **Môi trường**: WAMP / XAMPP (localhost)

---

## 🗂 Cấu trúc dự án

```
news-demo/
├── index.php          # Trang chủ
├── header.php         # Phần đầu trang
├── footer.php         # Phần chân trang
├── models/
│   └── db.php         # Kết nối CSDL (database: be1)
├── single.php         # Chi tiết bài viết
├── category.php       # Tin theo danh mục
└── assets/            # Hình ảnh, CSS, JS
```

---

## ⚙️ Hướng dẫn cài đặt

1. **Clone hoặc tải mã nguồn** về thư mục `www` (WAMP) hoặc `htdocs` (XAMPP).
2. **Tạo database** tên `be1` trong phpMyAdmin.
   ```sql
   CREATE DATABASE be1 CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
   ```
3. **Tạo bảng và chèn dữ liệu mẫu** (nếu có file `.sql`, hãy import).
4. **Kiểm tra lại kết nối** trong `models/db.php`:
   ```php
   new mysqli('localhost', 'root', '', 'be1', 3306);
   ```
5. **Bật Apache + MySQL**, truy cập:
   ```
   http://localhost/news-demo
   ```

> 💡 Lưu ý: Tên thư mục trên server phải khớp với đường dẫn bạn truy cập.

---

## 🎓 Mục đích

- Đồ án học phần **Lập trình Web** – ngành Công nghệ Thông tin.
- Rèn luyện kỹ năng PHP, thao tác với MySQL, thiết kế giao diện người dùng.
- Làm nền tảng để mở rộng (thêm đăng nhập, bình luận, quản trị…).

---

## 📄 Giấy phép

MIT License – Tự do sử dụng và chỉnh sửa cho mục đích học tập.

---

> 🔧 Dự án này **không sử dụng framework**, phù hợp để hiểu rõ luồng hoạt động cơ bản của website động với PHP & MySQL.
```

---

### ✅ Cách dùng:
1. Tạo file `README.md` trong thư mục gốc của dự án (`news-demo/`).
2. Dán toàn bộ nội dung trên vào.
3. Đảm bảo file `image.png` nằm cùng thư mục với `README.md` → GitHub sẽ tự hiển thị hình ảnh.

> 💡 Nếu bạn đổi tên ảnh thành `screenshot.png` hoặc `preview.jpg`, nhớ sửa dòng `![Giao diện trang chủ](image.png)` cho khớp.

---

Bạn cần mình xuất ra file `.md` thật để tải về, hay thêm phần **"Demo video"**, **"Cách mở rộng tính năng"**, hoặc **"Lỗi thường gặp"** không? Mình sẵn sàng hỗ trợ! 😊
