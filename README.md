# Hướng dẫn sử dụng Website Tin tức - Phiên bản nâng cao

## 🎉 Tính năng đã hoàn thành

### 1. **Tìm kiếm nâng cao** (`search.php`)
- Tìm kiếm theo từ khóa trong tiêu đề, nội dung và mô tả
- Lọc theo danh mục
- Sắp xếp theo mới nhất hoặc xem nhiều nhất
- Phân trang kết quả tìm kiếm
- Hiển thị số lượng kết quả

### 2. **Trang chi tiết tin tức** (`single.php`) ⭐ MỚI
- Hiển thị đầy đủ nội dung tin tức
- Breadcrumb navigation
- Tự động tăng lượt xem
- Nút chia sẻ lên Facebook, Twitter
- Nút in bài viết
- Tin tức liên quan (cùng danh mục)
- Sidebar xem nhiều nhất
- Sidebar tin mới nhất

### 3. **AJAX Tìm kiếm tự động** (`ajax-search.php`) ⭐ MỚI
- Autocomplete khi gõ từ khóa (tối thiểu 2 ký tự)
- Hiển thị gợi ý với hình ảnh, tiêu đề, danh mục
- Click vào gợi ý để chuyển đến trang chi tiết

### 4. **Print-friendly version** (`print.php`) ⭐ MỚI
- Trang in tối ưu cho bài viết
- CSS riêng cho in ấn
- Nút in và đóng

### 5. **Tất cả tin tức** (`all-news.php`)
- Hiển thị tất cả tin tức với phân trang
- Sắp xếp theo mới nhất hoặc xem nhiều nhất
- Layout 3 cột responsive
- Links đến trang chi tiết

### 6. **Trang danh mục** (`archive.php`)
- Hiển thị tin tức theo danh mục
- Phân trang Bootstrap 4
- Links đến trang chi tiết
- Thống kê số lượng

### 7. **Trang kết quả tìm kiếm** (`result.php`)
- Tìm kiếm cơ bản từ header
- Phân trang
- Links đến trang chi tiết

### 8. **Advanced Features** ⭐ MỚI
- Scroll to top button (hiện khi scroll xuống)
- Hiệu ứng hover cho các elements
- CSS tối ưu cho in ấn
- Animations mượt mà

## 📁 Cấu trúc file

```
news-demo/
├── single.php              # Trang chi tiết tin tức (MỚI)
├── ajax-search.php         # API AJAX search (MỚI)
├── print.php               # Trang in bài viết (MỚI)
├── advanced-features.php   # CSS & JS nâng cao (MỚI)
├── search.php              # Tìm kiếm nâng cao
├── all-news.php            # Tất cả tin tức
├── archive.php             # Trang danh mục
├── result.php              # Kết quả tìm kiếm
├── models/
│   ├── item.php            # Model Item (đã nâng cấp)
│   └── category.php        # Model Category (đã nâng cấp)
├── header.php              # Header (đã cập nhật menu)
└── footer.php              # Footer (đã tích hợp advanced features)
```

## 🔧 Model đã nâng cấp

### Model `Item` (`models/item.php`)
**Phương thức mới:**
- `getItemById($id)` - Lấy tin tức theo ID
- `increaseViews($id)` - Tăng lượt xem
- `getRelatedItems($category_id, $current_id, $limit)` - Lấy tin liên quan
- `getMostViewedItems($limit)` - Lấy tin xem nhiều nhất
- `getLatestItems($limit)` - Lấy tin mới nhất
- `searchAdvanced()` - Tìm kiếm nâng cao
- `searchCountAdvanced()` - Đếm kết quả nâng cao
- `getItemsWithPagination()` - Lấy tin với phân trang
- `getTotalItems()` - Đếm tổng số tin
- `paginate()` - Phân trang Bootstrap 4 cải tiến

### Model `Category` (`models/category.php`)
**Phương thức mới:**
- `getCateById($id)` - Lấy thông tin danh mục theo ID

