# Mô tả 
 - Nắm vững các khái niệm cơ bản về kiểm thử API.
 - Rèn luyện kỹ năng sử dụng Postman để thực hiện các thao tác kiểm thử API.
 - Đánh giá hiệu suất và khả năng mở rộng của API
# Phương thức GET
-  Hình ảnh
 ![Screenshot 2024-05-30 224610](https://github.com/21011132-NguyenThiHongHanh/github-repo/assets/124747121/b7b93676-54f8-4015-97cb-6f7402afb1fb)

- Mô tả chi tiết
   + Mã trạng thái phản hồi: 200 (thành công)
   + Thời gian phản hồi trung bình : 417ms
   + Kích thước phản hồi : 1.6KB
- Hình ảnh
![Uploading Screenshot 2024-05-30 225016.png…]()

- Mô tả chi tiết
    + Số lần lặp lại: 1
    + Khoảng thời gian: 913s
    + Số bài kiểm thử: 3
    + Thời gian chạy trung bình: 360ms
  
  - Kết quả kiểm thử
   *  Lỗi: Successful POST request | AssertionError: expected 200 to be one of [ 201, 202 ]:
       + Mô tả: Yêu cầu POST không thành công như mong đợi. Mã trạng thái của yêu cầu là 200, trong khi mã trạng thái mong đợi là 201 hoặc 202.
       + Ảnh hưởng: Có thể có sự không tương thích với quy trình hoặc luồng làm việc đã thiết lập với mã trạng thái phản hồi.
       + Khuyến nghị: Xác định và sửa lỗi trong quá trình xử lý yêu cầu POST để đảm bảo rằng mã trạng thái phản hồi đáp ứng đúng mong đợi.
   * Đúng: Status code is 200:
       + Mô tả: Mã trạng thái của phản hồi là 200, đúng như mong đợi.
       + Khuyến nghị: Không có vấn đề cụ thể được phát hiện trong quá trình kiểm thử này.
   * Lỗi: Response time is less than 200ms | AssertionError: expected 360 to be below 200:
       + Mô tả: Thời gian phản hồi vượt quá ngưỡng 200ms. Thực tế, thời gian phản hồi là 360ms, không đáp ứng được mong đợi.
       + Ảnh hưởng: Thời gian phản hồi lớn hơn ngưỡng cho phép có thể làm giảm trải nghiệm người dùng và gây ra sự không hài lòng.
       + Khuyến nghị: Kiểm tra và tối ưu hóa hiệu suất hệ thống để giảm thời gian phản hồi.
# Phương thức POST
- Hình ảnh
![Screenshot 2024-05-30 211859](https://github.com/21011132-NguyenThiHongHanh/github-repo/assets/124747121/4a81d77d-6e72-4498-b664-5dced009fde8)

![Screenshot 2024-05-30 211910](https://github.com/21011132-NguyenThiHongHanh/github-repo/assets/124747121/87b416cb-3a9b-4780-a107-f8b3b343baa2)
- Mô tả chi tiết
   + Mã trạng thái phản hồi: 200 (thành công)
   + Thời gian phản hồi trung bình : 560ms
   + Kích thước phản hồi : 800B
  - Hình ảnh
  ![Screenshot 2024-05-30 221749](https://github.com/21011132-NguyenThiHongHanh/github-repo/assets/124747121/1550314e-4ef2-43fc-b3cf-83a82cf1b28a)
- Mô tả chi tiết
    + Số lần lặp lại: 1
    + Khoảng thời gian: 2s624ms
    + Số bài kiểm thử: 3
    + Thời gian chạy trung bình: 2406ms
  - Kết quả kiểm thử
    * Lỗi: Response time is less than 200ms | AssertionError: expected 2406 to be below 200:
        + Mô tả: Thời gian phản hồi cho yêu cầu vượt quá ngưỡng 200ms. Thực tế, thời gian phản hồi là 2406ms, không đáp ứng được mong đợi.
        + Ảnh hưởng: Thời gian phản hồi lớn có thể làm giảm trải nghiệm người dùng và gây ra sự không hài lòng.
        + Khuyến nghị: Kiểm tra và tối ưu hóa hiệu suất hệ thống để giảm thời gian phản hồi.
    * Lỗi: Successful POST request | AssertionError: expected 200 to be one of [ 201, 202 ]:
        + Mô tả: Yêu cầu POST không thành công như mong đợi. Mã trạng thái của yêu cầu là 200, trong khi mã trạng thái mong đợi là 201 hoặc 202.
        + Ảnh hưởng: Có thể có sự không tương thích với quy trình hoặc luồng làm việc đã thiết lập với mã trạng thái phản hồi.
        + Khuyến nghị: Xác định và sửa lỗi trong quá trình xử lý yêu cầu POST để đảm bảo rằng mã trạng thái phản hồi đáp ứng đúng mong đợi.
    * Đúng: Content-Type is present:
        + Mô tả: Tiêu đề Content-Type xuất hiện trong phản hồi, đúng như mong đợi.
        + Khuyến nghị: Không có vấn đề cụ thể được phát hiện trong quá trình kiểm thử này.
