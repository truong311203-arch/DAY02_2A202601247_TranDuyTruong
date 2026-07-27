# 03 — Individual Reflection

> Phase 7 — Reflection cá nhân sau buổi lab Day 02.
> Viết bằng trải nghiệm thật. Không dùng AI để viết thay phần này.

---

## Tôi đã tham gia vào phần nào?

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng |
|---|---|---|
| Scan cá nhân | Scan 8 problems từ bối cảnh sinh viên cuối khóa đang thực tập: đọc tài liệu dài, tổng hợp báo cáo nhóm, gom feedback nhiều nguồn, EDA lặp lại, tìm quyết định cũ trong chat... | Có nhiều candidate đa dạng để pitch, không bị kẹt ở một bối cảnh |
| Pitch Problem Card | Pitch Problem Card #1 — đọc tài liệu dài trước khi làm task: trình bày actor (intern/sinh viên), workflow 6 bước, bottleneck rõ ở bước đọc và đoán phần liên quan, metric thời gian | Nhóm nhận ra pattern giống bài toán CSKH: cùng là "tìm đúng thông tin trong tài liệu phân tán trước khi hành động" |
| Challenge bài của bạn khác | Hỏi bài CSKH tra cứu nội quy: "Hiện tại nhân viên workaround thế nào khi tài liệu chưa được số hóa? Có trường hợp nào nhân viên mới làm vs cũ làm thời gian khác nhau rõ rệt không?" | Nhóm làm rõ hơn rằng bottleneck không chỉ là tốc độ tìm mà còn là độ tin cậy của tài liệu tìm được |
| Gom trùng / cluster | Gộp bài "đọc tài liệu dài" của tôi và bài "tra cứu nội quy CSKH" vào cluster "Tìm thông tin trong tài liệu phân tán trước khi hành động" | Giúp nhóm thấy pattern chung, dễ hội tụ hơn thay vì vote theo cảm tính |
| Chọn candidate problem | Đồng ý chọn bài CSKH vì nó có actor cụ thể hơn, impact đo được hơn (hàng trăm câu hỏi/tuần vs 2 lần/tuần của intern) | Nhóm chọn được bài có tác động rộng hơn thay vì bài của tôi có phạm vi hẹp hơn |
| Validation / research | Tìm các tool RAG và Q&A document đã có sẵn: Notion AI Q&A, Azure AI Search, LlamaIndex RAG pattern; ghi rõ giới hạn của từng tool | Nhóm thấy rõ không cần build từ đầu, pattern đã có sẵn; quyết định dùng RAG + human review |
| Workflow nhóm | Đóng góp bảng before/after: so sánh bước thủ công vs bước AI hỗ trợ, xác định fallback khi AI trả lời sai hoặc không tìm được trích dẫn | Workflow nhóm rõ hơn về boundary và điều kiện fallback |
| Problem Statement | Đề xuất bổ sung thêm boundary: "AI không tự gửi câu trả lời, chỉ gợi ý draft có kèm trích dẫn nguồn để nhân viên kiểm tra trước" | Boundary cuối rõ hơn, giảm rủi ro nhân viên tin AI 100% mà không kiểm |
| Rule / Workflow / Agent | Lập luận chọn Workflow (RAG) thay vì Agent: workflow tuyến tính, không cần AI tự quyết bước tiếp theo; nhân viên vẫn làm bước cuối | Nhóm thống nhất không over-engineer thành Agent |
| Decision | Đồng thuận Go với pilot nhỏ: dùng 1 bộ tài liệu nội quy thật, test với 20-30 câu hỏi mẫu, đo thời gian và tỷ lệ trích dẫn đúng | Quyết định có điều kiện rõ ràng, không "Go vì nghe hay" |

---

## Bảng dùng AI trong lab

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Gợi ý thêm problems sau khi tôi đã tự scan trước | Nhớ thêm được problem #4 (EDA lặp lại) và #6 (tìm quyết định cũ) | Gợi ý vài ý quá chung chung như "quản lý lịch họp" — không có workflow thật | Bỏ các ý không gắn với bối cảnh cụ thể của mình |
| Problem Card | Dùng AI phản biện Problem Card #1 của mình ("chỉ ra điểm yếu, đừng khen") | AI chỉ ra metric "số lần hỏi lại mentor" khó đo vì phụ thuộc mentor có thời gian không | AI đề xuất dùng Agent để tự động đọc và tóm tắt ngay khi nhận link — quá sớm | Giữ ở mức Workflow; thêm câu hỏi cho nhóm về tài liệu nhạy cảm |
| Workflow | Nhờ AI vẽ lại workflow dạng ASCII từ mô tả của tôi | Nhanh hơn, trình bày gọn hơn | AI gộp bước "đọc + ghi chú + đoán phần liên quan" thành 1 bước — làm mất bottleneck chính | Tách lại 3 bước riêng, bottleneck nằm đúng chỗ |
| Research | Hỏi AI về các tool RAG + document Q&A đang có sẵn | Gợi ý nhanh LlamaIndex, Azure AI Search, Notion AI | Đưa ra số liệu "giảm 80% thời gian" không có nguồn | Chỉ giữ link tool chính thức; bỏ mọi con số chưa verify |
| Problem Statement | Nhờ AI chỉ ra field nào còn mơ hồ trong PS v0 | Chỉ ra metric "95% câu trả lời đúng" cần ghi rõ ai xác nhận "đúng" | AI đề xuất thêm metric NPS của cư dân — ngoài scope lab | Giữ metric đo được trong pilot: thời gian + có trích dẫn nguồn |
| Rule / Workflow / Agent | Hỏi AI "bài toán này dùng Agent hay Workflow?" | Giải thích tốt sự khác nhau: Agent cần tự quyết bước tiếp theo | AI có xu hướng đề xuất Agent vì "nghe mạnh hơn" | Nhóm tự quyết dùng Workflow vì workflow tuyến tính, không cần AI lập kế hoạch động |
| Decision | Dùng AI để kiểm tra xem pilot plan có hợp lý không | Nhắc nhóm ghi rõ điều kiện exit (khi nào dừng pilot) | Không có điểm sai rõ ở phase này | Thêm điều kiện: "nếu 30% câu trả lời phải sửa lại nhiều thì Not Yet" |

