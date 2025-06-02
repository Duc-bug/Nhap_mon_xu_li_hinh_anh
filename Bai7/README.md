# Giải thích chương trình xác định biên ảnh với các bộ lọc

## Cách hoạt động của code

- Chương trình sử dụng các thư viện `numpy`, `imageio`, `scipy.ndimage`, `matplotlib`, `glob` và `os`.
- Đầu tiên, chương trình lấy danh sách các file ảnh (đuôi `.jpg`, `.png`) trong thư mục `Exercise`.
- Tạo thư mục mới `Exercise_edges` để lưu các ảnh kết quả.
- Với từng ảnh:
  - Đọc ảnh từ file.
  - Nếu ảnh là ảnh màu, chuyển sang ảnh xám.
  - Khử nhiễu ảnh bằng bộ lọc median (median filter).
  - Áp dụng các bộ lọc xác định biên:
    - **Sobel**: phát hiện biên theo hướng ngang và dọc, sau đó tổng hợp lại.
    - **Prewitt**: tương tự Sobel nhưng dùng mặt nạ khác.
    - **Laplace**: phát hiện biên dựa trên đạo hàm bậc hai.
  - Lưu các ảnh biên vào thư mục `Exercise_edges` với tên tương ứng.
  - Hiển thị song song ảnh gốc (xám) và các ảnh biên để dễ dàng so sánh.

