# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Trần Ngọc Khánh
- Mã học viên: 2A202602923
- Nhóm: X Zone C
- Candidate problem nhóm chọn: Chuẩn hóa commit message và tối ưu quy trình merge code nhiều lập trình viên khi push lên các nhánh feature và production trong dự án phát triển phần mềm.

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Tôi scan 10 vấn đề từ công việc quản lý fanpage theo 4 lăng kính và ghi số liệu theo chat/ngày, thời gian/chat, số đơn và tỷ lệ xử lý. | Nhóm có 3 candidate fanpage với actor, bottleneck và metric cụ thể để đưa vào bảng hội tụ. |
| Pitch Problem Card | Tôi pitch card trả lời FAQ, nêu rõ 30 chat FAQ/ngày, 60-180 giây/chat và 20% chat phải hỏi lại kho. | Candidate được đưa vào shortlist, nhưng sau đó nhóm đánh giá Rule-based chatbot đã giải quyết phần lớn nhu cầu. |
| Challenge bài của bạn khác | Tôi challenge candidate chuẩn hóa commit/merge ở phần quyền AI, nhánh được phép thao tác và nguy cơ AI làm mất code khi xử lý conflict. | Nhóm làm rõ AI chỉ được hỗ trợ trên feature branch; protected branches vẫn cần CI gate và human approval. |
| Gom trùng / cluster | Tôi cùng nhóm gom các candidate thành 4 cụm: quy trình phát triển phần mềm, tài liệu/số liệu, giao tiếp khách hàng và quản lý công việc. | Nhóm nhìn thấy cụm code/test/merge có cùng actor kỹ thuật và dễ thử nghiệm trực tiếp hơn. |
| Chọn candidate problem | Tôi tham gia so sánh FAQ, CI/CD fail log và commit/merge theo 7 tiêu chí actor, workflow, evidence, impact, lab fit, R/W/A và domain. | Nhóm chọn candidate commit/merge với điểm 35/35 vì workflow kỹ thuật rõ và tất cả thành viên hiểu domain. |
| Validation / research | Tôi tham gia xem bằng chứng 3 backend/Tech Lead, survey 8 sinh viên CNTT và review 30 Pull Requests được ghi trong group report. | Nhóm có evidence về commit sai chuẩn, thời gian merge và nhu cầu dọn lịch sử; đồng thời xác định cần giữ người review. |
| Workflow nhóm | Tôi tham gia rà current workflow từ code/stage → commit → PR → rebase → merge → changelog và future workflow có CI gate. | Workflow chỉ rõ bottleneck 15-20 phút/PR, handoff Dev/Tech Lead, nhánh protected và fallback thủ công. |
| Problem Statement | Tôi tham gia kiểm tra các field Actor, Workflow, Bottleneck, Impact, Success Metric và Boundary của bài toán mới. | PS v1 xác định rõ AI được thao tác trên feature branch nhưng không được sửa conflict logic, approve, merge hoặc push production. |
| Rule / Workflow / Agent | Tôi so sánh Commitlint/Branch Protection/CI Rule với Workflow có AI và Agent cục bộ. | Nhóm chọn Workflow có kiểm soát: Rule làm cổng an toàn, AI Agent chỉ hỗ trợ task cục bộ, người thật duyệt các điểm quan trọng. |
| Decision | Tôi cùng nhóm kiểm tra data/input, metric 2 tuần/20 PR, rủi ro source code và phương án rollback. | Nhóm chọn `Go` với pilot trên một repository nội bộ, giữ Commitlint, CI và Branch Protection làm lớp bảo vệ. |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Tôi là người đưa candidate fanpage và tham gia writer/workflow, nhưng candidate cuối cùng của nhóm là bài toán chuẩn hóa commit message và merge code. Dấu tay rõ nhất của tôi trong artifact cuối là phần challenge về boundary: AI có thể hỗ trợ feature branch, nhưng không được tự sửa conflict logic, approve, merge hoặc push vào protected branch.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Gợi ý thêm góc nhìn cho công việc quản lý fanpage sau khi tôi xác định bối cảnh. | Giúp tôi tạo candidate cá nhân để mang vào nhóm, đồng thời nhận ra không nên bắt đầu bằng Agent. | AI dễ đưa ý tưởng “AI tự bán hàng” quá rộng và không có workflow kiểm soát. | Tôi chỉ dùng phần scan fanpage làm candidate, sau đó để nhóm đánh giá cùng các bài kỹ thuật. |
| Problem Card | Phản biện actor, bottleneck, metric và non-AI alternative của card fanpage. | Giúp tôi hiểu FAQ/Saved Reply là phương án thay thế hợp lý. | AI có xu hướng đề xuất chatbot trước khi xác định pain còn lại sau Rule. | Tôi giữ candidate fanpage ở phạm vi trả lời FAQ, không trình bày nó như một Agent tự chốt đơn. |
| Workflow | Tôi dùng AI để kiểm tra cách mô tả workflow, nhưng không dùng AI để quyết định candidate cuối. | Có thể chuyển các bước Git thành chuỗi current/future rõ ràng để nhóm review. | AI có thể tự động hóa quá mức, đặc biệt ở bước sửa conflict hoặc merge production. | Tôi yêu cầu tách feature branch, protected branch, CI gate và human approval thành các boundary riêng. |
| Research | Tôi dùng AI để gợi ý các công cụ/pattern như Conventional Commits, Commitlint, GitHub Copilot và Semantic Release. | Giúp nhóm có hướng research nhanh về Rule, AI hỗ trợ PR và tự động hóa changelog. | AI không tự chứng minh được quyền riêng tư mã nguồn, chi phí hay mức hiệu quả của từng tool. | Tôi dựa vào link chính thức trong group report và không coi claim của AI là evidence nếu chưa kiểm tra. |
| Problem Statement | Tôi dùng AI để phản biện field mơ hồ, nhất là metric và boundary. | Giúp nhìn ra cần baseline theo 20 PR/2 tuần, tỷ lệ commit đúng chuẩn và điều kiện merge. | AI có thể viết các ngưỡng nghe hợp lý nhưng không thay thế dữ liệu Git thật. | Tôi giữ các metric gắn với timestamp PR, regex commit, CI status và branch protection, thay vì chỉ ghi “nhanh hơn”. |
| Rule / Workflow / Agent | Tôi dùng AI để so sánh ba mức trên bài toán commit/merge. | Giúp tách Rule kiểm tra cú pháp khỏi AI hỗ trợ sinh commit/PR summary và giải thích conflict. | AI có xu hướng xem Agent tự checkout, code, commit và push là giải pháp mặc định. | Tôi giới hạn Agent ở feature branch; Rule và con người giữ quyền kiểm soát merge, production và conflict logic. |
| Decision | Tôi dùng AI để rà điều kiện Go, pilot và rollback. | Giúp nhóm liệt kê rõ data thử nghiệm, 20 PR, 3 metric cốt lõi và điều kiện dừng. | AI không thể tự chịu trách nhiệm về source code privacy hoặc quyết định deploy. | Tôi giữ Tech Lead/Peer Reviewer là owner cuối, đồng thời duy trì fallback Commitlint và Branch Protection khi AI bị tắt. |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

