# Tử Vi Lạc Hồng 1.2 – Hạng mục hoàn thiện

## An sao và đối chiếu
- Bảng độ sáng 14 chính tinh đã cập nhật theo hệ thống Tân Biên được chọn. Các ký hiệu M/V/Đ/B/H tương ứng Miếu/Vượng/Đắc/Bình/Hãm theo dữ liệu nguồn. Từ điển giải nghĩa phụ tinh được bổ sung đủ 88 nhãn phụ tinh đang được bộ máy an sao sử dụng (gồm sao gốc và sao lưu).
- Lưu Hà: dùng bảng theo Can năm trong XemTuong.net/Tử Vi Đẩu Số Tân Biên; Đinh an Thìn, Canh an Thân.
- Thiên Trù: sửa Can Quý về Tuất.
- Bổ sung Lưu Niên Văn Tinh theo Can năm.
- Không khẳng định mọi trang Tử Vi phải cho kết quả giống nhau: các trường phái có thể dùng bảng an sao khác nhau. App cần ghi rõ hệ quy tắc đang dùng và cho phép đối chiếu.

## Hiển thị phụ tinh
Trước đây ô cung có chiều cao giới hạn và cắt khuất phần phụ tinh cuối danh sách. Bản 1.2 cho ô tự tăng chiều cao theo số sao, bỏ cắt chữ tên sao và xuất cả danh sách lên JPG/PDF.

## Lưu lá số
- Mỗi lần người dùng lập lá số bằng biểu mẫu hoặc tạo lá số ngẫu nhiên, hồ sơ đầu vào cùng ảnh chụp dữ liệu lá số đã tính được lưu vào localStorage của WebView.
- Lưu tối đa 50 hồ sơ gần nhất; có thể mở lại đúng dữ liệu đã lưu hoặc xóa từng hồ sơ/xóa toàn bộ.
- Lịch sử được lưu trên thiết bị hiện tại; xóa dữ liệu ứng dụng hoặc gỡ app có thể làm mất lịch sử. Chưa có đồng bộ tài khoản/cloud.

## Xuất tệp
- JPG được dựng trên canvas độ phân giải 2800 × 2100.
- PDF là một trang A4 ngang, nhúng ảnh JPG của lá số.
- Android 10 trở lên lưu vào `Download/TuViLacHong/`.
- Android 6–9 lưu vào thư mục Downloads riêng của ứng dụng (`Android/data/.../files/Download/TuViLacHong`).
- Nếu chạy ngoài APK, trình duyệt sử dụng thao tác tải tệp thông thường.

## Gửi yêu cầu kích hoạt qua Zalo
- Liên hệ: 034.559.3246.
- Mã yêu cầu, gói mua, mã cung và số tiền được đặt trong nội dung tin nhắn đã sao chép.
- Ứng dụng mở trang liên hệ Zalo; người dùng phải dán và bấm gửi vì app không có quyền gửi tin nhắn Zalo tự động.
- Thanh toán tự động qua ngân hàng vẫn tạm hoãn; chủ ứng dụng cần tự xác minh chuyển khoản trước khi tạo mã bằng `ADMIN_CAP_MA_KICH_HOAT.html`.

## Giới hạn và lưu ý
- Bảng an sao được chọn tương thích quy tắc Tân Biên tham chiếu XemTuong.net; điều này không bảo đảm trùng với mọi trang dùng trường phái khác.
- Một số hạn lưu/tháng lưu chưa được tính đầy đủ. App không tự tạo kết luận về lưu nguyệt nếu thiếu dữ liệu.
- Tử Vi là nội dung tham khảo truyền thống, không phải dự báo khoa học hay thay thế tư vấn chuyên môn.
- Mở khóa offline đang dùng khóa tích hợp trong APK; không chống sao chép ở mức máy chủ.
