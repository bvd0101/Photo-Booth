# Photo-Booth

Ứng dụng chụp ảnh trên trình duyệt của Bui Van Diep (Rapptor).

[Demo](https://photobooth.diep-robotech.cloud)

## Tính năng

- Chụp bằng webcam với lựa chọn khung ảnh và bộ lọc.
- Ghép ảnh thành dải ảnh; tải kết quả PNG trực tiếp.
- Đếm ngược thủ công hoặc chu kỳ tự động 5, 7, 10 giây.
- Tùy chọn hiệu ứng làm đẹp và nhạc nền.
- Khi cấu hình máy chủ phù hợp, tải ảnh lên để tạo mã QR cho liên kết tải.

## Chạy bản sao của bạn

1. Tải repo, giữ cấu trúc `index.html`, `assets/`, `music/` và `sounds/`.
2. Kiểm tra quyền sử dụng các tài nguyên theo `MEDIA_RIGHTS.md`; thay tài nguyên chưa được phép bằng tài nguyên của bạn.
3. Chạy qua HTTPS hoặc máy chủ localhost để trình duyệt có thể xin quyền camera.
4. Trình duyệt cần kết nối mạng để tải QRCode.js, Font Awesome và Google Fonts.

Ứng dụng dùng HTML, CSS và JavaScript trong `index.html`; không cần bước biên dịch.

## Máy chủ tải ảnh và quyền riêng tư

Mã hiện tại có hằng `GOOGLE_SCRIPT_URL` trỏ tới dịch vụ của bản demo. Trước khi vận hành bản sao của bạn, thay bằng máy chủ bạn kiểm soát hoặc tắt chức năng tải ảnh lên.

Khi nhấn **XEM KẾT QUẢ**, phiên bản hiện tại tự gửi ảnh PNG đã ghép tới địa chỉ trong `GOOGLE_SCRIPT_URL`. Đây không phải ứng dụng chỉ xử lý ảnh cục bộ.

Repo này không có mã máy chủ Cloudflare Worker / Google Apps Script dùng để tải ảnh, lưu Drive hoặc xóa ảnh. Dòng giao diện nói liên kết tự hủy sau 5 phút chưa được xác minh từ mã máy chủ trong repo. Người triển khai cần tự cung cấp máy chủ và chính sách lưu/xóa dữ liệu; giấy phép mã nguồn không cấp quyền dùng dịch vụ demo của tác giả.

## Đóng góp và báo lỗi

Khi mở issue, ghi trình duyệt, hệ điều hành, kích thước màn hình, bước tái hiện và kết quả mong muốn. Không đính kèm ảnh cá nhân hoặc dữ liệu nhạy cảm nếu chưa muốn công khai.

Các hướng đóng góp hữu ích gồm tương thích camera, giao diện di động, khả năng tiếp cận, xử lý lỗi tải ảnh và tài liệu triển khai máy chủ.

## Giấy phép

Giấy phép MIT trong [LICENSE](LICENSE) chỉ áp dụng cho mã HTML, CSS, JavaScript và tài liệu gốc do Bui Van Diep viết. Phần mã này được phép sử dụng, sửa đổi và phân phối, kể cả thương mại, với điều kiện giữ thông báo bản quyền và giấy phép.

MIT này không áp dụng cho `music/`, `sounds/`, `assets/` hoặc `bank-qr.jpg`. Các tài nguyên đó được quản lý riêng trong [MEDIA_RIGHTS.md](MEDIA_RIGHTS.md). Thành phần của bên thứ ba giữ giấy phép và thông báo của bên cung cấp.

### Ủng hộ tác giả (Donate)
Nếu bạn thấy mã nguồn này hữu ích và muốn mời tôi một ly cà phê, có thể chuyển khoản qua thông tin dưới đây:

* **Ngân hàng:** <u>[Techcombank]</u>
* **Số tài khoản:** <u>[9868633333]</u>
* **Chủ tài khoản:** <u>[BUI VAN DIEP]</u>

