**Bài làm**
Phần 1: Thiết kế Prompt 3 thành phần chuẩn hóa
1. Vì sao câu hỏi ban đầu khiến AI trả lời sai lệch?
Câu hỏi: “AI ơi phần mềm trạm sạc của tôi bị hỏng rồi làm sao đây?”

Câu hỏi này thiếu thông tin kỹ thuật cần thiết:
- Thiếu ngữ cảnh (Context): Không nêu thiết bị VoltCharge, hệ điều hành Windows 11, vị trí trạm sạc và tác vụ đang thực hiện.
- Thiếu mã lỗi (Raw Error): Không cung cấp thông báo lỗi cụ thể nên AI không biết chương trình đang gặp lỗi quyền truy cập.
- Thiếu yêu cầu (Instruction): Không nói rõ cần dịch lỗi, tìm nguyên nhân hay hướng dẫn khắc phục.
Phần 2: Giải mã lỗi và kịch bản khắc phục
3. Dịch lỗi và giải thích nguyên nhân gốc rễ
Dịch sang tiếng Việt:

Lỗi quyền truy cập: Chương trình không được phép truy cập vào tệp session.log tại thư mục dữ liệu của VoltCharge
4. Ba bước xử lý trên Windows 11
Chỉ thực hiện bởi kỹ thuật viên được ủy quyền
Vì đây là trạm sạc đang vận hành thực tế, cần phối hợp với người phụ trách hệ thống và tuân theo hướng dẫn của nhà cung cấp VoltCharge. Không tự ý thay đổi cấu hình dịch vụ đang cấp điện.

Bước 1: Kiểm tra và chạy chương trình với quyền Administrator
1. Mở Start Menu trên Windows 11.
2. Tìm phần mềm quản trị VoltCharge.
3. Nhấp chuột phải vào biểu tượng chương trình.
4. Chọn Run as administrator.
5. Xác nhận hộp thoại User Account Control (UAC) nếu được phép.
Bước 2: Kiểm tra và phân quyền thư mục data
1. Mở File Explorer.
2. Truy cập thư mục
3. Nhấp chuột phải vào thư mục data, chọn Properties.
4. Chọn thẻ Security.
5. Kiểm tra tài khoản chạy dịch vụ VoltCharge có quyền ghi dữ liệu hay không.
Bước 3: Kiểm tra hoạt động sau khi được cấp quyền
- Yêu cầu người phụ trách khởi động lại dịch vụ theo quy trình vận hành được phê duyệt.
- Kiểm tra nhật ký có ghi dữ liệu mới vào session.log hay không.
- Xác nhận lỗi UnauthorizedAccessException không còn xuất hiện.
- Kiểm tra trạng thái ControllerDaemon đã hoạt động bình thường chưa.
5. Bẫy an ninh: Xử lý API_KEY trước khi gửi cho AI
Nguyên tắc: Tuyệt đối không gửi API Key thật lên ChatGPT, Gemini hoặc nền tảng AI công cộng.

Cách xử lý:
1. Che hoặc xóa mã bí mật: Thay chuỗi API Key bằng nội dung [REDACTED] trước khi gửi.
2. Giữ lại cấu trúc lỗi: Chỉ cung cấp tên biến và vị trí xuất hiện để AI vẫn hiểu được ngữ cảnh.
3. Thu hồi và tạo khóa mới: Nếu API Key thật đã bị gửi lên nền tảng không được phép, cần báo quản trị viên để thu hồi khóa cũ và cấp khóa mới.