---

## Reflection câu hỏi mở

```text
Tôi học được gì khi nghe top 3 problems của các bạn khác?

Khi nghe các bạn pitch, tôi nhận ra mình hay nhìn problem từ góc của người làm việc đơn lẻ (intern tự đọc tài liệu). Bạn pitch bài CSKH tra cứu nội quy làm tôi nhận ra cùng một pattern "tìm thông tin trong tài liệu" nhưng khi nhân với hàng trăm câu hỏi mỗi tuần, impact lớn hơn rất nhiều. Lăng kính "Pain từ người khác" quan trọng hơn tôi nghĩ — nhiều khi vấn đề đáng giải quyết nhất không phải là vấn đề của bản thân mình.

---

Nhóm có lúc nào bị solution-first không?

Có. Khi bàn về bài CSKH, có lúc nhóm nhảy thẳng vào "dùng RAG" mà chưa hỏi rõ tài liệu hiện tại đang lưu ở đâu, format gì, ai cập nhật, phiên bản nào mới nhất. Tôi đã hỏi "hiện tại nhân viên đang workaround thế nào?" và câu hỏi đó kéo nhóm quay về workflow thật thay vì tiếp tục thảo luận về kỹ thuật RAG.

---

Tôi có thay đổi ý kiến sau khi bị challenge không?

Có. Ban đầu tôi muốn pitch bài của mình (đọc tài liệu dài cho intern) vì nghĩ nó phổ biến nhất. Sau khi nhóm hỏi "có bao nhiêu intern gặp vấn đề này mỗi tuần?" và so với bài CSKH "hàng trăm câu hỏi mỗi tuần", tôi thấy scope của mình nhỏ hơn nhiều. Tôi đổi sang đồng ý chọn bài CSKH — và thấy đây là quyết định đúng hơn vì impact rõ hơn.

---

Tôi đóng góp gì thật sự vào artifact cuối?

Gom cluster giúp nhóm thấy pattern "tìm thông tin trong tài liệu phân tán" là nét chung của nhiều candidate — từ đó hội tụ nhanh hơn. Đề xuất bổ sung boundary "AI không tự gửi, chỉ gợi ý có trích dẫn nguồn" vào PS — nhóm giữ nguyên. Ghi điều kiện fallback và exit cho pilot — giúp quyết định Go có cơ sở thay vì chỉ "nghe hay thì làm thử".

---

Điều khó nhất khi viết Problem Statement là gì?

Phần metric. Viết "giảm thời gian" dễ, nhưng phải ghi rõ: giảm từ bao nhiêu xuống bao nhiêu, đo bằng cách nào, ai xác nhận. Ban đầu nhóm viết "95% câu trả lời đúng" mà không định nghĩa "đúng" là gì và ai sẽ đánh giá. Phải mất một lúc thảo luận mới ra được: nhân viên CSKH xác nhận câu trả lời có trích dẫn nguồn đúng hay không — đó mới là metric đo được trong pilot.

---

Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

Ở bước validation. Nhóm chỉ nói "biết rằng nhân viên CSKH mất nhiều thời gian" nhưng chưa có số thật từ phỏng vấn hoặc log. Nếu làm lại, tôi sẽ đề xuất ngay từ Phase 4: hỏi thẳng 2-3 nhân viên CSKH "lần gần nhất bạn tìm sai hoặc không tìm được nội quy là khi nào?" — để có dấu hiệu thật thay vì ước tính. Validation yếu là điểm tôi nghĩ nhóm có thể cải thiện nhiều nhất.
```

---

## Tự kiểm cuối bài

- [x] [12đ cá nhân] Cá nhân có 8 problems (vượt mức tối thiểu 5) và top 3 Problem Cards đầy đủ 9 field.
- [x] [12đ cá nhân] Đã pitch Problem Card #1, challenge bài CSKH của nhóm, đặt câu hỏi đúng trọng tâm về workflow và validation.
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài (xem group-report.md).
- [x] [15đ nhóm] Nhóm có workflow trước/sau với actor, bottleneck, thời gian và fallback rõ.
- [x] [20đ nhóm] Nhóm có Problem Statement v0/v1 với metric (thời gian + tỷ lệ trích dẫn đúng) và boundary rõ.
- [x] [15đ nhóm] Nhóm có so sánh No AI / Rule / Workflow / Agent với lý do chọn Workflow.
- [x] [10đ nhóm] Nhóm có Go (với pilot nhỏ) và lý do dựa trên pattern đã tồn tại + điều kiện exit.
- [x] [10đ cá nhân] Reflection ghi rõ vai trò trong nhóm, cách dùng AI (và chỗ AI sai), điều học được và nếu làm lại sẽ đổi gì.
- [x] [6đ cá nhân] Tôi tự giải thích được mạch: CSKH nhận câu hỏi → tìm nội quy (bottleneck 3-10') → AI RAG tóm tắt + trích dẫn → nhân viên kiểm tra → trả lời → metric: dưới 30 giây + 95% có trích dẫn đúng → boundary: không tự gửi → Workflow đủ vì workflow tuyến tính + có nhân viên review → Go pilot.
