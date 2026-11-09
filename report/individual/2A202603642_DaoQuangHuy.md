# Báo cáo cá nhân — 2A202603642_DaoQuangHuy

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Đào Quang Huy
- MSSV: 2A202603642
- Email trường (không bắt buộc, repo có thể để public): 
- Tên nhóm: NhomDragon
- Link repo nhóm: https://github.com/DaoHuyPJ/K5-L3-Day02-NhomDragon-DiscoveryProblemFraming

**Bối cảnh / Nhân vật:** Huy, sinh viên ngành Công nghệ thông tin / Nhóm trưởng nhóm lab môn học K5, thường xuyên làm việc nhóm trên GitHub, quản lý các file báo cáo Markdown và chịu trách nhiệm đối soát toàn bộ bài làm với tài liệu Rubric chấm điểm của giảng viên trước deadline mỗi tuần.

**Vì sao đây là bài toán tốt:** Actor cụ thể (sinh viên nộp bài / nhóm trưởng); quy trình lặp lại đều đặn mỗi tuần; bottleneck rất rõ ở khâu đọc đối chiếu chi tiết từng dòng tiêu chí (20–25 phút); có baseline thời gian đo thật (60 phút); so sánh được rõ ràng 4 mức No AI / Rule / Workflow / Agent; và quan trọng nhất, **kết quả kiểm chứng cùng research làm nhóm đổi kết luận** (từ định xây AI Agent tự động sửa bài sang chọn giải pháp Workflow bán thủ công kết hợp Rule linter).

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi chuẩn bị nộp bài lab/project trước hạn 2 tiếng, tôi muốn đối soát toàn bộ file bài làm với rubric chấm điểm, để không bị mất điểm oan do thiếu mục hoặc sai định dạng | Sinh viên, cả nhóm làm bài | Mất 45–60 phút mỗi lần nộp lab; 2/4 bài lab gần nhất bị trừ từ 1–2 điểm vì sót checklist nhỏ |
| 2 | Tốn thời gian | Khi gặp lỗi cấu hình môi trường hoặc bug thư viện lạ trong dự án, tôi muốn tìm nhanh giải pháp từ các thread GitHub Issue và Discord liên quan, để sửa lỗi và tiếp tục làm bài | Sinh viên kỹ thuật, dev trong nhóm | Trung bình mất 60–90 phút/lần tìm kiếm; tuần trước mất cả buổi chiều (hơn 3 tiếng) vì lỗi version mismatch của thư viện |
| 3 | Lặp lại | Khi đến hạn báo cáo tiến độ đồ án mỗi tuần, tôi muốn tổng hợp các commit và pull request đã hoàn thành thành văn bản tóm tắt, để báo cáo cho giảng viên/mentor đúng hạn | Nhóm trưởng, thành viên dự án | Lặp lại mỗi tuần 1 lần vào Chủ nhật; mất 40–50 phút lọc git log và nhắn tin hỏi từng bạn |
| 4 | Lặp lại | Khi bắt đầu làm bài lab mới, tôi muốn kiểm tra và thiết lập khung thư mục theo đúng quy chuẩn đề bài yêu cầu, để cả nhóm không bị commit nhầm file rác hoặc sai cấu trúc repo | Cả nhóm (2–4 người) | 1–2 lần/tuần mỗi khi mở lab mới; mất 20–30 phút setup và giải thích lại cho thành viên |
| 5 | Tốn thời gian | Khi phải đọc tài liệu kỹ thuật dài 30–50 trang để chọn kiến trúc cho bài tập lớn, tôi muốn nắm nhanh các ưu/nhược điểm và điều kiện áp dụng của từng phương pháp, để chọn đúng giải pháp trước buổi họp nhóm | Sinh viên, nhóm làm đồ án | 2–3 tuần một lần; mất 2–3 tiếng đọc lướt tài liệu và ghi chú |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi cần biết lý do nhóm quyết định chọn phương án thiết kế A thay vì B từ tuần trước, tôi muốn tìm lại đúng đoạn thảo luận và kết luận đã chốt, để không phải tranh cãi lại từ đầu | Cả nhóm | Xảy ra 2–3 lần/tuần; mất 15–20 phút lục lại hàng trăm tin nhắn trong Discord/Zalo |
| 7 | Pain từ người khác | Khi thành viên mới vào nhóm hoặc clone repo về máy cá nhân, họ muốn chạy được ngay môi trường mà không bị lỗi dependency, để bắt đầu làm task được giao | Thành viên trong nhóm, người mới | Nhóm trưởng/người setup phải support giải thích 2–3 lần/người; mất 30–45 phút mỗi lần qua Google Meet/tin nhắn |
| 8 | Pain từ người khác | Khi giảng viên/mentor cần chấm bài hoặc xem demo tiến độ, họ muốn thấy rõ đóng góp cụ thể của từng thành viên, để đánh giá điểm số công bằng và chính xác | Giảng viên, sinh viên trong nhóm | Cuối mỗi kỳ hoặc mỗi mốc sprint; thường mất 1 tiếng đối chiếu git commit log với phân công công việc |
| 9 | Tốn thời gian | Khi làm bài tập AI cần chuẩn bị dữ liệu thử nghiệm, tôi muốn lọc và gán nhãn nhanh các mẫu văn bản/dữ liệu nhỏ, để có dataset kiểm thử mô hình | Sinh viên làm môn AI/Data | Mất khoảng 90–120 phút gán nhãn thủ công từng dòng dữ liệu mẫu |
| 10 | Lặp lại | Khi kết thúc buổi họp nhóm, tôi muốn có danh sách các đầu việc (action items) kèm người phụ trách và deadline, để các bạn không bị quên việc | Tất cả thành viên trong nhóm | Mỗi tuần 1–2 buổi họp; mất 20–25 phút vừa họp vừa ghi chép và gửi lại vào kênh chat |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý giữ lại:** Ý #9 (Lọc và gán nhãn dataset thử nghiệm) và Ý #10 (Ghi chép action item sau họp nhóm) do AI gợi ý sau khi tôi cung cấp bối cảnh học tập/làm bài tập nhóm. Tôi đã tự viết lại theo đúng trải nghiệm thực tế của các đồ án đã làm và bổ sung thời gian đo lường thật.
- **Ý bỏ:** AI có gợi ý "Xây dựng trợ lý AI tự động code và giải toàn bộ bài tập lab" và "Hệ thống tự động chấm điểm bài tập thay giáo viên". Tôi bỏ vì các ý này vi phạm nguyên tắc bài lab (đây là giải pháp AI trá hình chứ không phải problem cụ thể, quá rộng và không có quy trình rõ ràng đo lường được).

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Đối soát rubric & file bài nộp lab (#1) | Quy trình lặp lại thường xuyên, bottleneck rất rõ ở khâu rà soát chéo giữa rubric và nội dung các file markdown, impact sát sườn (điểm số môn học) | Tiêu chí đánh giá tính "đầy đủ, chặt chẽ" của nội dung có thể mang tính định tính |
| 2 | Tìm kiếm giải pháp debug lỗi kỹ thuật (#2) | Nỗi đau thật, tốn rất nhiều thời gian khi làm bài lab/dự án, dễ đo lường thời gian giảm được | Bản quyền hoặc quyền truy cập vào các forum kín/nhiều nguồn phân mảnh |
| 3 | Tổng hợp báo cáo tiến độ tuần từ git commit (#3) | Quy trình rõ ràng, đầu vào (git log, PR) đã có cấu trúc, dễ so sánh các mức No AI / Rule / Workflow | Dữ liệu commit message của thành viên đôi khi viết quá sơ sài ("fix bug", "update") |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị nộp bài lab/project trước hạn 2 tiếng, tôi muốn đối soát toàn bộ file bài làm với rubric chấm điểm, để không bị mất điểm oan do thiếu mục hoặc sai định dạng |
| Actor | Sinh viên, nhóm trưởng chịu trách nhiệm nộp bài lab kỹ thuật |
| Thời điểm / bối cảnh | Trước deadline nộp bài từ 1–2 tiếng trên GitHub/LMS |
| Quy trình hiện tại (3–7 bước) | 1. Mở file RUBRIC.md và CHECKPOINTS.md đọc từng tiêu chí (10') · 2. Mở từng file báo cáo markdown trong repo để tìm xem nội dung đã viết chưa (15') · 3. Đọc kỹ từng đoạn xem có đúng định dạng, đủ con số đo lường không (20') · 4. Đánh dấu các phần còn thiếu vào giấy nháp hoặc chat (10') · 5. Nhắc thành viên sửa lại phần thiếu trước khi commit cuối (15') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: Đọc đối chiếu chi tiết từng đoạn nội dung trong file báo cáo với tiêu chuẩn của Rubric (mất khoảng 20–25 phút, rất dễ sót khi mệt hoặc gấp) |
| Impact (nếu không giải thì sao) | Mất 60 phút mỗi lần nộp lab; 2/4 lab gần nhất bị mất từ 1–2 điểm (trên thang 10) vì sót quy định cấu trúc file hoặc thiếu con số chứng minh |
| Success metric (baseline → target) | Tổng thời gian đối soát giảm từ 60 phút xuống dưới 20 phút; Tỷ lệ phát hiện đúng các mục thiếu sót đạt > 90%; 0 bài nộp bị trừ điểm cấu trúc |
| Phương án không dùng AI | Dùng một file checklist dạng bảng Markdown in sẵn (Template checklist) để người nộp tự tick tay từng mục: giảm được nguy cơ quên mục nhưng vẫn mất trọn 45–60 phút đọc tay |
| Giả thuyết về AI | AI nhận đầu vào là file Rubric + nội dung bài nộp, trích xuất bảng đối chiếu các tiêu chí Đạt / Thiếu / Cần sửa kèm trích dẫn dòng; con người kiểm tra lại và sửa bài |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 60 phút

[1 Đọc Rubric: 10'] → [2 Mở duyệt từng file .md: 15']
→ [3 Đọc đối chiếu từng tiêu chí với nội dung: 20'] ← BOTTLENECK
→ [4 Ghi chú mục thiếu/lỗi: 5'] → [5 Nhắc sửa & kiểm lại: 10']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi gặp lỗi cấu hình môi trường hoặc bug thư viện lạ trong dự án, tôi muốn tìm nhanh giải pháp từ các thread GitHub Issue và Discord liên quan, để sửa lỗi và tiếp tục làm bài |
| Actor | Sinh viên lập trình, thành viên kỹ thuật trong nhóm |
| Thời điểm / bối cảnh | Trong quá trình code hoặc setup môi trường chạy lab |
| Quy trình hiện tại (3–7 bước) | 1. Copy thông báo lỗi từ terminal (2') · 2. Tìm kiếm trên Google / GitHub Issue (10') · 3. Đọc lướt qua 5–10 bài viết/thread dài (25') · 4. Thử lần lượt các lệnh/cách sửa được đề xuất (20') · 5. Kiểm tra code đã chạy được chưa và ghi chú cách sửa (10') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: Đọc và lọc trong các thread dài hàng chục bình luận để tìm đúng phiên bản thư viện/hệ điều hành tương ứng (mất 25–30 phút) |
| Impact (nếu không giải thì sao) | Mỗi lần gặp bug lạ mất từ 60–90 phút; làm chậm tiến độ cả nhóm, gây ức chế và trì hoãn |
| Success metric (baseline → target) | Thời gian tìm ra giải pháp phù hợp giảm từ 60 phút xuống dưới 15 phút |
| Phương án không dùng AI | Xây dựng file FAQ nội bộ của nhóm ghi lại các lỗi đã gặp và cách sửa: chỉ giải quyết được các lỗi cũ đã từng xuất hiện |
| Giả thuyết về AI | AI tổng hợp nhanh các cách giải quyết khả dĩ nhất từ log lỗi và ngữ cảnh phiên bản hệ điều hành |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 67 phút

[1 Copy error log: 2'] → [2 Search GitHub/Google: 10']
→ [3 Đọc lọc 5-10 thread dài: 25'] ← BOTTLENECK
→ [4 Thử áp dụng từng giải pháp: 20'] → [5 Kiểm tra lại: 10']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến hạn báo cáo tiến độ đồ án mỗi tuần, tôi muốn tổng hợp các commit và pull request đã hoàn thành thành văn bản tóm tắt, để báo cáo cho giảng viên/mentor đúng hạn |
| Actor | Nhóm trưởng sinh viên, người phụ trách repo |
| Thời điểm / bối cảnh | Tối Chủ nhật hàng tuần trước buổi review sáng thứ Hai |
| Quy trình hiện tại (3–7 bước) | 1. Mở GitHub xem danh sách commit và PR trong tuần (10') · 2. Nhắn tin hỏi thành viên nếu commit message viết chung chung (15') · 3. Viết nháp bản tổng hợp thành tựu, việc chưa xong và blocker (15') · 4. Rà soát format theo template của môn học (5') · 5. Gửi lên group lớp/LMS (5') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 và 3: Hỏi lại chi tiết và tổng hợp thành đoạn văn báo cáo mạch lạc (mất 25–30 phút) |
| Impact (nếu không giải thì sao) | Mất 50 phút mỗi tuần; nếu làm ẩu thì báo cáo sơ sài, giảng viên đánh giá thấp tinh thần làm việc nhóm |
| Success metric (baseline → target) | Thời gian hoàn thiện báo cáo tuần giảm từ 50 phút xuống dưới 15 phút |
| Phương án không dùng AI | Bắt buộc nhóm tuân thủ chuẩn commit message (Conventional Commits) và viết PR template: giảm bớt bước hỏi lại nhưng vẫn mất thời gian tổng hợp narrative |
| Giả thuyết về AI | AI đọc git diff / PR description và tạo nháp bản báo cáo tiến độ tuần theo template; nhóm trưởng duyệt và gửi |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 50 phút

[1 Xem git log/PR: 10'] → [2 Hỏi lại thành viên: 15']
→ [3 Viết nháp narrative báo cáo: 15'] ← BOTTLENECK
→ [4 Format theo template: 5'] → [5 Nộp/gửi báo cáo: 5']
```

### Card muốn pitch nhất

- Card số: 1 (Đối soát rubric chấm điểm với file bài làm nộp lab)
- Vì sao: Đây là bài toán cực kỳ quen thuộc với mọi sinh viên công nghệ, xảy ra thường xuyên ở mọi môn học có lab/dự án lớn; quy trình có bước nghẽn rất rõ ràng (đọc đối chiếu chi tiết), có dữ liệu đầu vào cụ thể (file Markdown và Rubric), và mang lại giá trị thiết thực tức thì (không lo bị trừ điểm oan).
- Câu hỏi muốn nhóm phản biện: Rubric có những tiêu chí mang tính định tính (ví dụ: "lập luận chặt chẽ", "trải nghiệm thật") thì làm sao một quy trình tự động/AI có thể đánh giá chính xác mà không bị ảo giác (hallucination)?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Success metric "không bị trừ điểm" là mong muốn gián tiếp, phụ thuộc vào người chấm chứ không chỉ phụ thuộc vào việc đối soát | Đồng ý | Đã bổ sung metric trực tiếp đo được: "Thời gian đối soát giảm từ 60 phút xuống dưới 20 phút" và "Tỷ lệ phát hiện đúng các tiêu chí thiếu sót đạt > 90%" |
| Đề xuất biến thành một "AI Agent tự động sửa file bài nộp luôn cho sinh viên" | Không đồng ý | Từ chối vì rủi ro sai sót rất cao và vi phạm tính trung thực học thuật. Giữ vững ranh giới: AI chỉ làm nhiệm vụ trích xuất bảng đối soát (Workflow), quyền sửa nội dung phải 100% thuộc về sinh viên |
| Bước 1 đọc Rubric chưa tính đến trường hợp Rubric có nhiều file phân mảnh (như RULES, RUBRIC, SUBMISSION) | Đồng ý | Đã chỉnh lại mô tả bước 1 và bước 2 trong quy trình: gộp việc rà soát từ các nguồn tài liệu yêu cầu của lab |

### Problem Statement v0 & v1 (Chuẩn hóa từ Card #1 theo mẫu bài lab)

#### Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên ngành Công nghệ thông tin / Nhóm trưởng chịu trách nhiệm nộp bài lab kỹ thuật trên GitHub/LMS |
| **Quy trình** | Trước deadline 2 tiếng: đọc Rubric.md & Checkpoints.md, duyệt từng file .md trong repo, đối chiếu chi tiết từng tiêu chí với nội dung, ghi chú mục thiếu, nhắc thành viên sửa và commit |
| **Bottleneck** | Bước đọc đối chiếu chi tiết từng dòng Rubric với bài làm mất khoảng 20–25 phút, rất dễ sót do hoa mắt và áp lực cận deadline |
| **Impact** | Tiêu tốn 45–60 phút/lần nộp lab; 86.4% sinh viên từng bị trừ 1–2 điểm oan do lỗi cấu trúc file hoặc sót checklist nhỏ; gây căng thẳng trong nhóm trước giờ G |
| **Success Metric** | Tổng thời gian rà soát từ 60' xuống dưới 20' (bấm giờ thực tế); tỷ lệ phát hiện đúng các tiêu chí thiếu sót đạt $\ge 90\%$; 0 bài nộp bị trừ điểm cấu trúc/format |
| **Boundary** | AI không được tự động sửa nội dung file markdown, không tự ý commit hay nộp bài lên LMS thay sinh viên, không tự phán xét đúng/sai tuyệt đối |

**Phản biện nhận được:** AI chỉ ra metric "0 bài bị trừ điểm" là kết quả gián tiếp, phụ thuộc vào việc sinh viên có chịu sửa bài hay không. Nhóm đã đồng ý và bổ sung metric trực tiếp vào v1: Tỷ lệ phát hiện lỗi thiếu sót $\ge 90\%$ và tỷ lệ báo nhầm (False Positive) $\le 10\%$.

#### Problem Statement v1 + Tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên ngành Công nghệ thông tin / Nhóm trưởng chịu trách nhiệm nộp bài lab kỹ thuật trên GitHub/LMS |
| **Quy trình** | Chạy Rule Linter kiểm tra format cứng → Workflow LLM trích xuất bảng đối soát → Sinh viên duyệt các cảnh báo & tự sửa bài → Sinh viên commit & nộp |
| **Bottleneck** | Bước đọc đối chiếu chi tiết tiêu chí Rubric với nội dung bài làm (mất 20–25 phút) |
| **Impact** | Tiêu tốn 45–60 phút/lần nộp; 86.4% sinh viên từng bị trừ 1–2 điểm oan |
| **Success Metric** | (1) Tổng thời gian rà soát từ 60' xuống dưới 20'; (2) Tỷ lệ phát hiện đúng thiếu sót $\ge 90\%$; (3) Tỷ lệ báo nhầm (False Positive) $\le 10\%$; (4) 0 bài nộp bị trừ điểm cấu trúc |
| **Boundary** | AI không tự ý sửa file, không tự commit/push lên LMS; bắt buộc phải trích dẫn nguyên văn (citation) số dòng; con người duyệt 100% (HITL) |
| **AI intervention point** | Chen vào giữa bước kiểm tra format cơ học và bước sinh viên duyệt bài: LLM trích xuất bảng ma trận đối chiếu 3 cột |
| **Mức chọn** | Workflow bán thủ công (Human-in-the-loop) |
| **Rủi ro & người kiểm tra** | Rủi ro AI báo nhầm (False Positive) gây hoang mang trước deadline → Nhóm trưởng kiểm tra từng dòng cảnh báo và đối chiếu file gốc trước khi sửa |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch Card #1 (Đối soát rubric bài lab kỹ thuật), nêu rõ bối cảnh trước deadline 2 tiếng và bước nghẽn đọc đối chiếu chi tiết (20–25') | Nhóm thống nhất chọn làm Candidate Problem chính cho cả bài lab |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt cho Long: *"1. Merge conflict là vấn đề về kỷ luật git và giao tiếp nhóm, công nghệ có can thiệp được tận gốc không? 2. Docker hoặc file requirements.txt chuẩn đã giải quyết việc setup demo rồi, bài toán đó có thực sự cần thiết kế mới không?"* | Long đồng ý và nhóm quyết định loại bài toán chia task git và setup demo để tập trung vào bài toán đối soát rubric |
| Nhận phản biện | Câu hỏi tôi nhận được từ Long: *"Rubric có những tiêu chí định tính (như 'lập luận chặt', 'trải nghiệm thật') thì đối soát tự động kiểu gì mà không bị hallucinate?"* | Tôi đã sửa gì: Thay vì để AI đánh giá toàn bộ, tôi sửa thiết kế thành: Rule xử lý định dạng/regex cơ học; AI trích xuất checklist và chỉ ra đoạn văn bản liên quan; con người trực tiếp đọc duyệt và sửa (Human-in-the-loop) |
| Gom cluster / cây OST | Tổng hợp 6 candidate thành 3 cụm A (Chất lượng & Tuân thủ), B (Debug lỗi kỹ thuật), C (Cộng tác nhóm); vẽ cây OST với 1 outcome duy nhất | Loại bỏ các ý tưởng giải pháp trá hình (như chatbot tự code, script commit tự động) |
| Chọn candidate problem | Chấm điểm shortlist trên bảng 7 tiêu chí cùng Long | Chốt bài toán #1 với số điểm cao nhất (35/35) |
| Kiểm chứng / research | Tìm kiếm và đối soát 3 giải pháp đã có trên thị trường (Turnitin, GitHub Actions Linter, Grammarly) | Giúp nhóm nhận ra khoảng trống: Chưa có công cụ nào kết hợp đối soát rubric tùy biến môn học với các file markdown bài tập |
| Quy trình nhóm | Phối hợp cùng Long xây dựng quy trình trước/sau và thiết lập phương án quay về (fallback) | Quy trình tương lai rút ngắn từ 5 bước thủ công xuống còn 1 bước bán thủ công có con người duyệt |
| Problem Statement | Viết dự thảo Problem Statement v0 và nâng cấp lên v1 | Bổ sung đầy đủ 6 trường + AI intervention point + ranh giới boundary an toàn |
| Mức can thiệp AI | Lập luận ma trận mơ hồ × phức tạp và điền AI Canvas rút gọn | Chứng minh vì sao mức Workflow là tối ưu, không chọn Agent |
| Quyết định | Cùng Long đánh giá 4 rủi ro và thiết lập ngưỡng dừng | Ra quyết định Go (phạm vi hẹp / pilot workflow) |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Mở rộng góc nhìn tìm thêm bài toán sau khi đã tự scan | Gợi ý bối cảnh gán nhãn dataset và tóm tắt action item sau cuộc họp | Đưa ra ý tưởng quá rộng như "AI tự code toàn bộ bài lab", vi phạm nguyên tắc problem-first | Bỏ các ý giải pháp trá hình, chỉ giữ lại ý có quy trình đo được và viết lại theo trải nghiệm thật |
| CP2 Problem Card | Đóng vai PM hoài nghi để phản biện Card #1 | Bắt bẻ success metric ban đầu ("không bị trừ điểm") là mong muốn gián tiếp, khó đo lường | Gợi ý đẩy lên mức Agent tự động sửa bài nộp (quá rủi ro và vi phạm liêm chính học thuật) | Tự sửa metric thành "Thời gian đối soát giảm từ 60' xuống < 20'" và giữ vững mức can thiệp là Workflow |
| CP4 Research | Tìm kiếm các công cụ tương tự trên thị trường | Liệt kê nhanh các công cụ như Markdownlint, Super-Linter và Turnitin Rubrics | AI nhận định hời hợt rằng Turnitin có thể tích hợp rà soát repo Git của sinh viên trước khi nộp | Tự kiểm tra lại và phát hiện Turnitin chỉ dành cho giảng viên chấm sau khi nộp, bài toán của nhóm vẫn là một khoảng trống thị trường lớn |
| CP5 Quy trình | Định dạng sơ đồ luồng quy trình ASCII và bảng so sánh Before/After | Tính toán chi tiết thời gian tiết kiệm (từ 60' xuống 17', giảm 71.6%) | AI gợi ý quy trình tự động hóa hoàn toàn, bỏ qua bước con người kiểm tra (HITL) | Tự bổ sung bước sinh viên duyệt lại các mục cảnh báo và bắt buộc phải có phương án quay về (Fallback Plan) |
| CP5–6 Problem Statement | Rà soát các trường trong Problem Statement và gợi ý câu hỏi Google PAIR | Giúp phân tích sâu câu hỏi "Báo nhầm hay Bỏ sót tệ hơn" và gợi ý cấu trúc 10 test cases eval | AI cho rằng "bỏ sót" tệ hơn "báo nhầm" theo góc nhìn lý thuyết chung | Nhóm tự phản bác: trong bối cảnh sát deadline 30 phút, "báo nhầm" (False Positive) tệ hơn rất nhiều vì gây hoảng loạn sửa sai bài làm; từ đó đưa chỉ số False Positive $\le 10\%$ vào Success Metric |
| CP6 Mức can thiệp / quyết định | Tham khảo khung 4 rủi ro Marty Cagan | Giúp nhóm hệ thống hóa 4 khía cạnh Value, Usability, Feasibility, Viability | AI khuyến khích xây dựng hệ thống Agent thông minh đa tác tử | Nhóm từ chối Agent vì bài toán chỉ có độ phức tạp thấp, kiên quyết chọn mức Workflow và đặt ngưỡng dừng đo lường cụ thể |

---

## 6. Reflection (CP7)

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Khi nghe Long trình bày về các vấn đề trong làm việc nhóm kỹ thuật (như phân chia task trên Git và setup môi trường demo), tôi nhận ra không phải mọi khó khăn trong quy trình đều phù hợp để giải quyết bằng AI. Những vấn đề như xung đột code chủ yếu xuất phát từ việc thiếu thống nhất quy ước giữa các thành viên. Một bài toán tốt để đưa vào lab cần có quy trình lặp lại rõ ràng, dữ liệu đầu vào ổn định và có thể đo lường thời gian trước/sau một cách độc lập.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có. Ngay khi bắt đầu, cả tôi và Long đều nghĩ ngay đến việc xây dựng một "AI Agent tự động sửa file bài nộp markdown theo rubric". Nhóm chỉ nhận ra mình đang bị cuốn vào giải pháp khi bắt tay vào vẽ cây Opportunity Solution Tree (OST) và không thể định nghĩa được người dùng thực sự gặp khó ở bước nào trong quy trình hiện tại. Việc đối chiếu với quy định trong RULES.md và nhận thức về rủi ro vi phạm tính liêm chính học thuật đã giúp nhóm dừng lại, loại bỏ ý tưởng chatbot tự động để quay về tập trung vào bước nghẽn đọc đối chiếu thủ công.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Tôi đã đổi ý về vai trò của AI trong giải pháp. Ban đầu, tôi đề xuất để AI trực tiếp đưa ra kết luận bài nộp "Đạt" hay "Chưa đạt". Long đã phản biện rằng Rubric môn học có nhiều tiêu chí định tính, AI rất dễ đưa ra đánh giá không nhất quán hoặc ảo giác (hallucination). Tôi đồng ý với lập luận này và thay đổi hoàn toàn thiết kế: đưa bài toán về mức Workflow bán thủ công, trong đó Rule xử lý các lỗi định dạng cơ học, AI chỉ làm nhiệm vụ trích xuất dẫn chứng kèm số dòng, còn việc đánh giá và chỉnh sửa nội dung vẫn do sinh viên tự thực hiện.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Điều làm tôi bất ngờ nhất là kết quả khảo sát 22 sinh viên cho thấy nỗi sợ lớn nhất không phải là công cụ thiếu tính năng, mà là rủi ro "báo nhầm" (False Positive). Trước giờ nộp bài, việc công cụ cảnh báo sai một tiêu chí sẽ khiến sinh viên hoang mang và tốn thêm thời gian kiểm tra lại. Bằng chứng này đã làm thay đổi nhận thức của nhóm, giúp nhóm đặt tiêu chí an toàn (chống báo nhầm) lên ưu tiên hàng đầu thay vì cố gắng tự động hóa toàn bộ.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Khó nhất là lượng hóa Success Metric và xác định ranh giới (Boundary). Ban đầu, nhóm đặt mục tiêu chung chung là "giúp sinh viên không bị trừ điểm". Sau khi phân tích, nhóm nhận ra điểm số là kết quả gián tiếp phụ thuộc vào người chấm. Việc phải tách bạch để tìm ra metric đo lường trực tiếp (giảm thời gian rà soát từ 60 phút xuống dưới 20 phút và đạt tỷ lệ phát hiện thiếu sót trên 90%) đòi hỏi nhóm phải suy nghĩ rất kỹ về năng lực thực tế của công cụ.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu làm lại, tôi sẽ tiến hành kiểm chứng giả định với người dùng sớm hơn ngay từ CP3 thay vì đợi đến CP4. Việc có số liệu khảo sát thực tế sớm sẽ giúp nhóm tiết kiệm nhiều thời gian thảo luận giả định và chọn candidate problem nhanh hơn.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình:
Bài toán của nhóm là sinh viên mất từ 45 đến 60 phút đọc đối chiếu thủ công và hay bị trừ điểm oan do sót lỗi cấu trúc trước deadline (**Problem**). Nhóm thiết kế lại quy trình 4 bước gồm Rule quét định dạng cơ học và LLM trích xuất bảng đối chiếu dẫn chứng (**Quy trình**). Hiệu quả được đo bằng việc rút ngắn thời gian xuống dưới 20 phút và đạt tỷ lệ phát hiện đúng lỗi thiếu sót trên 90% (**Metric**). Ranh giới an toàn là AI không được sửa nội dung hay tự ý nộp bài, sinh viên bắt buộc phải tự duyệt và sửa bài làm (**Boundary**). Do bài toán có độ phức tạp thấp và quy trình tuần tự cố định, nhóm chọn mức can thiệp là Workflow bán thủ công (**Mức can thiệp AI**). Nhóm đưa ra quyết định GO với phạm vi pilot nhỏ, kèm ngưỡng dừng nếu tỷ lệ báo nhầm vượt quá 20% sẽ quay về quy trình thủ công (**Quyết định**).

---

## 7. Tài liệu tham khảo

1. Design Council (UK). *The Double Diamond Model in Design Thinking*. [designcouncil.org.uk](https://www.designcouncil.org.uk)
2. Rob Fitzpatrick. *The Mom Test: How to talk to customers & learn if your business is a good idea when everyone is lying to you*.
3. Teresa Torres. *Continuous Discovery Habits: Opportunity Solution Tree*. [producttalk.org](https://www.producttalk.org)
4. Marty Cagan. *Inspired: How to Create Tech Products Customers Love* (4 Product Risks).
5. Google PAIR. *People + AI Guidebook* (Augment vs Automate, Designing for Errors). [pair.withgoogle.com](https://pair.withgoogle.com)
