---
artifact: 02 - JTBD Project Analysis
bai-tap: Lab 2 - Dùng JTBD để soi lại dự án nhóm
format: Theo nhóm dự án -> share trong bàn -> chốt hypothesis cuối
time: 25 phút trên lớp
nop-cuoi: Có - đây là file nộp cuối của Lab 2
companion-reference: Strategyn_JTBD_Playbook.pdf
---

# Lab 2 - JTBD Project Analysis / Dùng JTBD để soi lại dự án nhóm

**Tên dự án / sản phẩm:** AI Delivery Copilot cho team outsource phần mềm

## Bước 0 - Khoanh đúng 1 lát cắt của dự án

- **Dự án của nhóm tôi là:** AI Delivery Copilot giúp team outsource phần mềm biến yêu cầu khách hàng thành plan, task, test case và báo cáo tiến độ có kiểm soát.
- **Lát cắt tôi chọn để phân tích hôm nay là:** Giúp Project Manager / Tech Lead trong công ty outsource xử lý yêu cầu mới từ khách hàng enterprise trước khi giao cho developer.
- **Vì sao tôi chọn lát cắt này:**  
  > Đây là điểm đau và có tác động lớn: nếu hiểu sai requirement, toàn bộ sprint bị trễ, estimate sai, dev làm lại nhiều và khách hàng mất tin tưởng.

## Bước 1 - Project Snapshot

1. **Nhóm tôi đang nghĩ mình đang giải quyết vấn đề gì?**  
   > Team outsource tốn nhiều thời gian đọc requirement, hỏi lại khách hàng, tách task, estimate, viết acceptance criteria và cập nhật tiến độ.

2. **Người dùng chính hiện nhóm đang nhắm tới là ai?**  
   > Project Manager / Tech Lead phụ trách một team outsource 5-20 developer.

3. **Hiện tại người dùng đó đang giải quyết vấn đề này bằng cách nào?**  
   > Đọc tài liệu khách hàng thủ công, họp với BA/dev, viết ticket trên Jira, dùng template Excel/Google Docs, hỏi ChatGPT riêng lẻ và tự kiểm tra lại.

## Bước 2 - Market Context

1. **Ai đang gặp vấn đề này?**  
   > PM/Tech Lead trong công ty outsource phần mềm làm dự án cho khách hàng quốc tế.

2. **Vấn đề xuất hiện trong hoàn cảnh nào?**  
   > Khi khách hàng gửi requirement mới, change request hoặc feedback gấp trước sprint planning.

3. **Hiện tại họ đang dùng giải pháp thay thế nào?**  
   > Jira, Confluence, Excel, Google Docs, họp nội bộ, ChatGPT/Copilot dùng cá nhân và kinh nghiệm của senior.

4. **Vì sao đây là thời điểm đáng giải?**  
   > AI coding làm khách hàng kỳ vọng delivery nhanh hơn, nhưng bottleneck thực tế chuyển lên bước hiểu đúng requirement, tách việc và kiểm soát chất lượng.

### Tóm tắt market context

> Outsource phần mềm không chỉ cần viết code nhanh; cần biến yêu cầu mơ hồ của khách hàng thành công việc rõ, có ưu tiên, có acceptance criteria và có risk tracking.  
> Khi AI làm coding nhanh hơn, lợi thế của nhà cung cấp dịch vụ nằm ở khả năng điều phối workflow, domain context và đảm bảo chất lượng.  
> Nếu PM/Tech Lead vẫn làm bước phân tích requirement thủ công, team sẽ không tận dụng được AI và vẫn bị trễ ở đầu sprint.

## Bước 3 - Job Executor

- **Job executor của dự án này là:** Project Manager / Tech Lead trong team outsource phần mềm.
- **Vì sao tôi tin đây là người trực tiếp "thuê" giải pháp để làm job:**  
  > Họ là người nhận requirement, quyết định cách tách task, hỏi lại khách hàng, phân công dev và chịu trách nhiệm khi sprint trễ hoặc deliver sai.

