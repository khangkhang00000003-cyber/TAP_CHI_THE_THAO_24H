# Tạp chí thể thao 24h — source website

## Cấu trúc file
- `index.html`: trang chủ tạp chí, tìm kiếm, lọc danh mục, các bài xem nhanh và liên kết tới bài SEO chuyên sâu.
- `cach-chon-giay-chay-bo-cho-nguoi-moi.html`: bài viết SEO hoàn chỉnh, được liên kết ở khu vực Bài nổi bật và đầu danh sách Bài viết mới nhất trên trang chủ.
- `SEO-ONPAGE-SEOQUAKE-CHECKLIST.md`: checklist tự kiểm tra On-page và SEOquake.

## Định vị website
Đây là website biên tập blog độc lập có tên **Tạp chí thể thao 24h**, không phải trang chủ của cửa hàng SPORTHUB. Thanh điều hướng và footer chỉ liên kết giữa các chuyên mục/bài viết trong tạp chí. Liên kết đến website chính SPORTHUB chỉ được đặt theo ngữ cảnh trong nội dung bài viết, thay vì đặt ở menu chính hoặc footer.

Trang chính SPORTHUB hiện được liên kết ở bài SEO mẫu bằng URL:
`https://tranthiquynhnhu0901-hue.github.io/the-thao-song-khoe/`

Vì URL GitHub Pages riêng của Tạp chí thể thao 24h chưa được cung cấp, **canonical absolute, og:url và URL đầy đủ trong dữ liệu cấu trúc** được để chờ cập nhật sau khi bạn tạo repo riêng. Khi biết URL xuất bản chính thức, hãy khai báo canonical URL cho cả trang chủ và bài viết, cập nhật `og:url`, `mainEntityOfPage` và sitemap XML nếu cần. Không trỏ canonical của tạp chí về website cửa hàng SPORTHUB.

## Đưa website lên GitHub Pages
1. Tạo một repository riêng, ví dụ `tap-chi-the-thao-24h`.
2. Upload tất cả ba file HTML/MD cùng thư mục, đặc biệt không chỉ upload mỗi `index.html`.
3. Vào **Settings → Pages**, chọn nhánh và thư mục xuất bản.
4. Mở URL GitHub Pages riêng. Kiểm tra menu, tìm kiếm, lọc danh mục, thẻ bài SEO và các đường dẫn tương đối.
5. Khi URL chính thức đã hoạt động, cập nhật canonical/OG/JSON-LD, thêm sitemap XML với URL tuyệt đối thực tế, rồi chạy SEOquake trên trang đã xuất bản.

## Ảnh
Các ảnh được gọi trực tiếp từ Unsplash/Pexels nên cần Internet; tệp ảnh không được đóng gói trong repo.
