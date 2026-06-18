---
artifact: 01 - Case Analysis
bai-tap: Lab 1 - Phân tích "tử huyệt" chiến lược
format: Cá nhân trước -> share trong bàn -> chốt verdict cuối
time: 20 phút trên lớp
nop-cuoi: Có - đây là file nộp cuối của Lab 1
---

# Lab 1 - Case Analysis / Phân tích "tử huyệt" chiến lược

**Case đã chọn:** FPT Software / FPT Corporation - mô hình outsource phần mềm bị thị trường đánh giá lại dưới áp lực của AI coding  
**Người làm:** Nguyễn Văn Dương  
**Bàn / nhóm bàn:** 
**Ngày:** 18/06/2026

## Bước 0 - Chọn case thật nhanh

- **Case / sản phẩm / công ty:** FPT Software, mảng dịch vụ CNTT và outsource phần mềm của FPT Corporation.
- **AI / platform / sản phẩm mới tạo áp lực:** GitHub Copilot, ChatGPT, Claude/Cursor và các agent coding có khả năng tạo code, test, debug, viết tài liệu.
- **Vì sao tôi chọn case này?**  
  > FPT từng được thị trường định giá như một công ty công nghệ tăng trưởng cao nhờ lợi thế nhân lực kỹ sư, năng lực delivery offshore và khách hàng quốc tế. AI không "giết" FPT ngay, nhưng làm thay đổi cách khách hàng mua dịch vụ outsource: họ không chỉ mua giờ công lập trình nữa, mà đòi hỏi năng suất, outcome và năng lực AI-native.

## Bước 1 - Gom 3-5 bằng chứng chốt

| # | Bằng chứng / số liệu chốt | Vì sao số này quan trọng? | Nguồn |
|---|---|---|---|
| E1 | FPT Software là nhà cung cấp dịch vụ CNTT/toàn cầu và outsource phần mềm, có mặt tại hơn 30 quốc gia, hơn 80 văn phòng, khoảng 30.000 nhân sự; doanh thu Global IT Services đã vượt mốc 1 tỷ USD năm 2023. | Cho thấy "case trước AI" của FPT dựa nhiều vào quy mô nhân lực, delivery offshore và khả năng bán dịch vụ phần mềm cho khách hàng quốc tế. | FPT Software overview: https://en.wikipedia.org/wiki/FPT_Software |
| E2 | Năm 2024, FPT/FPT Software tiếp tục báo cáo tăng trưởng mạnh, doanh thu 2024 khoảng 2,47 tỷ USD và lợi nhuận trước thuế khoảng 434,57 triệu USD; cùng năm đó FPT xây 2 AI Factories tại Việt Nam và Nhật Bản với NVIDIA. | Đây là bằng chứng hai mặt: FPT vẫn là công ty tốt, nhưng bản thân FPT cũng phải chuyển sang AI infrastructure/AI service để tránh bị commoditize. | FPT Corporation / FPT Software summaries: https://en.wikipedia.org/wiki/FPT_Corporation |
| E3 | Nghiên cứu về GitHub Copilot cho thấy lập trình viên hoàn thành tác vụ nhanh hơn 55,8% trong thí nghiệm có kiểm soát. | Nếu AI làm tăng năng suất lập trình, khách hàng outsource sẽ hỏi lại: vì sao vẫn trả tiền theo số người/số giờ như cũ? | "The Impact of AI on Developer Productivity: Evidence from GitHub Copilot": https://arxiv.org/abs/2302.06590 |
| E4 | Stack Overflow Developer Survey 2025 được báo cáo là 84% developer đang dùng hoặc dự định dùng AI tools; tuy nhiên 46% không tin độ chính xác của output AI. | AI đã vào workflow đại trà, nhưng chưa thay thế hoàn toàn con người. Lợi thế mới không phải "có nhiều coder" mà là "biết kết hợp AI + governance + domain expertise". | ITPro tổng hợp Stack Overflow Survey 2025: https://www.itpro.com/software/development/developers-arent-quite-ready-to-place-their-trust-in-ai-nearly-half-say-they-dont-trust-the-accuracy-of-outputs-and-end-up-wasting-time-debugging-code |
| E5 | Giá cổ phiếu FPT trên HOSE có giai đoạn giảm đáng kể sau vùng đỉnh 2024/2025; tôi xem đây là tín hiệu thị trường đang chiết khấu lại kỳ vọng tăng trưởng/định giá, trong đó AI là một rủi ro chiến lược lớn với mô hình outsource. | Giá cổ phiếu không chứng minh AI là nguyên nhân duy nhất, nhưng là dấu hiệu nhà đầu tư bắt đầu hỏi: tăng trưởng nhân lực và billable hours còn bền vững không khi AI làm giảm giá trị coding commodity? | Biểu đồ HOSE:FPT trên TradingView/SSI/iBoard hoặc trang chứng khoán đang dùng khi nộp bài. |

### 3 phát hiện ban đầu

1. **Case này từng thắng nhờ...**  
   > khả năng tuyển, đào tạo và quản trị số lượng lớn kỹ sư phần mềm với chi phí cạnh tranh, cộng với năng lực delivery cho khách hàng Nhật, Mỹ, châu Âu.
