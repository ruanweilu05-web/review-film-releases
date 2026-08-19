# review film — bản phát hành

Kho này chỉ chứa **file chạy** của app và một file `manifest.json` để app tự
tìm bản mới. Mã nguồn nằm ở kho riêng.

## Vì sao chỉ có file chạy

Cả gói app nặng 6,4 GB, nhưng phần mã chỉ là `ReviewFilm.exe` khoảng 200 MB —
3,1%. Phần còn lại (hai bộ PaddleOCR, model giọng đọc, Chromium, ffmpeg) gần
như không bao giờ đổi giữa các bản, nên không việc gì bắt tải lại từ đầu.

## Cách cập nhật

Mở app, bấm nút **⬆ Cập nhật** ở thanh trên. App hỏi `manifest.json`, so số
hiệu bản, tải file chạy mới nếu có, kiểm vân tay SHA-256 rồi mới thay. Vân tay
sai thì bỏ file tải về và giữ nguyên bản đang chạy.

## Nguồn

App được xây trên nền một dự án mã nguồn mở, phần hoàn thiện và các tính năng
riêng do Lộc Nguyễn phát triển.
