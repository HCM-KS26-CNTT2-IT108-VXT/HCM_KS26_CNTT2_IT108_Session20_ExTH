# BÀI TẬP TỔNG HỢP: HÀNH TRÌNH XỬ LÝ 1 LỖI CÀI ĐẶT THẬT

## PHẦN 1 – GOoGLING ĐÚNG CÁCH

### 1. Vì sao câu hỏi văn nói tìm kiếm kém hiệu quả?

Vì câu hỏi quá dài, dùng cách nói chuyện thông thường và không có từ khóa kỹ thuật cụ thể nên Google khó tìm đúng lỗi.

### 2. Bóc tách lỗi theo 3 thành phần

| Thành phần | Nội dung bóc tách |
|---|---|
| Tên phần mềm / Hệ điều hành | Node.js / Windows 11 |
| Mã lỗi nguyên văn | `'npm' is not recognized as an internal or external command, operable program or batch file.` |
| Thao tác đang làm | Gõ lệnh `npm -v` trong Terminal của VS Code để kiểm tra phiên bản npm. |

### 3. Ba câu truy vấn Google

- **Dùng site:**
  `site:stackoverflow.com npm not recognized Windows 11`

- **Dùng ngoặc kép:**
  `"npm is not recognized as an internal or external command"`

- **Dùng dấu -:**
  `npm not recognized Windows 11 -windows-xp`

## PHẦN 2 – THẨM ĐỊNH STACKOVERFLOW

### 1. So sánh câu trả lời A và B

| Tiêu chí | Câu trả lời A | Câu trả lời B |
|---|---|---|
| Vote & Tích xanh | +186, có tích xanh. | +2, không có tích xanh. |
| Thời gian đăng bài | 2 năm trước. | 9 năm trước. |
| Tags | node.js, windows, npm. | node.js, windows-xp. |

### 2. Lựa chọn câu trả lời

Em chọn câu trả lời A vì có nhiều lượt bình chọn, có tích xanh và nội dung phù hợp với lỗi đang gặp.

Câu B là bẫy vì hướng dẫn cài driver mạng cho Windows XP không liên quan đến lỗi npm trên Windows 11.

### 3. Quy trình 30 giây đọc lướt

1. Xem số lượt bình chọn và tích xanh.
2. Kiểm tra Tags có phù hợp không.
3. Xem thời gian đăng bài.
4. Đọc nội dung câu trả lời.
5. Kiểm tra xem câu trả lời có phù hợp với lỗi của mình không.

## PHẦN 3 – HỎI AI ĐÚNG CÁCH VÀ NHẬN DIỆN RỦI RO

### 1. Viết Prompt 3 thành phần

**[Context – Ngữ cảnh]**

Em đang sử dụng Windows 11, đã cài Node.js và mở Terminal trong VS Code để kiểm tra npm.

**[Raw Error – Lỗi nguyên văn]**

```text
'npm' is not recognized as an internal or external command, operable program or batch file.
```

Em đã thử thêm đường dẫn Node.js vào biến môi trường PATH và mở Terminal mới nhưng lỗi vẫn xuất hiện.

**[Instruction – Yêu cầu]**

Hãy giải thích nguyên nhân bằng tiếng Việt dễ hiểu và hướng dẫn cách kiểm tra, khắc phục từng bước. Không đưa ra lệnh nguy hiểm hoặc làm ảnh hưởng đến Windows.

### 2. Đánh giá câu trả lời của AI

Câu trả lời của AI không an toàn vì lệnh `del /f /s /q C:\Windows\System32\*` có thể xóa các file hệ thống quan trọng, khiến Windows bị lỗi hoặc không khởi động được.

### 3. Phản hồi lại AI

Em sẽ hỏi:

"Lệnh này có thể gây ảnh hưởng gì đến Windows? Có cách nào kiểm tra và sửa lỗi PATH an toàn hơn mà không xóa file hệ thống không?"

## PHẦN 4 – VIẾT BUG REPORT CHUẨN

### 1. Tin nhắn kém

Thầy ơi máy em bị lỗi npm rồi, thầy giúp em với ạ!

### 2. Tin nhắn chuẩn theo Bug Reporting Framework

**[Context]**

Em sử dụng Windows 11, đã cài Node.js và mở Terminal trong VS Code.

**[Expected]**

Em mong muốn lệnh `npm -v` hiển thị phiên bản npm.

**[Actual]**

Máy báo lỗi `'npm' is not recognized as an internal or external command, operable program or batch file.` Em đã thử thêm PATH và mở Terminal mới nhưng vẫn bị lỗi.

**[Log & Screenshot]**

Em gửi kèm ảnh chụp màn hình thông báo lỗi để thầy kiểm tra và hướng dẫn khắc phục.

### 3. Phím tắt và lưu ý bảo mật

- **Phím tắt:** `Windows + Shift + S` để chụp một vùng màn hình.
- **Lưu ý:** Che thông tin cá nhân, mật khẩu và API Key trước khi gửi ảnh.