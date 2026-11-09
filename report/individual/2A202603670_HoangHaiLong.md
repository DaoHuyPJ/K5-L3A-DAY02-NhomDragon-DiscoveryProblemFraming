# Báo cáo cá nhân — 2A202603670_HoangHaiLong

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Hoàng Hải Long
- MSSV: 2A202603670
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: NhomDragon
- Link repo nhóm:https://github.com/DaoHuyPJ/K5-L3-Day02-NhomDragon-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Nhân vật: Chị Mai, mới có bằng lái, tự lái xe mới của mình đi lại hằng ngày, hay gặp khó khi lùi xe và đỗ chỗ hẹp.
Bối cảnh giả định (cần xác nhận): sống ở chung cư, đỗ xe dưới hầm, đi làm 5 ngày/tuần. Số có dấu ~ là ước lượng, chưa đo thật.

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi về nhà và phải lùi vào ô hẹp giữa hai xe, tôi muốn biết lúc nào cần đánh lái, để vào ô ngay mà không chạm xe bên cạnh | Chị Mai, chủ xe hai bên | ~10 phút/lần, tiến lùi 4–5 lần, 5 lần/tuần |
| 2 | Lặp lại | Khi phải lùi ra khỏi ngõ hẹp, tôi muốn giữ xe đi thẳng, để không quẹt tường | Chị Mai | ~6 phút/lần, 2 lần/tuần |
| 3 | Tốn thời gian | Khi sắp đến một nơi lạ, tôi muốn biết chỗ đó có chỗ đỗ dễ vào không, để quyết định lái xe đi hay gọi taxi | Chị Mai | ~15 phút vòng tìm chỗ/lần; ~2 chuyến/tuần bỏ xe, gọi taxi |
| 4 | Tốn thời gian | Khi chỉ còn chỗ đỗ sát lề đường, tôi muốn biết xe mình có vừa không, để khỏi loay hoay giữa đường | Chị Mai, xe phía sau | ~3/5 lần bỏ cuộc, đi tìm chỗ khác |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi lùi xe mà phải nhìn cùng lúc camera, hai gương và nghe tiếng cảm biến, tôi muốn biết nên tin tín hiệu nào, để không bị rối | Chị Mai | 4 nguồn tín hiệu; ~2–3 lần dừng lại vì rối mỗi lần lùi |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi tự luyện đỗ xe, tôi muốn có cách làm đúng với xe của mình, để không phải đoán mình sai ở đâu | Chị Mai | ~10 video đã xem, ~160 phút/buổi tập, ~6 buổi vẫn chưa đỗ chắc |
| 7 | Pain từ người khác | Khi không tự đỗ được, tôi muốn xử lý xong mà không cần nhờ ai, để người thân và bảo vệ không phải ra đỗ hộ | Người thân, bảo vệ | ~2–3 lần nhờ/tuần, ~5 phút/lần |
| 8 | Pain từ người khác | Khi lùi xe mà xe sau chờ và bóp còi, tôi muốn giữ bình tĩnh, để không đánh lái sai | Chị Mai, xe phía sau | ~1–2 lần/tuần |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Bỏ "Cần app hướng dẫn đỗ xe": đây là giải pháp trá hình, không phải problem.
- Bỏ "Tôi sợ lái xe": quá rộng, không vẽ được quy trình.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Lùi vào ô hẹp ở nhà (#1) | Xảy ra mỗi ngày, dễ bấm giờ | Xe đã có camera, vậy chị thiếu thông tin hay thiếu kỹ năng? |
| 2 | Đỗ xe ở nơi lạ (#3) | Có hành vi rõ: có xe mà vẫn gọi taxi | Có dữ liệu về chỗ đỗ không? |
| 3 | Tự luyện đỗ xe (#6) | Không phải làm lúc đang lái, an toàn hơn | Chị có chịu luyện đều không? |

### Problem Card #1 — Lùi vào ô hẹp ở nhà

| Trường | Nội dung |
|---|---|
| Job Story | Khi về nhà và phải lùi vào ô hẹp giữa hai xe, tôi muốn biết lúc nào cần đánh lái, để vào ô ngay mà không chạm xe bên cạnh |
| Actor | Người mới lái dưới 1 năm, tự lái xe riêng, đỗ ở hầm chung cư |
| Thời điểm / bối cảnh | Chiều tối đi làm về, hầm đông, ô hẹp, ánh sáng yếu |
| Quy trình hiện tại (3–7 bước) | 1. Tìm ô trống · 2. Căn vị trí bắt đầu · 3. Lùi vào ô, canh lúc đánh lái · 4. Tiến lùi chỉnh cho thẳng · 5. Xuống xe kiểm tra |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, canh lúc đánh lái: ~5 phút, phải tiến lùi 4–5 lần |
| Impact (nếu không giải thì sao) | ~50 phút/tuần; ~1 lần chạm xước/2 tháng, ~2 triệu/lần sửa |
| Success metric (baseline → target) | Thời gian đỗ ~10 → dưới 4 phút; tiến lùi 4–5 → tối đa 1 lần; 0 lần chạm xước trong 4 tuần. Đo bằng bấm giờ và tự ghi lại mỗi lần đỗ |
| Phương án không dùng AI | Học thầy 2–3 buổi; dán mốc căn trên gương; xin ô cố định, ô rộng ở hầm |
| Giả thuyết về AI (nếu có) | Nhìn hình camera và gợi ý thời điểm đánh lái. Chỉ gợi ý, không điều khiển xe, người lái luôn tự quyết |
| Cảm nhận nhanh | Chưa biết (nghiêng về No AI) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~10 phút/lần

[1 Tìm ô trống: 1'] → [2 Căn vị trí bắt đầu: 1']
→ [3 Lùi vào ô, canh lúc đánh lái: 5'] ← BOTTLENECK
→ [4 Tiến lùi chỉnh cho thẳng: 2'] → [5 Xuống xe kiểm tra: 1']
```

### Problem Card #2 — Đỗ xe ở nơi lạ

| Trường | Nội dung |
|---|---|
| Job Story | Khi sắp đến một nơi lạ, tôi muốn biết chỗ đó có chỗ đỗ dễ vào không, để quyết định lái xe đi hay gọi taxi |
| Actor | Người mới lái dưới 1 năm, đi đến nơi chưa từng đỗ xe |
| Thời điểm / bối cảnh | Đi gặp khách, đi khám bệnh, đi ăn ở khu đông, cuối tuần |
| Quy trình hiện tại (3–7 bước) | 1. Tra bản đồ, hỏi bạn về chỗ đỗ · 2. Đến nơi, vòng tìm chỗ dễ vào · 3. Thử đỗ, khó thì bỏ · 4. Đi bộ đến nơi |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2, vòng tìm chỗ dễ vào: ~15 phút |
| Impact (nếu không giải thì sao) | ~30 phút/lần; ~2 chuyến/tuần bỏ xe gọi taxi, ~100k/chuyến, ~800k/tháng |
| Success metric (baseline → target) | Vòng tìm chỗ ~15 → dưới 5 phút; bỏ xe ~2 → tối đa 1 chuyến/tuần. Đo bằng tự ghi lại mỗi chuyến trong 4 tuần |
| Phương án không dùng AI | Lưu sẵn danh sách bãi rộng, dễ vào; xem trước ảnh đường phố; ưu tiên hầm trung tâm thương mại |
| Giả thuyết về AI (nếu có) | Tổng hợp ảnh và đánh giá thành "chỗ này dễ đỗ không". Người lái tự chọn |
| Cảm nhận nhanh | Rule hoặc Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~30 phút/lần

[1 Tra bản đồ, hỏi bạn: 5'] → [2 Vòng tìm chỗ dễ vào: 15'] ← BOTTLENECK
→ [3 Thử đỗ, khó thì bỏ: 5'] → [4 Đi bộ đến nơi: 5']
```

### Problem Card #3 — Tự luyện đỗ xe

| Trường | Nội dung |
|---|---|
| Job Story | Khi tự luyện đỗ xe, tôi muốn có cách làm đúng với xe của mình, để không phải đoán mình sai ở đâu |
| Actor | Người mới lái dưới 1 năm, muốn tự tin đỗ xe mà chưa học thêm |
| Thời điểm / bối cảnh | Cuối tuần, ở bãi trống, tập một mình |
| Quy trình hiện tại (3–7 bước) | 1. Tìm video · 2. Xem và ghi nhớ · 3. Đi đến bãi trống · 4. Tập và tự đoán mình sai ở đâu · 5. Ghi lại kinh nghiệm |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4, tập và tự đoán mình sai ở đâu: ~60 phút, không ai chỉ lỗi |
| Impact (nếu không giải thì sao) | ~160 phút/buổi; ~6 buổi vẫn chưa đỗ chắc, nên pain ở card #1 kéo dài |
| Success metric (baseline → target) | Số buổi để đỗ đúng 3/3 lần vào ô hẹp: ~6 buổi chưa đạt → tối đa 3 buổi. Đo bằng cọc tiêu và ghi kết quả mỗi buổi |
| Phương án không dùng AI | Thuê thầy 2–3 buổi; nhờ người thân quay video và chỉ lỗi; dùng cọc tiêu tạo ô tập |
| Giả thuyết về AI (nếu có) | Xem video buổi tập, chỉ ra lỗi lặp lại và gợi ý bài tiếp theo. Chỉ dùng sau buổi tập, không dùng khi đang lái |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~160 phút/buổi

[1 Tìm video: 30'] → [2 Xem, ghi nhớ: 45'] → [3 Đi đến bãi trống: 20']
→ [4 Tập, tự đoán lỗi: 60'] ← BOTTLENECK → [5 Ghi lại kinh nghiệm: 5']
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Pain lặp lại mỗi ngày, bước nghẽn rõ, dễ đo.
- Câu hỏi muốn nhóm phản biện: Xe đã có camera và cảm biến, vậy chị Mai thiếu thông tin hay thiếu kỹ năng? Nếu thiếu kỹ năng thì card #3 có phải bài đúng hơn không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Mọi con số mới là ước lượng | Đồng ý | Gắn dấu ~ và ghi cách đo. Vẫn cần đo thật |
| Xe mới thường đã có camera, bottleneck "không nhìn rõ" chưa đúng | Đồng ý | Đổi bottleneck #1 thành "canh lúc đánh lái" |
| Metric chỉ đo tốc độ, đỗ nhanh mà vẫn quẹt thì sao? | Đồng ý | Thêm "0 lần chạm xước" và số lần tiến lùi |
| Gợi ý lúc đang lùi xe có thể gây phân tâm, sai là va chạm | Đồng ý | Ghi rõ chỉ gợi ý, không điều khiển xe; card #1 nghiêng về No AI |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch Card #1 (Đối soát rubric bài lab kỹ thuật), nêu rõ bối cảnh trước deadline 2 tiếng và bước nghẽn đọc đối chiếu chi tiết (20–25') | Thống nhất chọn làm Candidate Problem chính cho cả bài lab
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt cho Huy: (1) "Rubric có tiêu chí định tính (ví dụ 'lập luận chặt') thì đối soát tự động kiểu gì mà không bị hallucinate?" (2) "Lỗi lạ trên máy cá nhân mỗi người một kiểu, dữ liệu tìm kiếm phân mảnh thì làm sao đảm bảo giải pháp đưa ra chạy được?" (3) "Nếu commit message viết ẩu kiểu 'fix bug', 'update' thì lấy thông tin đâu ra để viết narrative?" *(nguồn: bảng pitch trong group_report.md mục 2.1)* | Huy sửa thiết kế: Rule xử lý format, AI chỉ trích dẫn đoạn liên quan, người duyệt và sửa (HITL) thay vì để AI kết luận Đạt/Chưa đạt |
| Nhận phản biện | Câu hỏi tôi nhận được từ Huy: (1) "Merge conflict là vấn đề kỷ luật git và giao tiếp nhóm, công nghệ có can thiệp được tận gốc không?" (2) "Docker hoặc requirements.txt chuẩn đã giải quyết việc setup demo rồi, bài toán đó có cần thiết kế mới không?" *(nguồn: báo cáo cá nhân của Huy, mục 4)* | Tôi đã làm gì: (1) Chia việc theo file để tránh conflict (2) Loại candidate này vì chưa chưa chắc cần |
| Gom cluster / cây OST | Cùng Huy gom 5 candidate thành 3 cụm: A (chất lượng và tuân thủ khi nộp bài), B (tìm kiếm và debug), C (cộng tác nhóm và báo cáo). Cây OST có 1 outcome: giảm 70% thời gian rà soát bài nộp mà không bị trừ điểm oan | Các ý như chatbot tự sửa bài, tool tự sinh code, script tự commit bị gạch vì là giải pháp đội lốt opportunity (group_report mục 2.2–2.3) |
| Chọn candidate problem | Tôi băn khoăn liệu đối soát tự động có xử lý được tiêu chí định tính của rubric không; nhóm chốt: Rule lo format, AI chỉ trích dẫn, người quyết định, và tôi đồng thuận *(nguồn: group_report mục 2.4 "Xử lý bất đồng")* | Nhóm chọn candidate #1 (đối soát rubric, 35/35) và loại hai candidate còn lại |
| Kiểm chứng / research | Cùng nhóm chốt kiểm chứng giả định #2 (mất điểm oan vì lỗi format) và #3 (sợ báo nhầm), bằng khảo sát 22 người và 3 buổi phỏng vấn; research 3 công cụ: Markdownlint, Turnitin Rubrics, ChatGPT/Claude tự do. *(nguồn: group_report mục 3. Bạn tự điền thêm phần bạn trực tiếp làm)* | Nhóm thu hẹp từ "công cụ đánh giá toàn diện" thành quy trình 2 tầng: Rule quét format, AI chỉ trích dẫn để người xác nhận |
| Quy trình nhóm | Cùng nhóm chốt quy trình hiện tại 5 bước, 60 phút, bottleneck là bước đọc đối chiếu (20–25'); quy trình tương lai 4 bước, khoảng 17 phút, có Rule, AI, người duyệt và phương án quay về (checklist tick tay 15') | Giảm khoảng 71.6% thời gian theo ước tính của nhóm (group_report mục 4) |
| Problem Statement | Cùng nhóm chốt v0 (6 trường) rồi nâng lên v1, thêm tỷ lệ báo nhầm không quá 10%, điểm chen của AI, mức chọn, rủi ro và người kiểm tra | Metric chuyển từ "không bị trừ điểm" sang chỉ số đo trực tiếp công cụ (group_report mục 5 và 7) |
| Mức can thiệp AI | Cùng nhóm chốt Workflow bán thủ công: loại No AI vì không bớt bước đọc, loại thuần Rule vì không hiểu ngữ nghĩa, loại Agent vì rủi ro sửa hỏng bài và vi phạm liêm chính học thuật | AI Canvas: Prediction là bảng đối soát 3 cột; PAIR: người dùng muốn augment, báo nhầm tệ hơn bỏ sót (group_report mục 6) |
| Quyết định | Cùng nhóm chốt Go phạm vi hẹp: pilot ngay trên bài lab Day 02, ngưỡng dừng là báo nhầm trên 20% hoặc kiểm lại cảnh báo trên 25 phút thì quay về Rule và checklist thủ công | Cả 4 rủi ro Value, Usability, Feasibility, Viability được chấm Thấp (group_report mục 8) |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Nhờ AI viết bản nháp toàn bộ bảng scan 8 problem về chị Mai | Chia đúng 4 lăng kính, viết đúng dạng Job Story | Toàn bộ con số (phút, tần suất, tiền) và bối cảnh (chung cư, hầm xe, đi làm 5 ngày/tuần) là AI tự ước lượng, không phải dấu hiệu thật | Tôi nhận thấy AI thêm phần đỗ xe ở chung cư khá hợp lý |
| CP2 Problem Card | Nhờ AI viết 3 card và tự phản biện card #1 | Chỉ ra bottleneck #1 chưa đúng (xe mới đã có camera), metric thiếu chất lượng, gợi ý lúc đang lùi xe có thể gây va chạm | Cột "Đồng ý?" trong bảng phản biện do AI điền thay tôi; gợi ý xe tự đỗ nhưng chưa kiểm chứng xe của chị Mai có sẵn tính năng này không | Tôi gợi ý rằng xe tự đỗ |
| CP4 Research | Dùng AI để tra cứu các công cụ giống với dự án | Gom nhanh được 2 giả định, các nguồn kiểm chứng và 3 công cụ đã research vào một dòng dễ đọc | AI hời hợt về các tool đã tìm kiếm | Kiểm tra lại các tool |
| CP5 Quy trình | Nhờ AI tóm tắt quy trình trước/sau của nhóm | Tóm gọn 5 bước còn 4 bước, nêu rõ bước Rule, AI và người duyệt | AI gợi ý tự động | Có xác nhận cuối của người dùng  |
| CP5–6 Problem Statement | Nhờ AI giải thích persona, problem statement, triệu chứng và gốc rễ của dự án Huy đề xuất | Tách được triệu chứng với gốc rễ và chỉ ra phần lớn lỗi format chỉ cần Rule | Phần gốc rễ là AI tự suy ra từ tài liệu, không phải nhóm đã viết trong báo cáo | Đúng với bài làm của nhóm |
| CP6 Mức can thiệp / quyết định | Nhờ AI tóm tắt mức can thiệp và quyết định Go của nhóm | Tóm đúng lý do loại No AI, Rule thuần và Agent, cùng ngưỡng dừng | AI chỉ chép lại kết luận của nhóm, không tự kiểm lại việc chấm cả 4 rủi ro đều "Thấp" có quá lạc quan không | *(bạn tự điền)* |
| CP7 Reflection (bản nháp) | Nhờ AI viết bản nháp mục 6.1–6.7 dựa trên tài liệu nhóm | Có sẵn khung 6 câu trả lời và chuỗi giải thích bài nhóm | Bản nháp dựa vào tài liệu, không phải trải nghiệm thật của tôi; các chỗ đánh dấu là chỗ AI không biết tôi đã làm gì | Có sửa lại theo ý cá nhân |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Từ ba problem của Huy (đối soát rubric, tìm lỗi thư viện, tổng hợp báo cáo tiến độ từ git), tôi thấy rõ nỗi đau của sinh viên hiện tại, và dự án khả thi để có thể thực hiện.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có. Theo ghi chép của Huy, lúc đầu nhóm nghĩ ngay tới một "AI Agent tự sửa file bài nộp theo rubric". Nhóm gạch các ý như chatbot tự sửa bài và quay về bước nghẽn thật là đọc đối chiếu rubric.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Huy có hỏi về vấn đề merge conflict và tôi đề xuất thực hiện theo quy ước nhóm, ai làm phần nào và Huy cũng thống nhất với ý kiến của tôi. 

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Theo báo cáo nhóm của tôi, 22 người được hỏi sợ nhất là AI "báo nhầm" sát giờ nộp, gây hoang mang.  

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Khó nhất là viết Success Metric có đủ baseline, target và cách đo. Ban đầu nhóm ghi "không bị trừ điểm", nhưng đó là kết quả gián tiếp, phụ thuộc người chấm và việc sinh viên có chịu sửa hay không.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Tôi sẽ đo thời gian thật và hỏi người thật ngay từ CP1, thay vì viết con số ước lượng rồi mới thấy cần kiểm chứng. Tôi sẽ phản biện nhóm mạnh hơn hai điểm. Thứ nhất, baseline 60 phút lấy từ đâu và đã bấm giờ mấy lần. Thứ hai, ngưỡng báo nhầm không quá 10% sẽ đo bằng bộ dữ liệu nào khi chưa có công cụ chạy thật.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
Sinh viên nộp bài lab tốn nhiều thời gian đọc đối chiếu rubric với file bài làm, và nhiều bạn vẫn bị trừ điểm oan vì sót lỗi cấu trúc. Quy trình là Rule quét format, AI trích xuất bảng đối soát có trích dẫn, người duyệt và sửa, rồi tự nộp. Success metric đo bằng thời gian trong khoảng 20 phút là đạt, phát hiện đúng thiếu sót từ 90% trở lên và báo nhầm không quá 10%. AI không được sửa file, không được commit hay nộp bài, và mọi cảnh báo đều do người duyệt. Nếu tỷ lệ báo lỗi nhầm vượt quá 20% thì quay về quy trình duyệt đối soát thủ công

---

## 7. Tài liệu tham khảo

1. Design Council (UK). *The Double Diamond Model in Design Thinking*. https://www.designcouncil.org.uk
2. Rob Fitzpatrick. *The Mom Test*.
3. Teresa Torres. *Continuous Discovery Habits: Opportunity Solution Tree*. https://www.producttalk.org
4. Marty Cagan. *Inspired* (4 Product Risks).
5. Google PAIR. *People + AI Guidebook*. https://pair.withgoogle.com
6. Báo cáo nhóm: `report/team/group_report.md`.
