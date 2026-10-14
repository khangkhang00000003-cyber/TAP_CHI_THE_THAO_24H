# SEO On-page + SEOquake checklist — Tạp chí thể thao 24h

## 1. Thông tin SEO đã cài trong HTML

| Hạng mục | Giá trị / cách kiểm tra |
|---|---|
| Website | Tạp chí thể thao 24h — blog/tạp chí riêng, không phải trang cửa hàng SPORTHUB |
| Bài mẫu | Cách chọn giày chạy bộ cho người mới: 7 tiêu chí cần biết |
| Từ khóa chính | `cách chọn giày chạy bộ` |
| Từ khóa phụ | `giày chạy bộ cho người mới`, `chọn size giày chạy bộ`, `giày chạy đường nhựa`, `giày chạy địa hình` |
| URL/slug | `/cach-chon-giay-chay-bo-cho-nguoi-moi.html` — chữ thường, không dấu, dùng dấu gạch ngang |
| SEO title | `Cách chọn giày chạy bộ cho người mới: 7 tiêu chí` |
| Meta description | Hướng dẫn chọn size, độ đệm, form chân, địa hình và ngân sách; tóm tắt đúng ý định tìm kiếm. |
| H1 | Một H1 duy nhất, trùng ý định tìm kiếm và có từ khóa chính |
| H2/H3 | Phân chia theo mục tiêu/cung đường, size/form, đệm, hỗ trợ, độ bám, ngân sách, thử giày, bảng so sánh và FAQ |
| Vị trí từ khóa | Trong title, H1, đoạn mở đầu, một số tiêu đề và nội dung; dùng biến thể tự nhiên, tránh nhồi từ khóa |
| Ảnh | Ảnh raster được tải từ Unsplash; alt mô tả nội dung; ảnh đầu bài có `width`, `height` và `fetchpriority="high"` |
| Liên kết trong tạp chí | Trang chủ có liên kết trực tiếp ở khu vực Bài nổi bật và đầu danh sách Bài viết mới nhất; trang bài viết có breadcrumb/quay về tạp chí |
| Liên kết sang website chính | Chỉ đặt theo ngữ cảnh trong nội dung bài viết và khối gợi ý liên quan, không đặt ở header/menu/footer của tạp chí |
| Liên kết ngoài | Tài liệu tham khảo REI Expert Advice có liên quan đến nội dung |
| Canonical | Chưa khai báo absolute canonical vì URL riêng của Tạp chí thể thao 24h chưa được cung cấp. Sau khi xuất bản, canonical phải trỏ về đúng URL bài trên website tạp chí — không trỏ sang website cửa hàng. |
| Social preview | Open Graph + Twitter Card |
| Structured data | JSON-LD `Article`; bổ sung URL xuất bản chính thức và breadcrumb schema sau khi biết URL GitHub Pages riêng |
| Mobile | Có `meta viewport` và CSS responsive |
| Ngôn ngữ | `lang="vi"`, UTF-8, doctype HTML5 |
| Meta keywords | Có để minh họa kỹ thuật; Google không dùng thẻ `meta keywords` làm tín hiệu xếp hạng. Không nhồi từ khóa vào nội dung. |

## 2. Cách kiểm tra bằng SEOquake

1. Tạo repository GitHub riêng cho Tạp chí thể thao 24h và tải **toàn bộ file trong ZIP** lên cùng thư mục xuất bản, không chỉ tải `index.html`.
2. Bật GitHub Pages trong **Settings → Pages**.
3. Mở trang chủ đã xuất bản; kiểm tra thẻ Bài nổi bật. Bấm **Đọc bài chuyên sâu** để xác nhận bài HTML mở bình thường.
4. Mở URL công khai của bài viết trong Chrome. SEOquake không thể xác nhận đầy đủ tình trạng indexability chỉ từ file HTML `file://`.
5. Mở SEOquake → Quick View và Full Report / On-Page SEO Audit (tên mục có thể khác theo phiên bản). Lưu ảnh chụp báo cáo làm bằng chứng.
6. Kiểm tra thủ công các tiêu chí: title, description, H1/H2/H3, ảnh ALT, liên kết, canonical, mobile viewport, mã trạng thái HTTP và URL xuất bản.
7. Sau khi chốt URL, thêm canonical absolute, cập nhật `og:url`, `mainEntityOfPage`, breadcrumb JSON-LD và tạo `sitemap.xml` với URL tuyệt đối đúng. Không điền URL phỏng đoán.

