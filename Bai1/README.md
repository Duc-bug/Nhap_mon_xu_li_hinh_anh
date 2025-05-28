# Giải thích chương trình tách kênh màu ảnh

## Cách hoạt động của code

- Chương trình sử dụng thư viện `numpy`, `imageio` và `matplotlib`.
- Đầu tiên, chương trình nạp một ảnh màu (ví dụ: `bird.png`).
- Sau đó, chương trình tạo ra 3 ảnh mới, mỗi ảnh chỉ giữ lại một kênh màu (đỏ, xanh lá, xanh dương) và đặt giá trị các kênh còn lại bằng 0.
- Các ảnh này được lưu lại với tên lần lượt là: `bird_red.png`, `bird_green.png`, `bird_blue.png`.
- Cuối cùng, chương trình hiển thị 3 ảnh này trên cùng một cửa sổ để người dùng dễ dàng so sánh.

## Kết quả

- Ảnh `bird_red.png`: chỉ hiển thị thành phần màu đỏ của ảnh gốc, các màu khác bị loại bỏ.
- Ảnh `bird_green.png`: chỉ hiển thị thành phần màu xanh lá cây của ảnh gốc.
- Ảnh `bird_blue.png`: chỉ hiển thị thành phần màu xanh dương của ảnh gốc.
- Việc hiển thị giúp quan sát rõ sự đóng góp của từng kênh màu trong ảnh gốc.