**Reflection:**

```text
Khi nghe các candidate của các thành viên, tôi nhận ra problem có vẻ phù hợp với AI vẫn cần được kiểm tra actor, workflow, data và boundary trước khi chọn. Candidate fanpage của tôi dễ hiểu và có số liệu, nhưng nhóm loại vì nhiều câu hỏi cố định đã có thể xử lý bằng Rule-based chatbot. Tôi thay đổi quan điểm khi thấy candidate commit/merge có workflow kỹ thuật rõ hơn, evidence từ PR và khả năng đo trực tiếp trên Git. Điều khó nhất khi viết Problem Statement là không gom tất cả thao tác Git vào một chữ “tự động hóa”, mà phải tách commit, PR, CI, review, merge và production thành các bước có owner. Tôi học được rằng Rule như Commitlint và Branch Protection không đối lập với AI mà là lớp kiểm soát bắt buộc. AI Agent chỉ nên hỗ trợ tác vụ cục bộ trên feature branch, còn người phải đọc diff và quyết định merge. Tôi đặc biệt chú ý đến boundary khi nhóm thảo luận nguy cơ AI tự sửa conflict và làm mất code của thành viên khác. Đóng góp rõ nhất của tôi là challenge về ranh giới quyền hạn, human approval và fallback khi AI gặp lỗi. Tôi đồng ý với quyết định Go vì nhóm có data đầu vào rõ, metric trên 20 PR trong 2 tuần và rollback về Commitlint/Branch Protection. Nếu làm lại, tôi sẽ yêu cầu nhóm kiểm tra lại các claim về chi phí API, source code privacy và khả năng self-host bằng nguồn chính thức trước khi đưa vào lập luận. Tôi cũng sẽ đề nghị thử Rule-only trước trên một số PR để đo chính xác phần giá trị tăng thêm của AI Agent.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI

