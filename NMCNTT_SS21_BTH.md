BÀI LÀM: QUY TRÌNH 4 BƯỚC XỬ LÝ LỖI npm -v TRÊN WINDOWS 11
PHẦN 1 – GOOGLING ĐÚNG CÁCH
1. Vì sao câu hỏi văn nói là Bad Query?
Nguyên nhân:
- Sử dụng ngôn ngữ giao tiếp, không chứa từ khóa kỹ thuật cụ thể.
- Không đề cập hệ điều hành Windows 11.
- Không có thông báo lỗi nguyên văn để Google tìm kiếm chính xác.
- Chứa nhiều từ thừa như "tại sao", "em", "thầy ơi".
2. Bóc tách lỗi theo 3 thành phần cốt lõi
Thành phần	Nội dung bóc tách
Tên phần mềm / Hệ điều hành	Node.js / Windows 11
Mã lỗi nguyên văn	'npm' is not recognized as an internal or external command, operable program or batch file.
Thao tác đang làm	Gõ lệnh npm -v trong Terminal của VS Code để kiểm tra phiên bản npm.

3. Ba câu truy vấn Google tối ưu
Câu 1 – Sử dụng toán tử site:
site:stackoverflow.com npm not recognized Windows 11 PATH
Câu 2 – Sử dụng toán tử ngoặc kép " "
"npm is not recognized as an internal or external command" Windows 11
Câu 3 – Sử dụng toán tử -
npm not recognized Windows PATH -windows-xp
PHẦN 2 – THẨM ĐỊNH STACKOVERFLOW
1. So sánh câu trả lời A và B
Tiêu chí	Câu trả lời A	Câu trả lời B
Vote & Tích xanh	+186 Upvotes, có Accepted Answer (tích xanh).	+2 Upvotes, không có tích xanh.
Thời gian đăng bài	2 năm trước, tương đối mới.	9 năm trước, khá cũ.
Tags khớp hệ điều hành/phần mềm	[node.js], [windows], [npm], phù hợp với vấn đề.	[node.js], [windows-xp], không phù hợp Windows 11.

2. Kết luận lựa chọn
Lựa chọn: Câu trả lời A.

Lý do:
- Có 186 lượt Upvote và được người hỏi xác nhận bằng tích xanh.
- Tags phù hợp với Node.js, npm và Windows.
- Nội dung hướng dẫn kiểm tra biến môi trường PATH, đúng với nguyên nhân có thể gây ra lỗi không nhận diện lệnh npm.
3. Quy trình 30 giây đọc lướt StackOverflow
Thực hiện theo đúng thứ tự:
1. Kiểm tra Tags: Xem bài viết có đúng phần mềm và hệ điều hành không.
2. Kiểm tra Vote: Ưu tiên câu trả lời có nhiều Upvotes.
3. Kiểm tra Accepted Answer: Tìm câu trả lời có tích xanh.
4. Kiểm tra thời gian: Ưu tiên hướng dẫn còn phù hợp với phiên bản hiện tại.
5. Đọc giải pháp: Xem nội dung hướng dẫn có liên quan trực tiếp đến lỗi đang gặp không.
PHẦN 3 – HỎI AI ĐÚNG CÁCH VÀ NHẬN DIỆN RỦI RO
1. Viết Prompt theo công thức 3 thành phần
**1. Ngữ cảnh (Context):**

Tôi vừa cài đặt Node.js trên laptop Windows 11 mới để học lập trình web. Tôi đang sử dụng Terminal tích hợp trong VS Code để kiểm tra phiên bản npm.

**2. Lỗi nguyên văn (Error):**

Khi chạy lệnh `npm -v`, Terminal hiển thị thông báo:

```text
'npm' is not recognized as an internal or external command, operable program or batch file.
```

Tôi đã thử thêm đường dẫn cài đặt Node.js (`C:\Program Files\nodejs\`) vào biến môi trường `PATH` và mở Terminal mới nhưng lỗi vẫn xuất hiện.

**3. Yêu cầu (Request):**

Hãy giải thích nguyên nhân có thể gây ra lỗi bằng tiếng Việt, hướng dẫn từng bước kiểm tra và khắc phục an toàn trên Windows 11. Ưu tiên các phương pháp không gây ảnh hưởng đến dữ liệu và hệ thống. Giải thích mục đích từng thao tác và cảnh báo rõ nếu có lệnh nguy hiểm. Không đề xuất xóa dữ liệu hệ thống hoặc chạy lệnh với quyền Administrator khi chưa thực sự cần thiết.
PHẦN 4 – VIẾT BUG REPORT CHUẨN ĐỂ NHỜ HỖ TRỢ
1. Tin nhắn kém (Bad Bug Report)
Thầy ơi, máy em bị lỗi npm rồi, em cài Node.js mà không chạy được. Thầy xem giúp em với ạ!
2. Tin nhắn chuẩn theo Bug Reporting Framework
Em chào thầy ạ! Em đang gặp lỗi khi kiểm tra npm trên laptop Windows 11, mong thầy hỗ trợ.

**1. Context (Bối cảnh):**

Em vừa cài đặt Node.js trên laptop Windows 11 và sử dụng Terminal trong VS Code để kiểm tra phiên bản npm.

**2. Expected (Kết quả mong muốn):**

Sau khi cài đặt Node.js thành công, khi chạy lệnh `npm -v`, Terminal sẽ hiển thị số phiên bản npm.

**3. Actual (Kết quả thực tế):**

Khi chạy `npm -v`, Terminal báo lỗi:

```text
'npm' is not recognized as an internal or external command, operable program or batch file.
```

Em đã thử thêm đường dẫn cài đặt Node.js (`C:\Program Files\nodejs\`) vào biến môi trường `PATH` và mở Terminal mới nhưng lỗi tương tự vẫn xuất hiện.

**4. Log & Screenshot (Nhật ký và ảnh chụp):**

Em gửi kèm ảnh chụp màn hình thông báo lỗi khi chạy lệnh `npm -v` để thầy tiện kiểm tra.

Nhờ thầy hướng dẫn em cách xác định nguyên nhân và khắc phục lỗi này an toàn trên Windows 11.

Em cảm ơn thầy ạ!
3. Phím tắt chụp màn hình và lưu ý bảo mật
- Phím tắt: Windows + Shift + S.
- Chức năng: Mở Snipping Tool để chọn vùng màn hình cần chụp.
- Lưu ý bảo mật: Che hoặc xóa thông tin nhạy cảm như mật khẩu, API Key, token truy cập và thông tin cá nhân trước khi gửi ảnh cho người khác.