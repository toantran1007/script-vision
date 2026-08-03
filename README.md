# ScriptVision

Chuyển kịch bản văn bản thành video hoàn chỉnh bằng AI: phân tích kịch bản → chia
đoạn phụ đề → tạo ảnh tham chiếu nhân vật → tạo ảnh từng cảnh → đọc giọng → ghép video.

**Repo này là kênh phát hành.** Mã nguồn không nằm ở đây — vào tab
[Releases](../../releases) để tải bản cài.

## Cài đặt

1. Tải `ScriptVision-<phiên-bản>-setup.exe` ở [Releases](../../releases/latest).
2. Chạy file cài. Chọn được thư mục cài đặt.

Windows có thể hiện cảnh báo SmartScreen vì bản cài chưa mua chứng thư ký số —
chọn **More info → Run anyway**.

## Yêu cầu

| Thứ | Mức |
|-----|-----|
| Hệ điều hành | Windows 10/11 64-bit |
| Ổ đĩa | ~15 GB (bản cài 93 MB + runtime giọng đọc tải lần đầu) |
| GPU | NVIDIA (bắt buộc cho giọng đọc) |
| Mạng | Cần cho lần chạy đầu và cho việc tạo ảnh |

**Lần chạy đầu** app tải runtime giọng đọc (~11 GB) và ffmpeg (~195 MB). Chỉ một
lần, sau đó chạy được không cần mạng cho phần giọng đọc.

Phần tạo ảnh và phân tích kịch bản gọi API bên ngoài, cần tự điền khoá của mình
trong **Settings**. Khoá lưu tại `%APPDATA%\ScriptVision\config.json` trên máy bạn,
không gửi đi đâu khác.

## Cập nhật

Mở **Settings → Cập nhật → 🔄 Kiểm tra**. Có bản mới thì bấm **⬇️ Tải về** rồi
**🚀 Cài & khởi động lại**.

Từ lần cập nhật thứ hai trở đi app chỉ tải phần thay đổi, không tải lại trọn bản
cài.

## Dữ liệu của bạn

Toàn bộ project, ảnh, giọng đọc và video nằm ở `%APPDATA%\ScriptVision\`. Gỡ app
không xoá thư mục này.
