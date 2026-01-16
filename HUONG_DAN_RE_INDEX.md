# Hướng dẫn yêu cầu Google re-index website

## Bước 1: Mở Google Search Console
1. Truy cập: https://search.google.com/search-console
2. Đăng nhập bằng tài khoản Google đã kết nối với website của bạn

## Bước 2: Chọn Property
- Trong danh sách properties, chọn: **turkmenistan-victour.com**

## Bước 3: Vào URL Inspection
- Trong menu bên trái, tìm và click vào: **"Kiểm tra URL"** (URL Inspection)
- Hoặc có thể tìm bằng thanh search ở đầu trang

## Bước 4: Nhập URL và Request Indexing
1. Trong ô tìm kiếm URL Inspection, nhập:
   ```
   https://turkmenistan-victour.com/
   ```
   (hoặc `https://www.turkmenistan-victour.com/` nếu bạn dùng www)

2. Nhấn Enter hoặc click vào icon kính lúp

3. Google sẽ kiểm tra URL và hiển thị thông tin

4. Sau khi có kết quả, tìm và click nút **"Yêu cầu lập chỉ mục"** (Request Indexing)
   - Nút này có thể ở trên cùng hoặc dưới phần thông tin

5. Xác nhận yêu cầu (nếu có popup)

## Bước 5: Submit Sitemap (Quan trọng!)

⚠️ **QUAN TRỌNG: Phải deploy website trước khi submit sitemap!**

1. **Đảm bảo đã deploy website** với file `sitemap.xml` mới

2. **Kiểm tra sitemap có hoạt động:**
   - Mở trình duyệt, truy cập: `https://turkmenistan-victour.com/sitemap.xml`
   - Nếu thấy nội dung XML (không phải lỗi 404), thì sitemap đã sẵn sàng

3. **Trong Google Search Console:**
   - Menu bên trái → **"Sơ đồ trang web"** (Sitemaps)

4. **Submit sitemap:**
   - Trong phần "Thêm sơ đồ trang web mới", nhập:
     ```
     sitemap.xml
     ```
     HOẶC thử với full URL:
     ```
     https://turkmenistan-victour.com/sitemap.xml
     ```

5. Click nút **"Gửi"** (Submit)

6. Đợi vài phút, refresh trang để xem status:
   - ✅ "Thành công" (Success) = OK
   - ❌ "Không thể tìm nạp" = cần kiểm tra lại URL hoặc deploy

## Lưu ý:
- ⏰ Google có thể mất vài giờ đến vài ngày để cập nhật
- ✅ Bạn có thể request indexing nhiều lần nhưng không nên spam (1-2 lần/tuần là đủ)
- 🔄 Sau khi deploy code mới, nên request indexing lại
- 📦 **Phải deploy website trước** - Google không thể truy cập sitemap nếu file chưa được deploy
- 🔍 Test sitemap trước: Mở `https://turkmenistan-victour.com/sitemap.xml` trong trình duyệt

## Kiểm tra kết quả:
1. Vào lại URL Inspection sau vài giờ
2. Kiểm tra trạng thái "Indexing requested" hoặc "Indexed"
3. Test bằng cách search: `site:turkmenistan-victour.com` trên Google

---

**Sau khi hoàn thành các bước trên, Google sẽ cập nhật preview ảnh và thông tin mới của website!**