## Bước 4 - Core JTBD

**Core JTBD bản nháp:**  
> Biến requirement của khách hàng thành kế hoạch delivery rõ ràng bằng AI.

**Các từ solution tôi đang lỡ nhét vào câu:** AI

**Core JTBD cuối cùng:**  
> Chuyển yêu cầu khách hàng thành kế hoạch delivery rõ ràng, có thể giao việc và kiểm soát được trước khi sprint bắt đầu.

## Bước 5 - 3 Job Stories

| # | Trigger / When | Motivation / I want to | Outcome / so I can | Điều story này cho thấy |
|---|---|---|---|---|
| JS1 | When khách hàng gửi requirement mới bằng email/tài liệu dài | I want to tóm tắt scope, câu hỏi mở và rủi ro chính | so I can phản hồi nhanh mà không bỏ sót điểm quan trọng | Pain nằm ở bước đọc-hiểu và clarify requirement |
| JS2 | When sprint planning sắp diễn ra nhưng requirement còn mơ hồ | I want to tách thành epic/story/task kèm acceptance criteria | so I can giao việc cho dev và QA mà ít phải làm lại | Pain nằm ở prepare/confirm trước khi execute |
| JS3 | When khách hàng thay đổi scope giữa sprint | I want to thấy tác động lên timeline, task và risk | so I can thương lượng lại deadline/effort có cơ sở | Pain nằm ở modify và monitor change |

## Bước 6 - Current Alternatives

| Alternative hiện tại | User đang thuê nó để làm gì? | Nó làm tốt gì? | Nó fail ở đâu? | Switching cost hiện tại cao hay thấp? |
|---|---|---|---|---|
| Jira + Confluence | Ghi task, tài liệu, trạng thái | Chuẩn enterprise, team quen dùng | Không tự hiểu requirement, không tự tạo câu hỏi/risk | Cao vì đã nằm trong workflow |
| Họp nội bộ với BA/dev senior | Làm rõ scope và estimate | Có context và judgement người thật | Tốn thời gian, phụ thuộc senior, khó scale | Trung bình |
| ChatGPT/Copilot cá nhân | Tóm tắt, viết draft ticket/test case | Nhanh, rẻ, linh hoạt | Rời rạc, khó bảo mật, không gắn với Jira/context dự án | Thấp |

**Nếu project của tôi biến mất hôm nay, user nhiều khả năng sẽ quay về:**  
> Jira/Confluence + họp nội bộ + dùng ChatGPT riêng lẻ để tạo draft.

## Bước 7 - JTBD Lite Map

| Step | Trong workflow này user đang cố làm gì? | Hôm nay họ đang dùng gì? | Friction / pain hiện tại | Mức đau |
|---|---|---|---|---|
| Define | Xác định mục tiêu, scope, deadline, stakeholder | Email, brief, họp kickoff | Requirement dài, mơ hồ, nhiều assumption ẩn | High |
| Locate | Tìm tài liệu, API, ticket cũ, decision cũ | Confluence, Drive, Jira | Context nằm rải rác nhiều nơi | Med |
| Prepare | Tách epic/story/task, viết AC, estimate | Jira, Excel, họp team | Tốn thời gian, chất lượng phụ thuộc senior | High |
| Confirm | Hỏi lại khách hàng, chốt scope và acceptance | Email, meeting notes | Câu hỏi không đầy đủ, dễ miss edge case | High |
| Execute | Dev code, QA test | IDE, GitHub, CI/CD, Copilot | AI hỗ trợ code nhưng nếu task sai thì vẫn làm lại | Med |
| Monitor | Theo dõi tiến độ, blocker, scope creep | Jira dashboard, daily standup | Báo cáo trễ, risk phát hiện muộn | Med |
| Modify | Xử lý change request giữa sprint | Họp gấp, sửa ticket thủ công | Khó thấy tác động lên timeline/effort | High |
| Conclude | Tổng kết delivery, demo, lesson learned | Report, retrospective | Knowledge không được tái sử dụng tốt | Low |

