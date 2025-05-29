# Giải thích chương trình áp dụng các bộ lọc khử nhiễu cho ảnh

## Cách hoạt động của code

- Chương trình sử dụng các thư viện `numpy`, `imageio`, `scipy.ndimage`, `matplotlib`, `glob` và `os`.
- Đầu tiên, chương trình lấy danh sách các file ảnh (đuôi `.jpg`, `.png`) trong thư mục `Exercise`.
- Tạo thư mục mới `Exercise_filtered` để lưu các ảnh sau khi xử lý.
- Với từng ảnh:
  - Đọc ảnh từ file.
  - Nếu ảnh là ảnh màu, áp dụng từng bộ lọc cho từng kênh màu.
  - Nếu ảnh là ảnh xám, áp dụng trực tiếp các bộ lọc.
  - Áp dụng ba bộ lọc khử nhiễu:  
    - **Mean filter** (bộ lọc trung bình)
    - **Median filter** (bộ lọc trung vị)
    - **Gaussian filter** (bộ lọc Gauss)
  - Lưu các ảnh đã lọc vào thư mục `Exercise_filtered` với tên tương ứng.
  - Hiển thị song song ảnh gốc và các ảnh đã lọc để dễ dàng so sánh.

## Kết quả và đánh giá

- **Mean filter**: Làm mịn ảnh, giảm nhiễu nhưng có thể làm mờ các chi tiết nhỏ.
- **Median filter**: Khử nhiễu muối tiêu rất hiệu quả, giữ được biên tốt hơn mean filter.
- **Gaussian filter**: Làm mịn ảnh, giữ chi tiết tốt hơn mean filter trong nhiều trường hợp.
- **Kết luận**:  
  - Nếu ảnh bị nhiễu muối tiêu, **median filter** thường cho kết quả tốt nhất.
  - Nếu ảnh nhiễu đều hoặc nhiễu Gaussian, **gaussian filter** thường giữ chi tiết tốt hơn mean filter.
  - Bạn nên quan sát kết quả hiển thị để chọn bộ lọc phù hợp nhất với từng loại ảnh và loại nhiễu.