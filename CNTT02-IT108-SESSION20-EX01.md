
# Bài 1 : Xử lý cảnh báo đăng nhập giả mạo GitHub
ký tự lạ trong ULR trong đường dẫn nằm ở chữ ú có dấu vì chữ thường như tên miền chính thống chữ u sẽ không có dấu
**tại sao nó đánh lừa người dùng**
đây là một kỹ thuật tấn công gọi là tấn công giả mạo ký tự chúng chọn các ký tự có hình dáng gần như không thể phân biệt bằng mắt thường so với các chữ lating gốc khi nhìn lướt qua dưới áp lực của một `cảnh báo bảo mật khẩn cấp` chúng sẽ bị rất dễ tự động bỏ qua các dấu nhỏ nhầm tưởng đây là trang `github` thật
**2 quy trình kiểm tra url nhanh trước khi đăng nhập master password**
**BƯỚC 1** quan sát kĩ bằng mắt thường 
- [x] tập trung nhìn vào tên miền chính ngay trước dấu chéo đầu tiên /
- [x] cảnh báo cao độ với thông báo `security alert` yêu cầu đăng nhập lại gấp vì các dịch vụ lớn thông thường không ép bạn đăng nhập lại mật khẩu qua liên kết lạ 
**BƯỚC 2** dựa vào trình quản lí mật khẩu `password manager
- [x] các phần mềm quản lý mật khẩu uy tính như ` bitwarden` 
- [x] nếu bạn vào trang web giả mạo quản lý mật khẩu sẽ không tự điền mật khẩu 
- [x] **Bước 3** Kiểm tra mã Punycode của trình duyệt
- [x] ác trình duyệt hiện đại thường tự động chuyển đổi các tên miền Unicode khả nghi sang mã máy chủ (dạng xn--...). Nếu bạn bôi đen, copy và dán URL đó vào thanh ghi chú hoặc thấy trình duyệt hiển thị dạng xn--..., đó chắc chắn là tên miền giả mạo dùng ký tự Unicode.
**Bước 4** Chủ động truy cập an toàn
- [x] Không bao giờ click trực tiếp vào đường link bên trong thông báo đáng ngờ
- [x] Hãy tự mở một tab trình duyệt mới, gõ thủ công địa chỉ [https://github.com](https://github.com) hoặc sử dụng Bookmark (Dấu trang) đã lưu sẵn từ trước để vào kiểm tra tài khoản một cách an toàn nhất.