JMeter

Kiểm tra hiệu năng trang web

Mục tiêu:

- Sử dụng JMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập trang web https://httpbin.org/get.
- Chạy kịch bản kiểm tra và ghi lại kết quả.
- Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, thông lượng,... .
- Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của trang web trong điều kiện kiểm thử.

Kịch bản kiểm tra:

- Thread Group:
  + Số lượng thread: 100.
  + Thời gian chạy: 60 giây.
  + Ramp-up period: 10 giây.
- HTTP Request:
  + URL: https://httpbin.org/get.
  + Protocol: HTTPS.
  + Server Name: httpbin.org.
  + Path: /get.
  + Method: GET.
  + Content encoding: UTF-8.
- Listeners:
  + View Results Tree.
  + Aggregate Report.
Kết quả kiểm tra:
<img width="397" height="357" alt="image" src="https://github.com/user-attachments/assets/3ce12962-4e86-4553-8054-0f735bac968f" />


Phân tích kết quả kiểm tra:
- Số lượng yêu cầu thành công: [Điền số liệu thực tế].
- Số lượng yêu cầu thất bại: [Điền số liệu thực tế].
- Tỷ lệ yêu cầu thành công: [Điền tỷ lệ thực tế].
- Tỷ lệ yêu cầu thất bại: [Điền tỷ lệ thực tế].
- Thời gian phản hồi trung bình: [Điền số liệu thực tế].
- Thời gian phản hồi trung vị: [Điền số liệu thực tế nếu có].
- Thời gian phản hồi percentile 90: [Điền số liệu thực tế nếu có].
- Thông lượng: [Điền số liệu thực tế] yêu cầu/giây.
Kết luận:
Dựa trên kết quả kiểm thử thực tế, đánh giá hiệu năng của HTTPBin thông qua thời gian phản hồi, tỷ lệ yêu cầu thất bại và thông lượng. Nếu tỷ lệ yêu cầu thành công cao, thời gian phản hồi thấp và thông lượng ổn định trong quá trình kiểm thử, có thể nhận xét rằng website đáp ứng tốt trong phạm vi tải đã thực hiện.
Kết quả kiểm thử chỉ phản ánh điều kiện thử nghiệm cụ thể, không đại diện cho hiệu năng của website trong mọi thời điểm hoặc mọi mức tải.
Hình ảnh tổng quát
Chụp ảnh giao diện Apache JMeter, cấu hình Thread Group và HTTP Request để minh họa quá trình xây dựng kịch bản kiểm thử.


