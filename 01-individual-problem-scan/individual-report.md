# 01 — Individual Problem Scan

## Scan rộng

| Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật cần xác thực |
|---|---|---|---|
| Pain từ người khác / rủi ro cao | Trẻ em hoặc thú cưng có thể bị bỏ quên, mắc kẹt trong xe đóng kín khi người lái rời đi | Trẻ em, thú cưng, phụ huynh/chủ xe, người thân | Có các vụ việc thực tế; xe đỗ dưới nắng nóng, người lái quên kiểm tra hàng ghế sau |
| Lặp lại | Nhân viên phải đọc, phân loại và phản hồi nhiều email/tin nhắn cùng lúc, dẫn tới bỏ sót hoặc trả lời chậm | Sales, CSKH, PM, quản lý, nhân viên văn phòng | Inbox có nhiều tin giống nhau: hỏi thông tin, xin cập nhật, đặt lịch, nhắc việc; một số email tồn đọng quá lâu |
| Tốn thời gian | Người tham gia họp mất thời gian tự tìm lại tài liệu, quyết định cũ, KPI và các đầu việc liên quan trước cuộc họp | PM, manager, sales, team member | Mọi người hỏi “context của cuộc họp này là gì?” hoặc mất 10–20 phút mở nhiều tab trước khi họp |
| AI có thể tốt hơn | Người bán trên sàn TMĐT có nhiều review, bình luận và dữ liệu thị trường nhưng khó rút ra lý do khách mua/chê sản phẩm | Seller, brand manager, đội e-commerce, marketing | Review bị đọc thủ công; insight thường dựa vào vài comment nổi bật thay vì toàn bộ dữ liệu |
| Lặp lại / cá nhân hóa kém | Người dùng quên việc hoặc nhận nhắc nhở không đúng lúc, vì các ứng dụng hiện tại ít hiểu ngữ cảnh và thói quen cá nhân | Nhân viên văn phòng, sinh viên, phụ huynh, người bận rộn | To-do list tồn đọng; người dùng tự tạo nhiều reminder nhưng vẫn snooze hoặc bỏ qua |

## Vì sao phần scan này mạnh

- Có 55 problem thuộc các mức độ khác nhau: an toàn, năng suất làm việc, phối hợp nhóm, insight kinh doanh và quản lý cá nhân.
- Mỗi problem xác định rõ actor chịu ảnh hưởng và hành vi/dấu hiệu cần kiểm chứng.
- Không bắt đầu từ giải pháp như “xây chatbot” hay “làm agent”, mà bắt đầu từ workflow và pain.
- Có phân biệt problem có rủi ro cao với problem có thể thử nghiệm nhanh.

## Top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | AI gom context trước cuộc họp | Workflow rõ, xảy ra thường xuyên, dễ đo thời gian tiết kiệm và có thể giữ người dùng review trước khi dùng | Cần quyền truy cập Calendar, Docs, Slack, Notion hoặc CRM; context nào là đủ và không gây nhiễu |
| 2 | Trợ lý phân loại và trả lời email/tin nhắn | Pain phổ biến, tần suất cao, giá trị dễ thấy qua thời gian phản hồi và số tin bị bỏ sót | Người dùng có tin AI gửi sai hoặc giọng điệu không phù hợp không; cần ranh giới rõ giữa draft và auto-send |
| 3 | Phân tích hành vi người mua TMĐT | Có giá trị kinh doanh trực tiếp: giúp cải thiện sản phẩm, nội dung bán hàng và xử lý complaint | Data từ sàn có đủ quyền truy cập không; insight có thực sự dẫn đến quyết định tốt hơn không |
| — | Phát hiện trẻ em/thú cưng trong xe | Impact an toàn rất lớn, nhưng thuộc bài toán safety-critical và cần độ tin cậy cực cao | Phần cứng/cảm biến, pháp lý, false positive/false negative và trách nhiệm khi hệ thống thất bại |
| — | Trợ lý nhắc việc cá nhân hóa | Nhu cầu rộng, nhưng thị trường đã đông và khó tạo khác biệt rõ ràng | Người dùng có muốn chia sẻ đủ dữ liệu ngữ cảnh; cá nhân hóa nào khiến họ quay lại hằng ngày |

## Problem Card #1 — AI gom context trước cuộc họp

### Problem 1 câu

