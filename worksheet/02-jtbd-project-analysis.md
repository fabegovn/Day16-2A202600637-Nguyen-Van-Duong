---
artifact: 02 - JTBD Project Analysis
bai-tap: Lab 2 - Dùng JTBD để soi lại dự án nhóm
format: Theo nhóm dự án -> share trong bàn -> chốt hypothesis cuối
time: 25 phút trên lớp
nop-cuoi: Có - đây là file nộp cuối của Lab 2
companion-reference: Strategyn_JTBD_Playbook.pdf
---

# Lab 2 - JTBD Project Analysis / Dùng JTBD để soi lại dự án nhóm

**Tên dự án / sản phẩm:** AI Phân Tích Phản Hồi & Đánh Giá Để Nâng Chất Lượng Dịch Vụ cho GreenSM

## Bước 0 - Khoanh đúng 1 lát cắt của dự án

- **Dự án của nhóm tôi là:** Hệ thống AI giúp GreenSM phân tích phản hồi khách hàng và đánh giá chuyến đi để phát hiện vấn đề dịch vụ, ưu tiên xử lý và theo dõi cải thiện.
- **Lát cắt tôi chọn để phân tích hôm nay là:** Giúp Operations/Customer Experience Manager theo dõi phản hồi tiêu cực sau chuyến đi và review app để tìm vấn đề dịch vụ cần xử lý trong ngày.
- **Vì sao tôi chọn lát cắt này:**  
  > Đây là lát cắt cụ thể, có dữ liệu thật, có workflow rõ và ảnh hưởng trực tiếp đến chất lượng dịch vụ: tài xế, xe, thời gian chờ, app, giá, an toàn và CSKH.

## Bước 1 - Project Snapshot

1. **Nhóm tôi đang nghĩ mình đang giải quyết vấn đề gì?**  
   > GreenSM có nhiều phản hồi từ rating chuyến đi, review app, hotline, ticket CSKH và mạng xã hội. Đội vận hành khó đọc hết, khó biết vấn đề nào nghiêm trọng và khó biến phản hồi thành hành động nhanh.

2. **Người dùng chính hiện nhóm đang nhắm tới là ai?**  
   > Operations Manager / Customer Experience Manager phụ trách chất lượng dịch vụ GreenSM theo thành phố hoặc khu vực.

3. **Hiện tại người dùng đó đang giải quyết vấn đề này bằng cách nào?**  
   > Xem dashboard rating tổng quan, đọc ticket thủ công, lọc review theo sao thấp, nhận báo cáo từ CSKH, họp với đội tài xế/vận hành và xử lý theo kinh nghiệm.

## Bước 2 - Market Context

1. **Ai đang gặp vấn đề này?**  
   > Đội vận hành và đội Customer Experience của GreenSM khi phải giữ chất lượng dịch vụ ổn định ở nhiều khu vực, nhiều tài xế và nhiều kênh phản hồi.

2. **Vấn đề xuất hiện trong hoàn cảnh nào?**  
   > Sau mỗi chuyến đi hoặc sau khi khách hàng để lại review/khiếu nại: xe đến muộn, thái độ tài xế chưa tốt, app lỗi, giá chưa rõ, xe không sạch, hỗ trợ chậm, hoặc trải nghiệm không đúng kỳ vọng.

3. **Hiện tại họ đang dùng giải pháp thay thế nào?**  
   > Dashboard vận hành, CRM/ticket CSKH, Excel/Google Sheets, báo cáo thủ công, đọc review app, social listening cơ bản và họp xử lý theo tuần/ngày.

4. **Vì sao đây là thời điểm đáng giải?**  
   > GreenSM mở rộng nhanh nên phản hồi tăng theo quy mô. Khách hàng gọi xe có switching cost thấp; nếu vấn đề lặp lại mà không được xử lý nhanh, họ có thể chuyển sang Grab, Be, taxi truyền thống hoặc phương tiện cá nhân.

### Tóm tắt market context

> GreenSM không chỉ cạnh tranh bằng xe điện mà còn bằng chất lượng dịch vụ sau mỗi chuyến đi.  
> Khi quy mô tăng, feedback rời rạc từ app, ticket và mạng xã hội trở thành dữ liệu vận hành quan trọng.  
> Đội vận hành cần biết vấn đề nào đang tăng, nghiêm trọng ở đâu, liên quan đến tài xế/khu vực/khung giờ nào và nên xử lý trước việc gì.

## Bước 3 - Job Executor

