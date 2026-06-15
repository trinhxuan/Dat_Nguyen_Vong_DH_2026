# Hệ Thống Tuyển Sinh Toàn Diện 2026 - T-Physics Pro

Dự án HTML tĩnh dùng để chạy trực tiếp trên GitHub Pages.

## Cách chạy trên GitHub Pages

1. Giải nén gói `nguyen-vong-2026-updated-github-ready.zip`.
2. Upload toàn bộ nội dung bên trong thư mục lên repository GitHub.
3. Vào **Settings → Pages**.
4. Chọn **Deploy from a branch**.
5. Chọn branch `main`, folder `/root`, rồi bấm **Save**.
6. Mở đường dẫn dạng `https://ten-tai-khoan.github.io/ten-repository/`.

## File quan trọng

- `index.html`: file chạy chính trên GitHub Pages.
- `nguyen-vong-2026-source-uploaded.html`: bản HTML gốc mới nhất người dùng đã gửi, giữ lại để đối chiếu.
- `.nojekyll`: giúp GitHub Pages phục vụ file tĩnh ổn định.

## Cập nhật dữ liệu

Khi có phổ điểm/đề án/điểm chuẩn mới, mở `index.html` và cập nhật các mảng JavaScript:

- `exactHSAPercentiles`
- `baseTableData`
- `uniDatabase`

## Tính năng đã tích hợp

- Quy đổi HSA theo hai phương pháp: nội suy điểm và nội suy phân vị.
- Tính điểm ưu tiên giảm tuyến tính theo quy chế.
- Tự động sắp xếp 15 nguyện vọng theo độ lệch điểm.
- Xuất CSV.
- In/PDF.
- Lưu cấu hình bằng `localStorage`.
- Reset và tự bù đủ 15 nguyện vọng mẫu.
