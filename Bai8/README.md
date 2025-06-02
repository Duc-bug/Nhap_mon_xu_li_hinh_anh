### Cách hoạt động của code

- Chương trình sử dụng các thư viện `numpy`, `imageio`, `scipy.ndimage`, `matplotlib`, `glob` và `os`.
- Đầu tiên, chương trình lấy danh sách các file ảnh (đuôi `.jpg`, `.png`) trong thư mục `Exercise`.
- Tạo thư mục mới `Exercise_randomcolor` để lưu các ảnh kết quả.
- Với từng ảnh:
  - Đọc ảnh từ file.
  - Khử nhiễu bằng median filter cho từng kênh nếu là ảnh màu, hoặc chuyển ảnh xám thành ảnh màu.
  - Sinh một hoán vị ngẫu nhiên của các kênh RGB và áp dụng hoán vị này để đổi màu ảnh.
  - Lưu ảnh đã đổi màu vào thư mục `Exercise_randomcolor`.
  - Hiển thị song song ảnh gốc và ảnh đã đổi màu để dễ dàng so sánh.
  - Kết quả:Ảnh sẽ được chuyển đổi ngẫu nhiên


---