- **Job executor của dự án này là:** Operations Manager / Customer Experience Manager của GreenSM.
- **Vì sao tôi tin đây là người trực tiếp "thuê" giải pháp để làm job:**  
  > Họ là người phải theo dõi chất lượng dịch vụ, ưu tiên vấn đề, giao việc cho đội CSKH/vận hành/tài xế và chịu trách nhiệm nếu trải nghiệm khách hàng xấu đi.

## Bước 4 - Core JTBD

**Core JTBD bản nháp:**  
> Dùng AI để phân tích feedback khách hàng và cải thiện chất lượng dịch vụ GreenSM.

**Các từ solution tôi đang lỡ nhét vào câu:** AI, GreenSM

**Core JTBD cuối cùng:**  
> Phát hiện và ưu tiên các vấn đề dịch vụ từ phản hồi khách hàng để cải thiện trải nghiệm sau mỗi chuyến đi.

## Bước 5 - 3 Job Stories

| # | Trigger / When | Motivation / I want to | Outcome / so I can | Điều story này cho thấy |
|---|---|---|---|---|
| JS1 | When số lượng đánh giá 1-2 sao tăng sau giờ cao điểm | I want to biết nhóm nguyên nhân chính và khu vực/tài xế liên quan | so I can xử lý vấn đề trước khi nó lặp lại trong ngày hôm sau | Pain nằm ở phát hiện pattern nhanh |
| JS2 | When có nhiều phản hồi chữ nhưng điểm sao trung bình vẫn chưa giảm mạnh | I want to hiểu sentiment và chủ đề phàn nàn ẩn trong nội dung review | so I can không bỏ sót vấn đề trước khi nó thành khủng hoảng | Pain nằm ở hiểu nội dung, không chỉ nhìn rating |
| JS3 | When đội CSKH đã xử lý ticket khiếu nại | I want to biết vấn đề đã giảm chưa và khách hàng có hài lòng hơn không | so I can đánh giá hành động vận hành có hiệu quả thật hay không | Pain nằm ở đóng vòng feedback |

## Bước 6 - Current Alternatives

| Alternative hiện tại | User đang thuê nó để làm gì? | Nó làm tốt gì? | Nó fail ở đâu? | Switching cost hiện tại cao hay thấp? |
|---|---|---|---|---|
| Dashboard rating/chuyến đi | Theo dõi điểm số tổng quan | Nhanh, dễ nhìn xu hướng lớn | Không giải thích nguyên nhân sâu, khó ưu tiên hành động | Trung bình |
| CRM/ticket CSKH | Ghi nhận và xử lý từng khiếu nại | Có quy trình, có owner | Dữ liệu rời rạc, khó thấy pattern toàn hệ thống | Cao |
| Đọc review thủ công/Excel | Tìm lỗi cụ thể từ phản hồi chữ | Linh hoạt, dễ làm ban đầu | Chậm, phụ thuộc người đọc, khó scale | Thấp |
| Social listening cơ bản | Theo dõi nhắc đến thương hiệu | Bắt được tín hiệu công khai | Nhiễu, khó nối với dữ liệu chuyến đi | Trung bình |

**Nếu project của tôi biến mất hôm nay, user nhiều khả năng sẽ quay về:**  
> Dashboard rating + CRM ticket + đọc review thủ công + họp vận hành để xử lý theo kinh nghiệm.

## Bước 7 - JTBD Lite Map

| Step | Trong workflow này user đang cố làm gì? | Hôm nay họ đang dùng gì? | Friction / pain hiện tại | Mức đau |
|---|---|---|---|---|
| Define | Xác định chất lượng dịch vụ cần theo dõi: tài xế, xe, app, giá, chờ lâu, an toàn, CSKH | KPI, SOP, dashboard | KPI tổng quan nhưng chưa gắn với phản hồi cụ thể | Med |
| Locate | Gom phản hồi từ rating chuyến, review app, ticket, hotline, social | CRM, app review, sheet, dashboard | Dữ liệu nằm rải rác, format khác nhau | High |
| Prepare | Làm sạch, nhóm chủ đề, gắn với khu vực/tài xế/khung giờ | Excel, thao tác thủ công | Tốn thời gian, dễ bỏ sót tín hiệu yếu | High |
| Confirm | Kiểm tra vấn đề có thật, mức độ nghiêm trọng và nguyên nhân | Gọi lại khách, hỏi CSKH, kiểm tra log | Khó phân biệt complaint đơn lẻ và pattern thật | High |
| Execute | Giao hành động: nhắc tài xế, sửa app, điều xe, bồi hoàn, cập nhật SOP | Ticket nội bộ, họp vận hành | Ưu tiên chưa rõ, dễ xử lý việc ồn ào thay vì việc quan trọng | Med |
| Monitor | Theo dõi sau khi xử lý: rating, complaint rate, repeat issue | Dashboard, báo cáo | Không rõ hành động nào tạo cải thiện | High |
| Modify | Điều chỉnh rule, training, incentive, quy trình CSKH | SOP, training, chính sách | Chậm nếu insight không đủ cụ thể | Med |
| Conclude | Tổng kết bài học và chuẩn hóa vào playbook vận hành | Báo cáo tuần/tháng | Knowledge khó tái sử dụng nếu chỉ nằm trong slide | Low |

