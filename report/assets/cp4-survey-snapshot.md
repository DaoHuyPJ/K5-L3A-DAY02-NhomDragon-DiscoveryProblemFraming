# CP4: Survey snapshot (khảo sát nhanh 4 sinh viên)

> Người thực hiện: Hoàng Hải Long. Tên người trả lời đã được che trong ảnh chụp: [cp4-survey-result.png](cp4-survey-result.png).
> Mẫu rất nhỏ (n = 4). Đây chỉ là tín hiệu ban đầu, chưa đủ để khái quát cho cả lớp.

## Giả định được kiểm chứng

- **Giả định #2**: sinh viên thường mất điểm hoặc phải nộp lại vì lỗi format / thiếu yêu cầu khi nộp bài.

## Cách hỏi

Chỉ hỏi về việc **đã xảy ra** (lần nộp bài gần nhất gặp lỗi gì), không hỏi giả định kiểu "Bạn có muốn…" (theo The Mom Test).

## Kết quả: 4 phản hồi

| # | Việc đã xảy ra (diễn đạt lại ngắn) | Loại lỗi | Hệ quả |
|---:|---|---|---|
| 1 | Điền form nộp bài nhưng dùng sai tên repo, không thấy repo được reset trên LMS, hỏi có cần gửi lại link repo mới không | Sai tên repo | Phải xin nộp lại |
| 2 | Điền form cần nộp lại vì dùng sai tên repo, quên không để ý có reset, định đổi tên và nộp lại | Sai tên repo | Phải xin nộp lại |
| 3 | Đặt sai tên GitHub (đang để "individual" và lớp "L3A" trong khi quy định ghi L3), muốn nộp lại cho đúng tên | Sai tên repo/GitHub | Phải xin nộp lại |
| 4 | Nộp bị thiếu file (`lab1_report`), hỏi có commit thêm được không | Nộp thiếu yêu cầu | Phải xin bổ sung sau hạn |

## Tổng hợp

- **4/4** bạn từng sai tên (3 trường hợp: tên repo/GitHub) hoặc nộp thiếu yêu cầu (1 trường hợp: thiếu file).
- Cả 4 lỗi đều là **lỗi format cơ học** (tên, file bắt buộc), kiểu lỗi có thể kiểm tra bằng Rule mà không cần AI.

## Insight / opportunity rút ra

Có nhu cầu kiểm tra nhanh tên repo và các file bắt buộc **trước khi nộp**. Đây là cơ sở để tầng 1 của quy trình tương lai dùng Rule (regex tên, kiểm tra file bắt buộc).

## Chưa kiểm chứng (cần làm tiếp)

- Thời gian sinh viên mất để rà soát trước khi nộp (nhóm đang dùng ước tính ~60 phút).
- Cách xử lý hiện tại (workaround) của từng người.
- Nỗi lo AI báo nhầm và việc không muốn AI tự sửa bài: mới là giả định của nhóm.
- Phỏng vấn sâu: chưa thực hiện.