Trước mỗi cuộc họp, PM và team member mất thời gian tìm tài liệu, quyết định cũ, KPI và action item liên quan từ nhiều công cụ, nên vào họp thiếu bối cảnh hoặc phải dùng thời gian họp để nhắc lại context.

### Actor

PM, manager, sales lead hoặc team member thường xuyên tham gia các cuộc họp có nhiều bên liên quan.

### Thời điểm / bối cảnh

Khoảng 10–30 phút trước cuộc họp; đặc biệt với weekly sync, project update, client meeting và cross-functional meeting.

### Current workflow

1. Mở Calendar để xem tiêu đề, người tham gia và agenda.
2. Tìm tài liệu liên quan trong Google Drive, Notion hoặc Confluence.
3. Tìm các thread Slack/email có quyết định hoặc trao đổi gần đây.
4. Kiểm tra task, KPI hoặc tiến độ trong Jira, CRM hay Sheets.
5. Tự ghi chú các câu hỏi cần hỏi và các việc cần follow-up.
6. Vào họp, đôi khi vẫn thiếu một phần context quan trọng.

### Bottleneck

Bước tìm và ghép context từ nhiều nguồn. Người dùng không chỉ mất thời gian tìm kiếm mà còn phải tự quyết định thông tin nào liên quan nhất.

### Impact

Nếu mỗi người mất khoảng 15 phút chuẩn bị cho 5 cuộc họp/tuần, họ mất khoảng 75 phút/tuần. Khi thiếu context, cuộc họp dễ lặp lại thông tin cũ, kéo dài hoặc ra quyết định thiếu dữ liệu.

### Success metric

- Giảm thời gian chuẩn bị từ khoảng 15 phút xuống dưới 5 phút/cuộc họp.
- Giảm số lần phải hỏi lại “quyết định trước là gì?” trong cuộc họp.
- Người dùng đánh giá context được chuẩn bị là hữu ích ở mức 4/5 trở lên.
- Không đưa nhầm tài liệu nhạy cảm hoặc không liên quan vào brief.

### Non-AI alternative

Dùng agenda template, yêu cầu người tổ chức đính kèm tài liệu trước họp và duy trì một trang meeting history. Cách này tốt nhưng phụ thuộc vào kỷ luật cập nhật thủ công của mọi người.

### AI hypothesis

AI đọc metadata cuộc họp và các nguồn đã được cấp quyền, sau đó tạo một pre-meeting brief ngắn gồm: mục tiêu cuộc họp, tài liệu liên quan, quyết định gần nhất, tiến độ, open questions và action item chưa hoàn thành. Người dùng luôn kiểm tra brief trước khi dùng.

### Quick gut

Workflow.

### Draft current workflow

Current state — khoảng 15 phút/cuộc họp

1. Mở Calendar: 1 phút
2. Tìm tài liệu: 5 phút
3. Tìm Slack/email: 4 phút
4. Kiểm tra task/KPI: 3 phút
5. Tự ghi chú: 2 phút

Bottleneck: tìm và ghép context phân tán giữa nhiều nguồn.

### Draft future workflow

Future state — khoảng 4 phút/cuộc họp

1. AI nhận diện cuộc họp: 1 phút
2. AI gom tài liệu, thread, task: 1 phút
3. AI tạo meeting brief: 1 phút
4. Người dùng review/chỉnh: 1 phút

### Human boundary

AI chỉ tổng hợp và đề xuất. Người dùng quyết định nội dung nào đáng tin, câu hỏi nào cần đưa vào họp, và không tự động gửi hoặc chia sẻ brief ra ngoài.

### Fallback

Nếu AI không tìm đủ context hoặc đưa nhầm tài liệu, người dùng quay lại Calendar, search và template chuẩn bị thủ công.

## Problem Card #2 và #3 — tóm tắt

| Card | Actor | Bottleneck | Metric | Quick gut | Vì sao chưa chọn làm #1 |
|---|---|---|---|---|---|
| Trợ lý phân loại và trả lời email/tin nhắn | Sales, CSKH, PM, nhân viên văn phòng | Đọc từng tin, xác định mức ưu tiên, tìm context rồi soạn phản hồi | Giảm thời gian xử lý inbox; giảm số tin quá hạn; tăng tốc độ phản hồi đầu tiên | Workflow / Agent | Rủi ro gửi sai, sai tone hoặc bỏ sót thông tin quan trọng; nên bắt đầu từ phân loại và draft thay vì auto-send |
| Phân tích hành vi người mua TMĐT | Seller, brand manager, e-commerce team | Đọc review thủ công và khó liên kết comment với giá, đối thủ, campaign hoặc dữ liệu bán | Giảm thời gian tổng hợp insight; số insight được dùng; cải thiện rating, conversion hoặc tỷ lệ hoàn hàng | Analysis workflow | Cần xác định nguồn dữ liệu và chứng minh insight tạo ra hành động kinh doanh thực tế |