**Bước đau nhất #1:** Locate  
**Bước đau nhất #2:** Prepare / Confirm

**Vì sao đây là nơi đáng chú ý nhất:**  
> Nếu không gom và hiểu đúng phản hồi, đội vận hành chỉ nhìn thấy rating tổng quan hoặc một vài ticket nổi bật.  
> Nơi AI tạo leverage lớn nhất là biến dữ liệu rời rạc thành nhóm vấn đề có mức độ ưu tiên, bằng chứng và owner xử lý.

## Bước 8 - AI Leverage Point

| Step | AI nên giúp bằng cách nào? | Vì sao AI hợp ở đây? | Rủi ro chính nếu dùng AI |
|---|---|---|---|
| Locate / Prepare | Tự động gom phản hồi đa kênh, chuẩn hóa văn bản, nhận diện sentiment, topic, severity và entity như tài xế/khu vực/khung giờ | AI hợp với dữ liệu ngôn ngữ tự nhiên, nhiều nguồn, nhiều cách diễn đạt | Phân loại sai, hiểu sai tiếng lóng/giọng địa phương, thiếu context chuyến đi |
| Confirm / Monitor | Phát hiện pattern bất thường, gợi ý nguyên nhân, ưu tiên ticket và theo dõi sau xử lý | AI có thể so sánh xu hướng và tìm tín hiệu lặp lại nhanh hơn người đọc thủ công | Gợi ý sai nguyên nhân, tạo bias với tài xế/khu vực nếu dữ liệu lệch |

**AI leverage point quan trọng nhất của dự án tôi là:**  
> Phân loại và ưu tiên phản hồi tiêu cực theo chủ đề, mức độ nghiêm trọng, khu vực/tài xế/khung giờ để đội vận hành biết vấn đề nào cần xử lý trước.

**Vì sao không phải ở bước khác:**  
> Nếu chỉ dùng AI để viết câu trả lời CSKH thì chưa chạm vào gốc rễ chất lượng dịch vụ. Điểm đau lớn hơn là phát hiện pattern và biến feedback thành hành động vận hành.

## Bước 9 - Product Hypothesis

> Nếu chúng ta giúp Operations/CX Manager phát hiện và ưu tiên vấn đề dịch vụ từ phản hồi khách hàng ở bước Locate/Prepare/Confirm,  
> bằng cách dùng AI phân tích rating, review, ticket và social feedback để nhóm chủ đề, đo severity, tìm pattern và đề xuất owner xử lý,  
> thì họ sẽ chuyển từ dashboard + CRM + đọc review thủ công sang hệ thống AI Feedback Intelligence,  
> vì họ có thể xử lý vấn đề nhanh hơn, giảm complaint lặp lại và nâng chất lượng trải nghiệm chuyến đi.

### Tín hiệu sớm nếu hypothesis này đúng

1. Thời gian từ lúc phản hồi tiêu cực xuất hiện đến lúc đội vận hành biết nguyên nhân chính giảm ít nhất 30-50%.
2. Tỷ lệ complaint lặp lại ở cùng chủ đề/khu vực/tài xế giảm sau 2-4 tuần thử nghiệm.

## Bước 10 - Assumptions to Validate

| Assumption | Vì sao assumption này rủi ro? | Tôi đang có bằng chứng gì? | Cần validate bằng cách nào tiếp theo? |
|---|---|---|---|
| A1: Operations/CX Manager là job executor đúng | Nếu CSKH lead hoặc city manager mới là người dùng chính, workflow sẽ khác | Suy luận từ trách nhiệm chất lượng dịch vụ | Phỏng vấn 3-5 người trong vai trò CX/Operations |
| A2: Dữ liệu feedback đủ phong phú và truy cập được | Nếu dữ liệu rời rạc hoặc bị hạn chế quyền riêng tư, AI khó tạo giá trị | Có nhiều kênh phản hồi trong dịch vụ gọi xe | Audit nguồn dữ liệu: rating, review, ticket, hotline, social |
| A3: AI phân loại chủ đề/severity đủ chính xác | Nếu sai, đội vận hành mất niềm tin | Nghiên cứu app review cho thấy có thể tự động phân tích review | Test mô hình trên 500-1.000 phản hồi đã gán nhãn |
| A4: Insight dẫn đến hành động vận hành thật | Nếu chỉ ra vấn đề nhưng không có owner/quy trình xử lý, dashboard sẽ bị bỏ | Workflow vận hành có thể giao ticket | Prototype với action queue và owner rõ ràng |
| A5: Cải thiện feedback có thể đo được | Nếu không đo được before/after, khó chứng minh ROI | Có rating và complaint rate làm chỉ số | Chạy pilot theo 1 thành phố/khu vực trong 4 tuần |

