# Giải thích chương trình chỉnh sửa kênh màu HSV của ảnh

## Cách hoạt động của code

- Chương trình sử dụng các thư viện `numpy`, `imageio`, `matplotlib` và `matplotlib.colors`.
- Đầu tiên, chương trình nạp một ảnh màu (ví dụ: `bird.png`) và chuẩn hóa giá trị pixel về [0, 1].
- Ảnh được chuyển từ hệ màu RGB sang hệ màu HSV.
- Chương trình thực hiện thay đổi trên hai kênh:
  - Kênh Hue (H): giảm còn 1/3 giá trị gốc (`Hnew = 1/3 * Hold`), làm thay đổi tông màu tổng thể.
  - Kênh Value (V): giảm còn 3/4 giá trị gốc (`Vnew = 3/4 * Vold`), làm ảnh tối hơn.
- Ảnh HSV sau khi chỉnh sửa được chuyển ngược lại sang hệ màu RGB và lưu với tên `hsv_modified.png`.
- Cuối cùng, chương trình hiển thị đồng thời ảnh gốc và ảnh đã chỉnh sửa để người dùng dễ dàng so sánh.

## Kết quả

- Ảnh `hsv_modified.png`: màu sắc tổng thể của ảnh bị thay đổi do kênh Hue bị giảm, đồng thời ảnh cũng tối hơn do kênh Value bị giảm.
- Việc hiển thị song song giúp quan sát rõ tác động của việc chỉnh sửa các kênh HSV lên ảnh gốc.