**Bước đau nhất #1:** Prepare  
**Bước đau nhất #2:** Confirm

**Vì sao đây là nơi đáng chú ý nhất:**  
> Nếu prepare/confirm sai, AI coding ở bước execute chỉ giúp team làm nhanh một việc sai.  
> Đây cũng là nơi PM/Tech Lead có nhiều tài liệu, ngữ cảnh và quy tắc để AI hỗ trợ, nhưng vẫn cần người chốt để tránh sai requirement.

## Bước 8 - AI Leverage Point

| Step | AI nên giúp bằng cách nào? | Vì sao AI hợp ở đây? | Rủi ro chính nếu dùng AI |
|---|---|---|---|
| Prepare | Đọc requirement, đề xuất epic/story/task, acceptance criteria, test ideas và estimate range | Đây là tác vụ nhiều ngôn ngữ tự nhiên, có pattern lặp lại, cần draft nhanh | Hallucinate scope, estimate ảo, bỏ sót rủi ro domain |
| Confirm | Tạo danh sách câu hỏi clarify, risk log và impact nếu không chốt | AI giỏi trong việc soát lỗ hổng và đối chiếu checklist | Hỏi quá nhiều câu chung chung, làm khách hàng rối |

**AI leverage point quan trọng nhất của dự án tôi là:**  
> Biến requirement mơ hồ thành draft backlog + câu hỏi clarify + risk log trước sprint planning.

**Vì sao không phải ở bước khác:**  
> Execute đã có Copilot/Cursor hỗ trợ code. Pain lớn hơn nằm trước khi code: hiểu sai, tách sai, confirm thiếu. Nếu chen AI vào prepare/confirm, team giảm rework và tăng độ tin của delivery.

## Bước 9 - Product Hypothesis

> Nếu chúng ta giúp PM/Tech Lead chuyển yêu cầu khách hàng thành backlog, acceptance criteria và câu hỏi clarify tốt hơn ở bước Prepare/Confirm,  
> bằng cách dùng AI đọc requirement, truy xuất context dự án và đề xuất risk/task có human approval,  
> thì họ sẽ chuyển từ Jira + họp thủ công + ChatGPT riêng lẻ sang AI Delivery Copilot tích hợp với workflow dự án,  
> vì họ tiết kiệm thời gian planning, giảm rework và có bằng chứng rõ hơn khi thương lượng scope với khách hàng.

### Tín hiệu sớm nếu hypothesis này đúng

1. PM/Tech Lead sẵn sàng đưa requirement thật vào tool và dùng draft ticket trong sprint planning.
2. Thời gian từ lúc nhận requirement đến lúc có backlog draft/câu hỏi clarify giảm ít nhất 30%.

## Bước 10 - Assumptions to Validate

| Assumption | Vì sao assumption này rủi ro? | Tôi đang có bằng chứng gì? | Cần validate bằng cách nào tiếp theo? |
|---|---|---|---|
| A1: PM/Tech Lead là job executor đúng | Nếu BA mới là người làm chính, product sẽ sai user | Suy luận từ workflow outsource | Phỏng vấn 5 PM/Tech Lead và 5 BA |
| A2: Prepare/Confirm là pain đủ đau | Nếu pain thật nằm ở sales/contract hoặc QA, leverage point sai | Logic từ rework trong sprint | Diary study 2 sprint, đo thời gian planning/rework |
| A3: User tin AI nếu có human approval | Nếu AI bị xem là quá rủi ro, adoption thấp | AI hiện đã được dùng cá nhân | Prototype với audit trail và approval flow |
| A4: Tích hợp Jira/Confluence đủ để tạo giá trị | Nếu context nằm trong email/call/Slack quá nhiều, tool thiếu dữ liệu | Alternatives hiện tại dùng Jira/Confluence | Test import dữ liệu thật từ 2-3 dự án |
| A5: Khách hàng chấp nhận cách làm AI-assisted | Nếu hợp đồng/bảo mật cấm đưa tài liệu vào AI, bị chặn | Enterprise có lo ngại data | Validate với chính sách bảo mật và option private deployment |