**Assumption nguy hiểm nhất nếu tôi đang sai:**  
> AI có thể phân loại feedback tốt nhưng đội vận hành không thể hoặc không có quyền hành động đủ nhanh; khi đó sản phẩm chỉ tạo insight mà không cải thiện chất lượng dịch vụ.

## Bước 11 - Share trong bàn

| Ý phản biện tôi nghe được | Nó chạm vào phần nào? | Tôi sẽ giữ / sửa gì? |
|---|---|---|
| "Đừng chỉ phân tích review app, phải nối với dữ liệu chuyến đi." | AI leverage point | Sửa để thêm entity: tài xế, khu vực, khung giờ, loại xe |
| "Nếu chỉ dashboard thì không đủ, cần action queue." | Product hypothesis | Thêm owner xử lý và theo dõi sau xử lý |
| "Cẩn thận bias với tài xế nếu AI kết luận sai." | Assumptions / risk | Thêm human review và kiểm tra bằng chứng trước khi xử lý kỷ luật |

## Bước 12 - Chốt version cuối sau thảo luận

### Sau khi nghe phản biện, tôi thay đổi gì?

- [x] Giữ nguyên `job executor`
- [ ] Sửa `job executor`
- [ ] Giữ nguyên `core JTBD`
- [x] Sửa `core JTBD`
- [ ] Giữ nguyên `AI leverage point`
- [x] Sửa `AI leverage point`
- [ ] Giữ nguyên `product hypothesis`
- [x] Sửa `product hypothesis`

### Vì sao tôi giữ / sửa?

> Tôi giữ Operations/CX Manager vì đây là người chịu trách nhiệm trực tiếp với chất lượng dịch vụ.  
> Tôi sửa JTBD và hypothesis để không chỉ nói "phân tích feedback", mà nhấn mạnh phát hiện vấn đề, ưu tiên xử lý, giao owner và theo dõi cải thiện.

### Version cuối cùng tôi nộp

**Job executor:**  
> Operations Manager / Customer Experience Manager của GreenSM.

**Core JTBD:**  
> Phát hiện và ưu tiên các vấn đề dịch vụ từ phản hồi khách hàng để cải thiện trải nghiệm sau mỗi chuyến đi.

**2 bước đau nhất trong workflow:**  
> Locate và Prepare/Confirm.

**AI leverage point chính:**  
> AI gom phản hồi đa kênh, phân loại sentiment/topic/severity, gắn với tài xế/khu vực/khung giờ và đề xuất action queue cho đội vận hành.

**Product hypothesis:**  
> Nếu GreenSM giúp Operations/CX Manager phát hiện sớm và ưu tiên đúng vấn đề dịch vụ từ feedback khách hàng bằng AI Feedback Intelligence, họ sẽ chuyển từ dashboard + CRM + đọc review thủ công sang hệ thống mới vì nó giảm thời gian phát hiện lỗi, giảm complaint lặp lại và cải thiện trải nghiệm chuyến đi.

**Assumption cần validate đầu tiên:**  
> Insight từ AI có dẫn tới hành động vận hành đủ nhanh và đo được cải thiện trong rating/complaint rate hay không.

## Checklist trước khi nộp

- [x] Tôi đã khoanh đúng 1 lát cắt cụ thể của dự án.
- [x] Tôi đã phân biệt được `job executor` với buyer / influencer.
- [x] `Core JTBD` của tôi không nhét solution vào câu.
- [x] Tôi đã viết đủ 3 `job stories`.
- [x] Tôi đã điền `JTBD lite map` và khoanh ra 2 bước đau nhất.
- [x] Tôi đã chỉ ra `AI leverage point` thay vì nhảy thẳng vào feature list.
- [x] Tôi đã ghi rõ `assumptions to validate`.
- [x] Tôi đã sửa version cuối sau khi share trong bàn.

