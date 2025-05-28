# Giải thích chương trình hoán đổi kênh màu ảnh

## Cách hoạt động của code

- Chương trình sử dụng các thư viện `numpy`, `imageio` và `matplotlib`.
- Đầu tiên, chương trình nạp một ảnh màu (ví dụ: `bird.png`).
- Sau đó, chương trình tạo ra 3 ảnh mới bằng cách hoán đổi vị trí các kênh màu RGB:
  - Ảnh 1: Hoán đổi kênh Đỏ và Xanh dương (`Red <-> Blue`).
  - Ảnh 2: Hoán đổi kênh Đỏ và Xanh lá (`Red <-> Green`).
  - Ảnh 3: Hoán đổi kênh Xanh lá và Xanh dương (`Green <-> Blue`).
- Các ảnh kết quả được lưu lại với tên: `swap_rb.png`, `swap_rg.png`, `swap_gb.png`.
- Cuối cùng, chương trình hiển thị 3 ảnh này trên cùng một cửa sổ để người dùng dễ dàng so sánh.

## Kết quả

- Ảnh `swap_rb.png`: màu sắc của ảnh bị thay đổi do kênh Đỏ và Xanh dương đã bị hoán đổi.
- Ảnh `swap_rg.png`: màu sắc của ảnh bị thay đổi do kênh Đỏ và Xanh lá đã bị hoán đổi.
- Ảnh `swap_gb.png`: màu sắc của ảnh bị thay đổi do kênh Xanh lá và Xanh dương đã bị hoán đổi.
- Việc hiển thị giúp quan sát rõ sự thay đổi màu sắc khi các kênh màu bị hoán đổi trong ảnh gốc.