2. **AI shock làm thay đổi...**  
   > đơn vị giá trị trong outsource: từ "số giờ lập trình/số người trong team" sang "tốc độ ra output, chất lượng, IP, domain knowledge và trách nhiệm kết quả".
3. **Dấu hiệu mạnh nhất cho thấy luật chơi mới là...**  
   > AI coding tools đã vào workflow đại trà, FPT cũng phải đầu tư AI Factory/NVIDIA; nghĩa là đây không còn là xu hướng bên lề mà là nền tảng cạnh tranh mới.

## Bước 2 - Viết 4 nhận định bắt buộc

### Nhận định 1 - Trước AI, case này thắng nhờ giả định gì?

**Trả lời của tôi:**  
> Trước AI, FPT Software thắng nhờ giả định rằng khách hàng quốc tế cần "thuê năng lực lập trình bên ngoài" với chi phí thấp hơn, quy mô linh hoạt hơn và delivery on-time hơn so với tự xây team nội bộ. Giá trị lõi của FPT là quy mô kỹ sư, process delivery, quan hệ khách hàng, năng lực tiếng Nhật/thị trường Nhật và khả năng chạy dự án lớn.
>
> Job-to-be-done mà khách hàng "thuê" FPT làm là: biến nhu cầu số hóa/phần mềm thành hệ thống chạy được mà không phải tự tuyển, đào tạo và quản trị toàn bộ đội ngũ kỹ thuật.

**Bằng chứng đỡ nhận định này:** E1, E2

### Nhận định 2 - Kỳ vọng người dùng và luật chơi cạnh tranh đã đổi ở đâu?

**Shift kỳ vọng quan trọng nhất:** Làm xong giúp tôi / trả theo kết quả  
**Competitive dynamic quan trọng nhất:** switching costs giảm và build-copy cycles tăng tốc

**Trả lời của tôi:**  
> Khách hàng outsource không còn mặc định chấp nhận việc tăng headcount là cách chính để tăng output. Khi Copilot/ChatGPT/Claude có thể tạo code, test, refactor, viết tài liệu nhanh hơn, buyer sẽ kỳ vọng nhà cung cấp dịch vụ phải dùng AI để giao nhanh hơn, ít người hơn, minh bạch hơn và gắn với business outcome hơn.
>
> Luật chơi cạnh tranh đổi từ "ai có nhiều kỹ sư hơn" sang "ai có workflow AI-native, data/domain context, quality gate và governance tốt hơn". Nếu FPT chỉ bán manpower, phần giá trị đó dễ bị ép giá; nếu FPT bán AI-enabled delivery và domain solution, FPT vẫn có cửa sống.

**Bằng chứng đỡ nhận định này:** E3, E4, E5

### Nhận định 3 - Giả định nào không còn đúng nữa? Điều gì đã thay đổi vĩnh viễn?

**Điều đã thay đổi vĩnh viễn theo tôi là:**  
> Giả định "lập trình viên là đơn vị sản xuất chính và giờ công là đơn vị tính tiền tự nhiên" không còn chắc đúng. AI biến một phần coding, test, debug, document thành công việc có thể tự động hóa hoặc tăng tốc mạnh. Từ đây, khách hàng sẽ ngày càng hỏi về giá trị cuối cùng: thời gian ra sản phẩm, chất lượng, bảo mật, hiểu biết domain và khả năng chịu trách nhiệm.
>
> Phân khúc outsource vẫn tồn tại, nhưng cách phục vụ sẽ khác: ít giống "cho thuê coder" và giống "đối tác delivery có AI, có tài sản tái sử dụng, có chuyên môn ngành" hơn. Điều vĩnh viễn không phải là giá FPT giảm, mà là chuẩn mới trong đầu buyer: nhà cung cấp phần mềm phải chứng minh năng suất AI và outcome.

**Bằng chứng đỡ nhận định này:** E3, E4, E5

### Nhận định 4 - Case này còn cứu được không? Nếu có, phải đổi bằng cách nào?

**Verdict ban đầu của tôi:** Có nhưng phải đổi rất mạnh

**Trả lời của tôi:**  
> FPT không phải case "chết vì AI"; đây là case "bị AI buộc phải đổi moat". FPT còn nhiều lợi thế: khách hàng lớn, uy tín delivery, thị trường Nhật, quy mô nhân lực, FPT Education và khả năng đầu tư hạ tầng AI. Nhưng nếu FPT tiếp tục để thị trường nhìn mình như công ty outsourcing theo billable headcount, valuation sẽ bị ép.
>
> Cách đổi là chuyển từ labor arbitrage sang AI-native service: dùng AI để tăng năng suất nội bộ, đóng gói solution theo ngành, bán outcome/SLA thay vì chỉ bán số người, xây governance bảo mật cho enterprise, và biến AI Factory thành năng lực giao hàng thật chứ không chỉ là câu chuyện truyền thông.

**Bằng chứng đỡ nhận định này:** E2, E3, E4