## Problem Card bổ sung — Phát hiện trẻ em/thú cưng bị kẹt trong xe

### Problem 1 câu

Người lái có thể rời xe mà không nhận ra trẻ em hoặc thú cưng vẫn ở trong khoang xe, tạo ra rủi ro nghiêm trọng khi nhiệt độ tăng nhanh.

### Actor

Phụ huynh, chủ thú cưng, tài xế gia đình; đối tượng chịu ảnh hưởng trực tiếp là trẻ em và thú cưng.

### Bottleneck

Con người dựa vào trí nhớ và thói quen kiểm tra xe, vốn có thể thất bại khi mệt mỏi, mất tập trung hoặc thay đổi lịch sinh hoạt.

### Impact

Đây là pain có tần suất không nhất thiết cao nhưng hậu quả cực lớn. Vì vậy metric không thể chỉ là “tiết kiệm thời gian” mà phải ưu tiên phát hiện đáng tin cậy và cảnh báo kịp thời.

### Success metric

- Phát hiện đúng sự hiện diện trong các điều kiện vận hành đã kiểm thử.
- Cảnh báo đến tài xế trong thời gian rất ngắn sau khi xe tắt/khóa.
- Tỷ lệ cảnh báo giả đủ thấp để người dùng không tắt tính năng.
- Có cơ chế escalation khi tài xế không phản hồi, phù hợp quy định địa phương.

### Non-AI alternative

Cảnh báo kiểm tra hàng ghế sau khi tắt máy, nhắc nhở qua app, quy trình vật lý như để túi xách ở ghế sau. Đây là các biện pháp nên luôn tồn tại song song.

### AI hypothesis

Kết hợp cảm biến hiện diện trong xe, tín hiệu ghế, camera hoặc radar để xác định khả năng có người/thú cưng còn lại; hệ thống chỉ hỗ trợ cảnh báo, không được quảng bá là biện pháp an toàn duy nhất.

### Quick gut

Safety-critical system, không nên là MVP phần mềm thuần túy nếu chưa có năng lực phần cứng, kiểm thử và tuân thủ an toàn.

## Problem Card bổ sung — Trợ lý nhắc việc cá nhân hóa

### Problem 1 câu

Người dùng có nhiều việc cần làm nhưng reminder hiện tại chủ yếu dựa trên thời gian cố định, không hiểu mức ưu tiên, lịch làm việc, vị trí hay thói quen nên thường bị bỏ qua.

### Actor

Người đi làm bận rộn, sinh viên, phụ huynh và người quản lý nhiều đầu việc cá nhân.

### Bottleneck

Người dùng phải tự quyết định khi nào cần nhắc, nhắc bao nhiêu lần và việc nào quan trọng hơn; khi lịch thay đổi, reminder trở nên lỗi thời.

### Impact

Các việc nhỏ bị quên, deadline bị trễ và người dùng mất niềm tin vào hệ thống nhắc việc vì nhận quá nhiều thông báo không đúng lúc.

### Success metric

- Tăng tỷ lệ hoàn thành việc đúng hạn.
- Giảm tỷ lệ snooze hoặc dismiss reminder.
- Người dùng giữ lại hoặc chủ động dùng lại các gợi ý của AI.
- Giảm số thông báo nhưng không giảm tỷ lệ hoàn thành.

### Non-AI alternative

Dùng time blocking, Eisenhower matrix, recurring reminders và weekly review. Đây là giải pháp đơn giản, đáng thử trước khi xây lớp AI phức tạp.

### AI hypothesis

AI đọc task, deadline, calendar và lựa chọn cá nhân của người dùng để đề xuất thời điểm nhắc phù hợp, ví dụ nhắc chuẩn bị tài liệu khi có khoảng trống 30 phút trước cuộc họp thay vì nhắc đúng 9 giờ sáng.

### Quick gut

Personalization workflow, nhưng cần chọn một nhóm người dùng thật hẹp để tránh trở thành một to-do app chung chung.