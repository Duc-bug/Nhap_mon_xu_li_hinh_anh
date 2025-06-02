### Cách hoạt động của code

- Chương trình sử dụng các thư viện `numpy`, `imageio`, `scipy.ndimage`, `matplotlib.colors`, `matplotlib`, `glob` và `os`.
- Đầu tiên, chương trình lấy danh sách các file ảnh (đuôi `.jpg`, `.png`) trong thư mục `Exercise`.
- Tạo thư mục mới `Exercise_randomhsv` để lưu các ảnh kết quả.
- Với từng ảnh:
  - Đọc ảnh từ file.
  - Khử nhiễu bằng median filter cho từng kênh nếu là ảnh màu, hoặc chuyển ảnh xám thành ảnh màu.
  - Chuyển ảnh sang hệ màu HSV.
  - Sinh một hoán vị ngẫu nhiên (không trùng với thứ tự gốc) của các kênh HSV và áp dụng hoán vị này.
  - Chuyển ảnh trở lại hệ màu RGB.
  - Lưu ảnh đã đổi màu vào thư mục `Exercise_randomhsv`.
  - Hiển thị song song ảnh gốc và ảnh đã đổi màu HSV để dễ dàng so sánh.



