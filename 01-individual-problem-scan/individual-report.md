# 01 — Individual Problem Scan

> Bối cảnh cá nhân: Sinh viên năm cuối vừa học vừa đi thực tập. Công việc hằng tuần gồm: làm bài tập và dự án nhóm ở trường, họp nhóm thường xuyên, xử lý data và xây dựng dự án công ty và đồ án. Hầu hết các vấn đề đều xuất phát từ trải nghiệm học tập và đi làm thực tế.

---

## Phase 1 — Bảng Scan (8 problems)

| # | Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Tốn thời gian | Mỗi lần bắt đầu sprint hoặc bài tập mới, phải đọc 20-40 trang tài liệu hướng dẫn / paper / PRD để hiểu đủ context trước khi làm | Sinh viên, intern | Mỗi lần đọc mất 45-90 phút, vẫn không chắc mình hiểu đúng phần quan trọng |
| 2 | Lặp lại | Sau mỗi buổi họp nhóm / standup, phải tự ghi lại meeting notes, action items và deadline rồi chia sẻ cho cả team | Các thành viên nhóm | Lặp lại mỗi tuần 2-3 buổi, tốn 20-30 phút/lần, hay bị bỏ sót action item |
| 3 | Lặp lại | Khi làm dự án nhóm, phải tổng hợp kết quả làm việc của từng thành viên vào một báo cáo chung mỗi tuần | Trưởng nhóm, thành viên phụ trách tổng hợp | Mỗi lần tổng hợp mất 60-90 phút vì format khác nhau, thiếu thông tin, phải hỏi lại |
| 4 | AI có thể tốt hơn | Khi phân tích data, phải tự viết code EDA từ đầu cho mỗi dataset mới trong khi nhiều bước là lặp lại (load, check null, plot distribution) | Intern data, sinh viên làm project | Mỗi dataset mất 1-2 giờ setup lại từ đầu dù bước cơ bản giống nhau |
| 5 | Pain từ người khác | Thành viên trong nhóm hay hỏi lại "deadline là lúc mấy giờ", "link file mới nhất ở đâu", "ai làm phần nào" — những thông tin đã có trong nhóm nhưng bị chôn trong chat | Cả nhóm | Xảy ra 3-5 lần/tuần trên Discord/Zalo, làm chậm tiến độ |
| 6 | Tốn thời gian | Khi cần review lại quyết định cũ (tại sao chọn model này, tại sao thay đổi approach), phải tìm lại trong message Discord / Google Doc cũ rất mất công | Cả nhóm, mentor | 15-20 phút/lần tìm kiếm, đôi khi không tìm được |
| 7 | AI có thể tốt hơn | Khi viết báo cáo kết quả thực nghiệm, phải tự tóm tắt các con số từ nhiều file log/Excel thành phần narrative giải thích kết quả cho người đọc hiểu | Intern, sinh viên làm thesis | Phần viết narrative mất 30-45 phút, hay bị blank page |
| 8 | Pain từ người khác | Mentor / giảng viên gửi feedback dưới dạng comment rải rác trong nhiều file khác nhau; sinh viên phải tự tổng hợp, hiểu ý và sửa — không biết mình đã sửa đủ chưa | Sinh viên, intern | Hay bị sót feedback, phải hỏi lại "anh/chị muốn mình sửa chỗ nào nữa không?" |

---

## Phase 2 — Top 3 Problem Cards

