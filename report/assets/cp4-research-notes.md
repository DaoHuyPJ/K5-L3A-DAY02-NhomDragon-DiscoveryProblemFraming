# CP4: Ghi chú research giải pháp đã có

Ghi chú chi tiết cho mục 3.3 của [group_report.md](../team/group_report.md).

| Công cụ / case / pattern | Link | Giải bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Markdownlint / Super-Linter (GitHub Action) | https://github.com/DavidAnson/markdownlint | Kiểm tra định dạng markdown (tiêu đề, cú pháp, khoảng trắng, link hỏng) | Rất nhanh, chạy tự động khi commit/push, chính xác theo rule cứng | Không hiểu ngữ nghĩa nội dung môn học, không đối soát được với Rubric | Dùng Rule cho lỗi format cơ học (tên file, cấu trúc mục, bảng rỗng), không cần dùng AI |
| Turnitin Rubrics & Grading Tools | https://www.turnitin.com/products/feedback-studio/rubrics | Giảng viên dựng ma trận rubric và chấm bài theo tiêu chí | Rubric trực quan, gắn điểm theo mức độ | Phục vụ giảng viên sau khi bài đã nộp; sinh viên không tự kiểm tra trước hạn; không hỗ trợ repo Git/Markdown | Cần một công cụ "pre-flight check" dành cho sinh viên trước khi nộp |
| Workaround: ChatGPT / Claude với prompt tự viết | https://chatgpt.com | Sinh viên dán Rubric và bài nộp, nhờ AI tìm chỗ thiếu | Đọc hiểu tiếng Việt tốt, chỉ ra được thiếu sót về lập luận | Dễ bịa tiêu chí ngoài rubric (hallucination); giới hạn context khi nhiều file; không có ranh giới an toàn | Không để AI chat tự do; chuẩn hóa thành workflow: input cố định → prompt đối chiếu có trích dẫn → output dạng bảng |

## Kết luận từ research

- Lỗi format cơ học: dùng Rule (Markdownlint là ví dụ).
- Đối soát ngữ nghĩa với rubric: chưa có công cụ dành cho sinh viên tự kiểm tra trước hạn, nên nhóm chọn workflow bán thủ công với người duyệt.
- Cách dùng chatbot hiện tại cho thấy cần ràng buộc AI bằng trích dẫn nguyên văn và bước người xác nhận.

> Ghi chú: các link nên được mở lại và kiểm tra còn truy cập được trước khi nộp.