## 🚀 Hướng dẫn sử dụng

### 1. Cài đặt
```bash
# Import database
1. Mở phpMyAdmin
2. Tạo database tên 'news'
3. Import file news.sql

# Cấu hình
1. Mở config.php
2. Kiểm tra thông tin kết nối database
```

### 2. Chạy website
```bash
1. Khởi động XAMPP (Apache + MySQL)
2. Truy cập: http://localhost/news-demo
```

### 3. Sử dụng tính năng

**Tìm kiếm AJAX:**
- Gõ từ khóa vào ô tìm kiếm ở header
- Chờ gợi ý hiện ra (sau 2 ký tự)
- Click vào gợi ý để xem chi tiết

**Xem chi tiết tin tức:**
- Click vào tiêu đề bất kỳ tin tức nào
- Xem đầy đủ nội dung
- Chia sẻ lên mạng xã hội
- In bài viết
- Xem tin liên quan

**Tìm kiếm nâng cao:**
- Vào menu "Tìm kiếm nâng cao"
- Nhập từ khóa, chọn danh mục, sắp xếp
- Xem kết quả với phân trang

## 🎨 Tính năng UI/UX

### Phân trang
- Bootstrap 4 pagination
- Hiển thị: Trước | 1 2 3 ... | Sau
- Trang hiện tại được highlight
- Responsive trên mobile

### AJAX Search
- Autocomplete real-time
- Hiển thị hình ảnh thumbnail
- Thông tin danh mục và ngày đăng
- Số lượt xem

### Scroll to Top
- Nút tròn màu xanh
- Hiện khi scroll > 300px
- Smooth scroll animation
- Fixed position

### Print Styles
- CSS riêng cho in ấn
- Ẩn các element không cần thiết
- Font size tối ưu
- Page break control

## 📊 Thống kê

- **Tổng số trang:** 8 trang
- **Tổng số phương thức mới:** 11 phương thức
- **Dòng code thêm mới:** ~1000+ dòng
- **Tính năng nâng cao:** 8 tính năng

## 🔒 Bảo mật

- ✅ Prepared Statements (SQL Injection protection)
- ✅ HTML Escaping (XSS protection)
- ✅ URL Encoding
- ✅ Input validation

## 🌐 Tương thích

- ✅ Desktop (Chrome, Firefox, Edge, Safari)
- ✅ Tablet
- ✅ Mobile
- ✅ Print

## 💡 Gợi ý phát triển tiếp

1. **Comments System** - Hệ thống bình luận
2. **User Authentication** - Đăng nhập/đăng ký
3. **Admin Panel** - Quản trị nội dung
4. **Rich Text Editor** - Soạn thảo nội dung
5. **Image Upload** - Upload ảnh
6. **Tags System** - Hệ thống tags
7. **RSS Feed** - RSS feed
8. **Email Subscription** - Đăng ký nhận tin
9. **Social Login** - Đăng nhập bằng Facebook/Google
10. **Analytics** - Thống kê truy cập

## 🐛 Troubleshooting

**Lỗi AJAX không hoạt động:**
- Kiểm tra jQuery đã load chưa
- Kiểm tra đường dẫn ajax-search.php
- Xem Console log

**Lỗi phân trang:**
- Kiểm tra tham số page trong URL
- Kiểm tra hàm paginate()

**Lỗi không tăng lượt xem:**
- Kiểm tra quyền UPDATE trong database
- Kiểm tra hàm increaseViews()

## 📞 Hỗ trợ

Nếu gặp vấn đề, kiểm tra:
1. XAMPP đã khởi động chưa
2. Database đã import đúng chưa
3. File config.php có đúng thông tin kết nối không
4. Đường dẫn ảnh trong thư mục `img/` có tồn tại không
5. Console log có lỗi JavaScript không

---

**Phiên bản:** 2.0 (Advanced Features)  
**Ngày cập nhật:** <?php echo date('d/m/Y'); ?>  
**Tác giả:** Your Name
