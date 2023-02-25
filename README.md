# Schiper-Eggli-Sandoz-Algorithm
This project is used to implement SES algorthim in Distributed Systems

# Detail
Đồ án SES.
Đồ án 2 sv làm
Deadline: 13-03-2023
Mục tiêu: Hiểu và cài đặt thuật toán SES
## 1. Mô tả
Viết chương trình minh họa cài đặt thuật toán SES. Chương trình bao gồm 7 processes, có thể chạy
trên 1 hoặc nhiều máy tính. Mỗi process tự động gửi tới mỗi process còn lại 150 messages. Nội dung
của message có thể đơn giản chỉ là: “message 1”, “message 2”,… Thời gian phát sinh các message là
ngẫu nhiên, ví dụ 10 messages trên phút hoặc 100 messages trên phút.
## 2. Thiết kế chương trình
Chương trình tuân thủ theo thuật toán SES trong bài giảng.
Yêu cầu chính của đồ án là phải hiển thị rõ ràng việc buffering hay delivery các messages trên màn
hình và trong log file. Ví dụ, msg X bị buffered bởi vị phải chờ msg Y, thì chương trình phải hiển thị:
- Trạng thái của msg X (buffer or delivery)
- Time stamp của msg X
- Chỉ ra khi msg Y được delivery thì msg X được lấy từ trong buffer để deliver.
- Chỉ ra hệ thống đồng hồ quản lý các thông điệp của chương trình đã được cập nhật
- Có thể sử dụng thêm các chức năng từ bàn phím để giải thích chương trình của bạn cho các
trợ giảng dễ dàng hơn.
## 3. Demo
Chương trình demo phải cho thực thi cùng lúc ít nhất 7 processes. Mỗi process sẽ phải tạo 6 threads
chạy song song để gửi msg cho 6 processes còn lại. Các thông số của chương trình nên được định
trước trong configuration file, ví dụ địa chỉ IP, port, processed,... Mỗi process phải có khả năng xử lý
150 msgs từ mỗi process khác mà chương trình không bị treo, hay dừng giữa chừng. Log file phải có
cho mỗi process.
## 4. Nộp bài
Nộp duy nhất một thư mục đã nén theo dạng <MSSV>.zip, ví dụ 1231521_1231522.zip trong đó là
MSSV của sinh viên làm đồ án.
Trong thư mục nộp bài phải có file readme.doc để ghi chú về chương trình của nhóm. Tài liệu sử dụng
và thiết kế của chương trình
## 5. Chấm điểm
- 15% tài liệu đi kèm
- 25% trình bày log file
- 15% phần hiển thị, giao tiếp người sử dụng
- 45% tính đúng đắn của chương trìn