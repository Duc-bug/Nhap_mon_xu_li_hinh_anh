# Giải thích chương trình áp dụng mean filter cho các ảnh trong thư mục

## Cách hoạt động của code

- Chương trình sử dụng các thư viện `numpy`, `imageio`, `scipy.ndimage`, `matplotlib`, `glob` và `os`.
- Đầu tiên, chương trình lấy danh sách các file ảnh (đuôi `.jpg`, `.png`) trong thư mục `exercise`.
- Tạo thư mục mới `exercise_mean` để lưu các ảnh sau khi xử lý.
- Với từng ảnh (tối đa 3 ảnh đầu tiên):
  - Đọc ảnh từ file.
  - Nếu ảnh là ảnh màu, áp dụng mean filter (bộ lọc trung bình) riêng cho từng kênh màu.
  - Nếu ảnh là ảnh xám, áp dụng mean filter trực tiếp.
  - Lưu ảnh đã lọc vào thư mục `exercise_mean`.
  - Hiển thị song song ảnh gốc và ảnh đã lọc để dễ dàng so sánh.

## Kết quả

- Các ảnh sau khi áp dụng mean filter sẽ mịn hơn, giảm nhiễu và chi tiết nhỏ.
- Ảnh kết quả được lưu trong thư mục `exercise_mean` với tên giống ảnh gốc.
- Việc hiển thị song song giúp quan sát rõ tác dụng của mean filter lên từng ảnh.