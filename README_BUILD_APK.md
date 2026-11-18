# Tử Vi Lạc Hồng 1.2 – Android APK

## Tính năng bản 1.2
- Cân Xương Tính Số dùng đủ bốn bảng: 60 hoa giáp, 12 tháng, 30 ngày, 12 giờ; đối chiếu 51 mức từ 2 lượng 1 chỉ đến 7 lượng 1 chỉ.
- Trợ lý luận giải nội bộ chạy bằng bộ quy tắc/tri thức tích hợp, không gọi Gemini/OpenAI và không cần API Key.
- Luận giải cung có xét vị trí thực tế của sao, trạng thái sáng/tối, sao đồng cung, tam hợp và xung chiếu.
- Bảng độ sáng 14 chính tinh được cập nhật theo bộ quy tắc Tân Biên được chọn; hiệu chỉnh Lưu Hà, Thiên Trù và bổ sung Lưu Niên Văn Tinh.
- Hiển thị toàn bộ danh sách phụ tinh trong từng cung; ô lá số và bản JPG/PDF tự điều chỉnh để hạn chế cắt khuất sao.
- Xuất lá số thành JPG chất lượng cao hoặc PDF khổ ngang A4.
- Tự lưu tối đa 50 lá số gần nhất (thông tin sinh và ảnh chụp dữ liệu lá số) trong lịch sử cục bộ; chạm “Mở lá số” để khôi phục hồ sơ đã lưu.
- Mở khóa thủ công: người dùng gửi mã yêu cầu qua Zalo 034.559.3246; tin nhắn được sao chép trước, người dùng dán và bấm gửi.
- Icon ứng dụng phong cách Thiên Cung vàng trên nền thiên hà.

> Lưu ý: đây là bộ máy luận giải chuyên biệt theo quy tắc được đóng gói sẵn, không phải mô hình ngôn ngữ tổng quát như ChatGPT chạy cục bộ. Các thư viện giao diện/font hiện vẫn được tham chiếu từ CDN; muốn ứng dụng hiển thị đầy đủ khi hoàn toàn không có Internet cần đóng gói các thư viện đó vào assets ở một bước riêng.

## Build APK bằng GitHub Actions
1. Tải toàn bộ dự án lên một repository GitHub.
2. Mở tab **Actions** và chạy workflow **Build Android APK** (hoặc push lên nhánh `main`).
3. Tải artifact **TuViLacHong-ThienCung-APK**; bên trong có `app-debug.apk`.

## Build bằng Android Studio
Mở thư mục dự án trong Android Studio, chờ Gradle sync, chọn **Build > Build Bundle(s) / APK(s) > Build APK(s)**. Dự án dùng Gradle 8.4 trong workflow GitHub Actions.

## Quy trình mở khóa thủ công (tạm thời)
- Thanh toán tự động qua ngân hàng hiện đang tạm hoãn; app vẫn hiển thị thông tin QR/tài khoản ngân hàng hiện có.
- Người dùng bấm **Tôi đã chuyển khoản – nhận mã mở khóa** để lấy mã yêu cầu, sau đó nhấn **Gửi yêu cầu qua Zalo 034.559.3246**.
- Ứng dụng sao chép nội dung yêu cầu và mở liên hệ Zalo; người dùng cần dán nội dung vào cuộc trò chuyện và tự nhấn Gửi. Ứng dụng không tự gửi tin nhắn Zalo nền.
- Quản trị viên mở `ADMIN_CAP_MA_KICH_HOAT.html`, nhập mã yêu cầu, chọn đúng gói và mã cung (nếu mua lẻ), tạo mã rồi gửi lại người dùng.
- Người dùng nhập mã vào app để mở khóa. Quyền mở khóa được lưu trên thiết bị bằng localStorage.
- Đây là cơ chế cấp mã offline tạm thời; khóa xác thực được đóng gói trong APK nên không có độ bảo mật như xác minh phía máy chủ. Không dùng làm cơ chế chống sao chép/chống gian lận lâu dài.

- Android 10 trở lên: JPG/PDF được lưu vào `Download/TuViLacHong/`. Android 6–9: lưu trong thư mục Download riêng của ứng dụng.
