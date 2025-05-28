# Giải thích chương trình tách kênh màu HSV của ảnh

## Cách hoạt động của code

- Chương trình sử dụng các thư viện `numpy`, `imageio`, `matplotlib` và `matplotlib.colors`.
- Đầu tiên, chương trình nạp một ảnh màu (ví dụ: `bird.png`) và chuẩn hóa giá trị pixel về [0, 1].
- Ảnh được chuyển từ hệ màu RGB sang hệ màu HSV.
- Chương trình tạo ra 3 ảnh mới, mỗi ảnh chỉ giữ lại một kênh trong không gian màu HSV:
  - Ảnh 1: Chỉ giữ kênh Hue (màu sắc), các kênh còn lại đặt giá trị tối đa.
  - Ảnh 2: Chỉ giữ kênh Saturation (độ bão hòa), các kênh còn lại đặt giá trị phù hợp.
  - Ảnh 3: Chỉ giữ kênh Value (độ sáng), các kênh còn lại đặt giá trị phù hợp.
- Các ảnh này được chuyển ngược lại sang hệ màu RGB và lưu với tên: `hue.png`, `saturation.png`, `value.png`.
- Cuối cùng, chương trình hiển thị 3 ảnh này trên cùng một cửa sổ để người dùng dễ dàng so sánh.

## Kết quả

- Ảnh `hue.png`: thể hiện thông tin về màu sắc gốc của ảnh, không phụ thuộc vào độ sáng hay độ bão hòa.
- Ảnh `saturation.png`: thể hiện mức độ bão hòa màu của từng điểm ảnh.
- Ảnh `value.png`: thể hiện độ sáng của từng điểm ảnh trong ảnh gốc.
- Việc hiển thị giúp quan sát rõ vai trò của từng kênh HSV trong việc tạo nên màu sắc tổng thể của ảnh.