### Bảng kiểm trước khi nộp

| Nhóm | Kỳ vọng | Trạng thái hiện tại |
|---|---|---|
| Title | Rõ chủ đề và khác biệt với trang chủ | Đã cài trong HTML; cần audit trên URL live |
| Meta description | Duy nhất, tóm tắt nội dung | Đã cài; cần xem cách SEOquake đếm ký tự Unicode |
| Headings | Một H1 rõ ràng; H2/H3 phân cấp hợp lý | Đã cài |
| Image ALT | Ảnh có alt phù hợp | Đã cài; cần xem cảnh báo sau deploy |
| Liên kết đến bài | Trang chủ liên kết trực tiếp tới bài SEO | Đã cài ở Bài nổi bật và Bài viết mới nhất |
| Link sang trang chính | Nằm trong ngữ cảnh bài viết, không nằm ở menu tạp chí | Đã cài trong bài mẫu; cần kiểm tra đích đến khi deploy |
| Canonical / robots | Canonical chính xác, robots cho phép crawl | Robots `index,follow` đã cài; canonical chờ URL riêng chính thức |
| Mobile viewport | Có viewport và layout responsive | Đã cài |
| Ngôn ngữ / encoding | `lang="vi"`, UTF-8, HTML5 | Đã cài |
| URL và nội dung | Slug dễ đọc, nội dung đáp ứng ý định tìm kiếm | Đã cài; cần chạy SEOquake trên URL live |
| Sitemap / robots.txt | Khai báo theo domain/repository thật | Chờ URL xuất bản chính thức để tạo chính xác |
| Structured data | JSON-LD hợp lệ, không dùng URL sai | `Article` đã cài; kiểm tra và bổ sung URL sau deploy |

**Lưu ý:** Đây là checklist chuẩn bị kiểm tra, không phải điểm audit SEOquake thật. Mình chưa xác nhận điểm số hay trạng thái index của URL công khai. Điểm SEOquake cũng không bảo đảm thứ hạng Google.

## 3. Checklist biên tập

- [ ] Đọc lại toàn bài và kiểm chứng các khuyến nghị trước khi dùng làm bài xuất bản lâu dài.
- [ ] Kiểm tra ảnh tải được và quyền sử dụng; ảnh hiện được hotlink từ Unsplash nên cần Internet.
- [ ] Khi URL tạp chí đã hoạt động, cập nhật canonical và URL trong OG/JSON-LD.
- [ ] Mở tất cả liên kết; xác nhận điều hướng nội bộ tạp chí không dẫn sang cửa hàng ngoài ý muốn.
- [ ] Chạy SEOquake trên URL live, lưu báo cáo thực tế và kiểm tra JSON-LD bằng validator phù hợp.
- [ ] Tạo `sitemap.xml` từ các URL tuyệt đối đã xuất bản; không dùng URL giả định.

## 4. Nguồn hướng dẫn

- SEOquake — Page SEO Audit: https://www.seoquake.com/guide/basic/diagnosis.html
- SEOquake — Terms & definitions: https://www.seoquake.com/guide/definitions.html
- Google Search Central — SEO Starter Guide: https://developers.google.com/search/docs/fundamentals/seo-starter-guide
- Google Search Central — Title links: https://developers.google.com/search/docs/appearance/title-link
- REI — How Should Running Shoes Fit?: https://www.rei.com/learn/expert-advice/how-should-running-shoes-fit.html
- REI — How to Choose Running Shoes: https://www.rei.com/learn/expert-advice/running-shoes.html
