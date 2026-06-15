# Hệ thống tuyển sinh toàn diện 2026

Dự án web tĩnh dùng cho GitHub Pages để mô phỏng quy đổi điểm HSA - THPT và sắp xếp chiến thuật 15 nguyện vọng.

## Cấu trúc

- `index.html`: toàn bộ giao diện, dữ liệu và logic JavaScript.
- `.nojekyll`: giúp GitHub Pages phục vụ file tĩnh trực tiếp.

## Cách đưa lên GitHub Pages

1. Tạo repository mới trên GitHub, ví dụ: `nguyen-vong-2026`.
2. Giải nén gói này và upload toàn bộ file trong thư mục lên repository.
3. Vào **Settings → Pages**.
4. Chọn **Deploy from a branch**.
5. Chọn branch `main`, folder `/root`, rồi bấm **Save**.
6. Chờ GitHub Pages build xong, mở link dạng `https://ten-tai-khoan.github.io/nguyen-vong-2026/`.

## Cập nhật dữ liệu

Mở `index.html`, tìm các mảng sau:

- `baseTableData`: bảng quy đổi bách phân vị HSA → THPT.
- `exactHSAPercentiles`: bách phân vị HSA chi tiết.
- `uniDatabase`: cơ sở dữ liệu trường/ngành/điểm chuẩn.

Sau khi sửa, commit lại lên GitHub. Trang GitHub Pages sẽ tự cập nhật sau vài phút.

## Chức năng đã hoàn thiện

- Chạy trực tiếp trên GitHub Pages không cần backend.
- Tự điền đủ 15 nguyện vọng mẫu.
- Tính điểm ưu tiên theo công thức giảm tuyến tính khi điểm gốc từ 22,5 trở lên.
- Mô phỏng phổ điểm THPT bằng thanh trượt độ lệch.
- Phân loại nguyện vọng: Mơ ước, Vừa đủ, An toàn, Bỏ qua.
- Lưu cấu hình trên trình duyệt bằng `localStorage`.
- Xuất danh sách nguyện vọng ra CSV.
- In hoặc lưu PDF bằng chức năng in của trình duyệt.

## Lưu ý

Dữ liệu trong file là dữ liệu tham khảo để mô phỏng chiến thuật. Khi có phổ điểm hoặc đề án tuyển sinh 2026 chính thức, cần cập nhật lại dữ liệu trước khi sử dụng để tư vấn quyết định thật.