## Tóm tắt cá nhân trước khi share trong bàn

1. `Case này yếu đi vì...` FPT Software nếu chỉ được nhìn như nhà cung cấp giờ công lập trình sẽ bị AI coding tools làm giảm giá trị của phần coding commodity.
2. `Điều thay đổi vĩnh viễn là...` buyer outsource sẽ đòi hỏi năng suất AI, delivery theo outcome và domain expertise, không còn mặc định trả tiền theo headcount.
3. `Verdict của tôi là...` FPT còn cứu được, nhưng phải đổi từ labor outsourcing sang AI-native delivery partner.

## Bước 3 - Share trong bàn

| Người | Case | Bằng chứng mạnh nhất họ nêu | Điều họ cho là "thay đổi vĩnh viễn" | Verdict của họ |
|---|---|---|---|---|
| Bạn 1 | Chegg | Thuê bao giảm mạnh sau ChatGPT | Entry point học tập chuyển sang chatbot | Khó cứu nếu chỉ bán lời giải |
| Bạn 2 | Stack Overflow | Developer hỏi AI thay vì lên forum | Knowledge Q&A bị AI chen vào workflow | Phải thành data/enterprise layer |
| Bạn 3 | FPT outsourcing | AI coding tăng năng suất và FPT phải đầu tư AI Factory | Billable headcount không còn là moat đủ | Có nhưng phải đổi mạnh |
| Bạn 4 | Jasper | Copywriting generic bị ChatGPT ép giá | Lớp vỏ prompt/content dễ bị commoditize | Phải đi vào workflow marketing sâu hơn |

**1. Bàn tôi thấy case nào có bằng chứng mạnh nhất? Vì sao?**  
> Chegg và Stack Overflow có bằng chứng tác động trực tiếp hơn về user/traffic. Case FPT khó hơn vì giá cổ phiếu chỉ là tín hiệu gián tiếp, nhưng nó đáng giá vì cho thấy AI ảnh hưởng cả những công ty vẫn tăng trưởng tốt.

**2. Có pattern nào lặp lại giữa nhiều case không?**  
> Pattern lặp lại là AI chiếm entry point và làm giảm giá trị của tác vụ generic. Nơi nào sản phẩm chỉ bán "làm hộ một việc có thể prompt ra được", switching cost giảm rất nhanh. Nơi nào có dữ liệu riêng, workflow sâu, trust và accountability thì còn lợi thế.

**3. Một cảnh báo cho chính dự án của nhóm tôi là gì?**  
> Đừng xây sản phẩm chỉ là lớp vỏ mỏng trên AI. Phải chọn một workflow có pain thật, có dữ liệu/ngữ cảnh riêng và có lý do để user tin kết quả hơn việc tự hỏi ChatGPT.

## Bước 4 - Chốt lại verdict cá nhân sau thảo luận

### Sau khi nghe bàn phản biện, verdict của tôi:

- [ ] Giữ nguyên
- [x] Đổi nhẹ
- [ ] Đổi mạnh

### Vì sao tôi giữ / đổi verdict?

> Tôi đổi nhẹ vì bàn góp ý rằng không nên viết "giá cổ phiếu FPT giảm bởi AI" như một quan hệ nhân quả chắc chắn. Cách viết đúng hơn là: AI là một rủi ro chiến lược làm thị trường re-rating các công ty outsourcing; giá cổ phiếu là một tín hiệu, không phải bằng chứng duy nhất.
>
> Vì vậy verdict cuối tập trung vào thay đổi vĩnh viễn trong buyer expectation, không tập trung vào biến động giá ngắn hạn.

### Verdict cuối cùng của tôi (phiên bản nộp)

**Case này tổn thương trước AI vì:**  
> Một phần giá trị của FPT Software nằm ở việc cung cấp kỹ sư và giờ công phần mềm quy mô lớn. AI coding tools làm phần việc coding/test/document generic nhanh hơn và rẻ hơn, khiến khách hàng outsource có lý do ép giá hoặc đòi hỏi output cao hơn với ít người hơn.

**Điều thay đổi vĩnh viễn là:**  
> Trong dịch vụ phần mềm, "nhiều lập trình viên" không còn tự động đồng nghĩa với "nhiều giá trị". Chuẩn mới là AI-native delivery: nhanh hơn, có domain context, có quality/security governance và gắn với outcome kinh doanh.

**Nếu phải rút 1 bài học cho dự án của nhóm mình, tôi rút ra:**  
> Đừng xây AI product dựa trên tác vụ generic dễ bị copy. Phải tìm đúng job đau nhất trong workflow, gắn AI vào nơi tạo outcome rõ, và có một moat ngoài model như dữ liệu riêng, quy trình tin cậy, domain expertise hoặc distribution.

## Checklist trước khi nộp

- [x] Tôi đã chọn ít nhất 3 bằng chứng chốt có nguồn.
- [x] Mỗi nhận định đều chỉ vào ít nhất 1 bằng chứng.
- [x] Tôi đã ghi lại phần share trong bàn.
- [x] Tôi đã viết verdict cuối sau thảo luận.