### Bảng chọn Top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Đọc/tổng hợp tài liệu dài trước khi làm task (Problem #1) | Xảy ra đều đặn, tốn nhiều thời gian nhất, rõ bottleneck, có thể đo bằng thời gian | "Hiểu đủ" nghĩa là gì? Metric quality khó đo |
| 2 | Tổng hợp báo cáo nhóm hằng tuần (Problem #3) | Workflow rõ, nhiều người đồng cảm, impact đo được, có thể so sánh Rule / Workflow / Agent | Phụ thuộc từng nhóm, format khác nhau |
| 3 | Tổng hợp feedback từ nhiều file (Problem #8) | Pain rõ, người gặp cụ thể, workflow có thể vẽ | Quyền truy cập file phức tạp nếu dùng tool |

---

## Problem Card #1 — Đọc tài liệu dài trước khi bắt đầu task

**Problem 1 câu:**
Sinh viên / intern mỗi khi nhận task mới phải đọc 20-40 trang tài liệu để nắm context, mất 45-90 phút nhưng vẫn không chắc đã hiểu đúng phần quan trọng, dẫn đến làm sai hướng hoặc phải đọc lại.

**Actor:**
Sinh viên năm 3-4 đang làm dự án / intern tại công ty tech, có nhiệm vụ đọc hiểu tài liệu kỹ thuật (paper, PRD, spec, hướng dẫn dự án) trước khi bắt đầu implement.

**Thời điểm / bối cảnh:**
Đầu mỗi sprint hoặc khi nhận task mới; thường xảy ra 1-2 lần/tuần.

**Current workflow:**

```text
1. Nhận task + link tài liệu từ mentor/leader
2. Mở tài liệu (20-40 trang) đọc từ đầu đến cuối
3. Ghi chú thủ công những điểm quan trọng (vào notebook hoặc file riêng)
4. Tự đoán phần nào liên quan đến task của mình
5. Hỏi mentor những điểm chưa hiểu
6. Bắt đầu làm
```

**Bottleneck:**
Bước 2 → 4: đọc toàn bộ tài liệu để tìm phần liên quan đến task — mất 45-90 phút vì tài liệu không có cấu trúc rõ ràng theo task, và sinh viên chưa biết phần nào quan trọng cho mình.

**Impact:**
45-90 phút/task × 2 lần/tuần = 90-180 phút/tuần chỉ để đọc hiểu context. Nếu đọc sai trọng tâm → làm sai hướng → phải làm lại, mất thêm thời gian.

**Success metric:**
Giảm thời gian đọc/nắm context từ 45-90 phút xuống dưới 20 phút; số lần phải hỏi lại mentor vì "không hiểu tài liệu" giảm từ 2-3 lần/task xuống dưới 1 lần.

**Non-AI alternative:**
- Mentor/leader viết TL;DR đầu mỗi tài liệu (chỉ giải quyết được nếu mentor có thời gian)
- Wiki nội bộ tổng hợp key points (tốn công duy trì, dễ lỗi thời)

**AI hypothesis:**
AI đọc tài liệu dài → trích xuất các phần liên quan đến task cụ thể → tóm tắt theo cấu trúc rõ (context, yêu cầu, điểm cần chú ý) → sinh viên đọc bản tóm tắt và hỏi AI để làm rõ trước khi bắt tay làm.

**Quick gut:**
- [x] Workflow

---

### Draft Workflow #1

```text
CURRENT STATE — 6 bước, khoảng 60-90 phút/task

[1 Nhận task + link tài liệu: 5']
→ [2 Đọc toàn bộ tài liệu 20-40 trang: 45-90']  <-- bottleneck chính
→ [3 Ghi chú thủ công: 10']
→ [4 Tự đoán phần liên quan: 5']
→ [5 Hỏi mentor điểm chưa hiểu: 10']
→ [6 Bắt đầu làm: --]

FUTURE STATE — 5 bước, khoảng 20-25 phút/task

[1 Nhận task + link tài liệu: 5']
→ [2 AI đọc & tóm tắt theo task context: 1']        -- Workflow step
→ [3 Sinh viên đọc bản tóm tắt + hỏi AI làm rõ: 10']  -- Human + AI
→ [4 Hỏi mentor (nếu còn điểm chưa chắc): 5']       -- Human boundary
→ [5 Bắt đầu làm: --]

Fallback: AI tóm tắt sai / bỏ sót phần quan trọng
→ Sinh viên quay lại đọc thẳng tài liệu gốc ở phần đó.
```

---

## Problem Card #2 — Tổng hợp báo cáo nhóm hằng tuần

**Problem 1 câu:**
Mỗi tuần người phụ trách tổng hợp phải gom kết quả từ 3-4 thành viên về một báo cáo chung, mất 60-90 phút vì format khác nhau, thông tin bị thiếu và phải hỏi lại nhiều lần.

**Actor:**
Trưởng nhóm hoặc thành viên được phân công tổng hợp báo cáo tiến độ dự án cho nhóm 3-5 người.

**Thời điểm / bối cảnh:**
Cuối tuần (thứ Sáu / Chủ Nhật) trước khi nộp báo cáo tiến độ cho giảng viên / mentor.

**Current workflow:**

```text
1. Nhắn từng thành viên nộp phần của mình
2. Chờ thành viên nộp (hay bị trễ, phải nhắc nhiều lần)
3. Nhận file/text từ nhiều nguồn (Google Doc, Zalo, Discord, file Word rời)
4. Copy-paste thủ công vào file tổng hợp
5. Chuẩn hóa format (font, heading, cách trình bày)
6. Đọc lại, điền những phần thiếu, hỏi lại thành viên
7. Viết phần tóm tắt / executive summary cho cả nhóm
8. Gửi báo cáo cuối
```

**Bottleneck:**
Bước 4-7: tổng hợp, chuẩn hóa và viết phần tóm tắt — mỗi lần mất 60-90 phút vì thông tin đến từ nhiều nơi, format khác nhau, và viết phần tóm tắt cần đọc hiểu toàn bộ rồi mới viết được.

**Impact:**
60-90 phút/tuần cho người tổng hợp. Nếu có 3 dự án song song thì lên đến 3-4.5 giờ/tuần chỉ để tổng hợp. Báo cáo trễ → thiếu feedback từ mentor để cải tiến kịp.

**Success metric:**
Giảm thời gian tổng hợp từ 60-90 phút xuống dưới 25 phút; số lần phải hỏi lại thành viên vì thiếu thông tin giảm từ 3-5 lần xuống dưới 1 lần/tuần.

**Non-AI alternative:**
- Template bắt buộc mỗi thành viên điền theo đúng form → giảm bước chuẩn hóa
- Google Form thu thập thông tin có cấu trúc → vẫn phải viết tóm tắt thủ công

**AI hypothesis:**
Mỗi thành viên điền template chuẩn (Rule) → AI gom các phần lại, phát hiện thông tin thiếu và draft executive summary → người tổng hợp review + chỉnh sửa → gửi.

**Quick gut:**
- [x] Workflow (kết hợp Rule cho bước thu thập)

---

### Draft Workflow #2

```text
CURRENT STATE — 8 bước, khoảng 60-90 phút/tuần

[1 Nhắn thành viên nộp phần: 5']
→ [2 Chờ + nhắc lại: 10-20']  <-- chờ, không kiểm soát được
→ [3 Nhận file từ nhiều nguồn: 5']
→ [4 Copy-paste + gom lại: 15']
→ [5 Chuẩn hóa format: 15']  <-- bottleneck
→ [6 Điền thiếu + hỏi lại: 10']
→ [7 Viết executive summary: 15']  <-- bottleneck thứ hai
→ [8 Gửi: 5']

FUTURE STATE — 5 bước, khoảng 20-25 phút/tuần

[1 Thành viên điền template chuẩn (Google Form / Notion): 5']  -- Rule
→ [2 AI gom input, phát hiện thiếu sót và draft summary: 1']  -- Workflow
→ [3 Người tổng hợp review, chỉnh sửa: 15']                   -- Human boundary
→ [4 Hỏi lại thành viên nếu vẫn thiếu: 3']
→ [5 Gửi báo cáo: 2']

Fallback: AI draft summary sai/nhạt → người tổng hợp tự viết lại phần đó.
```

---

## Problem Card #3 — Tổng hợp feedback từ nhiều file/nguồn

**Problem 1 câu:**
Sau khi nộp bài / báo cáo, sinh viên nhận feedback rải rác ở nhiều nơi (comment trong file, email, chat) và không biết mình đã giải quyết đủ tất cả các điểm feedback chưa.

**Actor:**
Sinh viên / intern sau khi nộp bản draft (báo cáo, code, slide) và nhận feedback từ mentor hoặc giảng viên.

**Thời điểm / bối cảnh:**
Sau mỗi lần review / nộp bản draft — xảy ra 1-3 lần/tuần tùy giai đoạn dự án.

**Current workflow:**

```text
1. Nhận feedback từ nhiều nguồn (comment Google Doc, email, Zalo/Discord)
2. Tự đọc từng nguồn và ghi nhớ / ghi note những điểm cần sửa
3. Vào từng file để sửa
4. Tự đối chiếu lại xem đã sửa hết chưa
5. Hỏi lại mentor "anh/chị xem còn điểm nào cần sửa không?"
6. Nhận thêm feedback (nếu có) và lặp lại
```

**Bottleneck:**
Bước 2 + 4: tự đọc và tự đối chiếu feedback nhiều nguồn — hay bỏ sót, không biết feedback nào quan trọng hơn, và mất 15-25 phút chỉ để gom + đọc hiểu feedback trước khi sửa.

**Impact:**
15-25 phút gom feedback × 1-3 lần/tuần + rủi ro bỏ sót → phải hỏi lại → mất thêm thời gian, ảnh hưởng đến tiến độ và chất lượng bài nộp cuối.

**Success metric:**
Giảm thời gian gom + đọc hiểu feedback từ 15-25 phút xuống dưới 5 phút; số lần phải hỏi lại "còn sót gì không" giảm từ 2-3 lần/review xuống 0-1 lần.

**Non-AI alternative:**
- Mentor/giảng viên điền feedback vào 1 form chuẩn (không thực tế, không kiểm soát được phía mentor)
- Tự lập checklist sau mỗi lần đọc (có ích nhưng vẫn tốn thời gian đọc)

**AI hypothesis:**
Dán tất cả feedback từ nhiều nguồn vào một prompt → AI phân loại, tóm tắt và tạo checklist sửa có ưu tiên → sinh viên sửa theo checklist và đánh dấu done từng điểm.

**Quick gut:**
- [x] Workflow

---

### Draft Workflow #3

```text
CURRENT STATE — 6 bước, khoảng 30-45 phút/lần review

[1 Nhận feedback nhiều nguồn: 5']
→ [2 Đọc + ghi nhớ từng feedback: 15-25']  <-- bottleneck chính
→ [3 Vào file sửa: 10-20']
→ [4 Tự đối chiếu: 10']  <-- dễ bỏ sót
→ [5 Hỏi lại mentor: 5']
→ [6 Lặp lại nếu còn sót: --]

FUTURE STATE — 4 bước, khoảng 15-20 phút/lần review

[1 Copy toàn bộ feedback vào một chỗ: 3']
→ [2 AI phân loại + tóm tắt thành checklist ưu tiên: 1']  -- Workflow
→ [3 Sinh viên sửa theo checklist, đánh dấu done: 10-15'] -- Human làm chính
→ [4 Review nhanh checklist trước khi gửi lại: 2']        -- Human boundary

Fallback: AI bỏ sót feedback quan trọng → sinh viên đọc lại nguồn gốc để kiểm tra.
```

---

## Card muốn pitch nhất với nhóm

**Card tôi chọn để pitch:** Problem Card #1 — Đọc tài liệu dài trước khi bắt đầu task

**Vì sao:**

```text
- Workflow rõ nhất trong 3 card: có thể vẽ từng bước, biết bottleneck ở đâu.
- Metric đo được: thời gian đọc trước/sau, số lần hỏi lại mentor.
- Nhiều người trong nhóm khả năng cao cũng gặp — intern nào cũng phải đọc tài liệu.
- Có thể so sánh Rule / Workflow / Agent rõ ràng.
- Không quá rộng: chỉ tập trung vào bước "đọc hiểu context trước khi làm".
```

**Câu hỏi tôi muốn nhóm challenge:**

```text
1. "Baseline 45-90 phút có đúng không hay chỉ là ước đoán? Các bạn có trải nghiệm tương tự không?"
2. "Metric 'số lần hỏi lại mentor' có đo được trong thực tế không?"
3. "Có workflow nào không cần AI mà vẫn giải được 70-80% bài toán này không?"
4. "Nếu tài liệu có nội dung nhạy cảm (code nội bộ, data riêng tư), có thể paste vào AI không?"
```

---

## Tự kiểm Phase 1 & 2

- [x] Có 8 problems (vượt mức tối thiểu 5), dùng nhiều lăng kính khác nhau.
- [x] Mỗi problem có actor, lăng kính và dấu hiệu thật.
- [x] Top 3 Problem Cards điền đủ 9 field.
- [x] Có draft workflow trước/sau cho cả 3 card.
- [x] Ghi rõ card muốn pitch và câu hỏi muốn được challenge.
- [ ] Chưa pitch thật với nhóm (sẽ làm ở Phase 3 trong buổi học).
