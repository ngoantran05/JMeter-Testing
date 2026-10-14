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
- Số lượng yêu cầu thành công: 200.
- Số lượng yêu cầu thất bại: 0%.
- Thời gian phản hồi trung bình: 727 ms.
- Thời gian phản hồi trung vị: 869 ms.
- Thời gian phản hồi percentile 90: 1.528 ms.
- Thông lượng: 17. yêu cầu/giây.
Kết luận:
Trang web https://httpbin.org/get có hiệu năng tốt. Số lượng yêu cầu thành công rất cao (100%), số lượng yêu cầu thất bại rất thấp (0%). Thời gian phản hồi trung bình, trung vị và percentil 90 đều ở mức cao. Chuyển tải của trang web cũng khá cao (17.1 yêu cầu/giây).
Hình ảnh tổng quát
<img width="1917" height="605" alt="Screenshot 2026-10-14 105848" src="https://github.com/user-attachments/assets/70be3ee1-dd51-4332-88ff-7b41ee53a340" />