**Assumption nguy hiểm nhất nếu tôi đang sai:**  
> Pain Prepare/Confirm không đủ lớn hoặc không xảy ra thường xuyên; nếu sai, product chỉ là tool tạo ticket đẹp chứ không giảm được rework thật.

## Bước 11 - Share trong bàn

| Ý phản biện tôi nghe được | Nó chạm vào phần nào? | Tôi sẽ giữ / sửa gì? |
|---|---|---|
| "Đừng gọi user là công ty outsource, phải chọn PM/Tech Lead hoặc BA." | Job executor | Giữ PM/Tech Lead làm executor, BA là collaborator |
| "AI tạo ticket thì dễ copy; moat nằm ở context dự án và approval flow." | AI leverage point | Sửa hypothesis để nhấn mạnh tích hợp Jira/Confluence và human approval |
| "Nếu requirement sai từ đầu, AI có thể làm sai nhanh hơn." | Risk / assumptions | Thêm assumption về trust, audit trail và validate bằng prototype |

## Bước 12 - Chốt version cuối sau thảo luận

### Sau khi nghe phản biện, tôi thay đổi gì?

- [x] Giữ nguyên `job executor`
- [ ] Sửa `job executor`
- [ ] Giữ nguyên `core JTBD`
- [x] Sửa `core JTBD`
- [x] Giữ nguyên `AI leverage point`
- [ ] Sửa `AI leverage point`
- [ ] Giữ nguyên `product hypothesis`
- [x] Sửa `product hypothesis`

### Vì sao tôi giữ / sửa?

> Tôi giữ PM/Tech Lead vì đây là người chịu trách nhiệm delivery và ra quyết định trong sprint planning.  
> Tôi sửa JTBD và hypothesis để bỏ bớt từ "AI" khỏi job statement, đồng thời nhấn mạnh context dự án, approval flow và risk log thay vì chỉ tạo ticket tự động.

### Version cuối cùng tôi nộp

**Job executor:**  
> Project Manager / Tech Lead trong team outsource phần mềm.

**Core JTBD:**  
> Chuyển yêu cầu khách hàng thành kế hoạch delivery rõ ràng, có thể giao việc và kiểm soát được trước khi sprint bắt đầu.

**2 bước đau nhất trong workflow:**  
> Prepare và Confirm.

**AI leverage point chính:**  
> Đọc requirement và context dự án để tạo backlog draft, acceptance criteria, câu hỏi clarify và risk log có human approval.

**Product hypothesis:**  
> Nếu chúng ta giúp PM/Tech Lead làm rõ requirement và tạo backlog có thể giao việc ở bước Prepare/Confirm bằng AI có context dự án và approval flow, họ sẽ chuyển từ Jira + họp thủ công + ChatGPT riêng lẻ sang AI Delivery Copilot vì nó giảm thời gian planning và giảm rework trong sprint.

**Assumption cần validate đầu tiên:**  
> Prepare/Confirm có phải pain đủ lớn, xảy ra đủ thường xuyên và đang làm team mất tiền/thời gian vì rework hay không.

## Checklist trước khi nộp

- [x] Tôi đã khoanh đúng 1 lát cắt cụ thể của dự án.
- [x] Tôi đã phân biệt được `job executor` với buyer / influencer.
- [x] `Core JTBD` của tôi không nhét solution vào câu.
- [x] Tôi đã viết đủ 3 `job stories`.
- [x] Tôi đã điền `JTBD lite map` và khoanh ra 2 bước đau nhất.
- [x] Tôi đã chỉ ra `AI leverage point` thay vì nhảy thẳng vào feature list.
- [x] Tôi đã ghi rõ `assumptions to validate`.
- [x] Tôi đã sửa version cuối sau khi share trong bàn.

