# Group Report — Day 02

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm |
|-----|-----------|-------------|--------------------|
| 1 | Phạm Xuân Phong | 2A202602027 | Thành viên |
| 2 | Bùi Hoàng Vương | 2A202601553 | Trưởng nhóm |
| 3 | Đặng Tiến Thành | 2A202601305 | Thành viên đề xuất |
| 4 | Ngô Thành Đạt | 2A202601323 | Thành viên |
| 5 | Nguyễn Chí Quang | 2A202601932 | Thành viên đề xuất |
| 5 | Nguyễn Chí Quang | 2A202601932 | Thành viên đề xuất |

1) Nhật ký hội tụ

Qua quá trình thảo luận, nhóm dần hội tụ về một vấn đề rất rõ: SMEs và freelancer bán hàng trên thương mại điện tử đang thiếu một công cụ AI đủ rẻ, đủ sâu và đủ sát thực tế để phân tích hành vi khách hàng từ comment. Các giải pháp analytics hiện có thường quá đắt, chỉ cho insight tổng quan, chưa đi sâu vào những tín hiệu thật sự quan trọng như nhu cầu, phản đối, do dự, ý định mua và cảm xúc của khách hàng. Vì vậy, nhóm xác định trọng tâm không phải là “xây AI cho có”, mà là xây một hệ thống AI tập trung vào comment như nguồn dữ liệu hành vi giàu giá trị nhất.
2) Validation / Research

Từ research ban đầu, nhóm nhận thấy comment là một nguồn dữ liệu cực kỳ quan trọng trong thương mại điện tử vì nó phản ánh trực tiếp suy nghĩ thật của khách hàng. Trong comment có thể tìm thấy các dấu hiệu như: khách đang quan tâm điều gì, họ lăn tăn điểm nào, lý do họ chưa mua, lý do họ quay lại hỏi thêm, và những yếu tố nào ảnh hưởng đến quyết định mua hàng. Tuy nhiên, phần lớn công cụ hiện nay либо chỉ dừng ở việc đếm số lượng comment, phân tích cảm xúc rất nông, chưa chuyển được dữ liệu này thành insight hành động cho người bán. Điều đó cho thấy bài toán là có thật, có nhu cầu thật, và còn khoảng trống lớn để AI giải quyết.
3) Workflow trước / sau

Trước khi có AI, người bán thường phải tự đọc từng comment, tự phân loại câu hỏi, tự đoán cảm xúc khách hàng và tự rút ra insight thủ công. Cách này vừa tốn thời gian, vừa dễ bỏ sót tín hiệu quan trọng, nhất là khi số lượng comment tăng nhanh theo từng chiến dịch bán hàng.
Sau khi có AI, hệ thống có thể tự động thu thập comment, phân loại theo chủ đề, nhận diện sentiment, phát hiện câu hỏi lặp lại, tìm pain point và tóm tắt các xu hướng hành vi khách hàng. Nhờ đó, người bán không chỉ nhìn thấy “khách đang nói gì” mà còn hiểu được “vì sao họ nói như vậy” và “nên làm gì tiếp theo”.
4) Rule / Workflow / Agent

Nhóm định hướng triển khai theo thứ tự Rule → Workflow → Agent.

    Ở tầng Rule, hệ thống cần xác định rõ các tiêu chí như comment nào là câu hỏi, comment nào là phàn nàn, comment nào thể hiện ý định mua, comment nào là spam.

    Ở tầng Workflow, AI sẽ hỗ trợ tự động hóa các bước thu thập, làm sạch, gắn nhãn, tổng hợp và xuất báo cáo insight.

    Ở tầng Agent, hệ thống có thể tiến xa hơn bằng cách đề xuất hành động tiếp theo, ví dụ: gợi ý trả lời comment, gợi ý cải thiện nội dung sản phẩm, hoặc cảnh báo xu hướng phản hồi tiêu cực đang tăng.

Cách đi này giúp nhóm không sa vào xây agent quá sớm, mà đi từ quy trình rõ ràng rồi mới nâng cấp mức độ tự động hóa.
5) Quyết định Go / Not Yet / No-Go

Go khi bài toán kinh doanh đã rõ, dữ liệu comment có thể thu thập được, và hệ thống có thể tạo ra insight hữu ích cho SMEs/freelancer với chi phí hợp lý.
Not Yet khi nhu cầu đã có nhưng dữ liệu chưa đủ sạch, rule phân loại chưa ổn định, hoặc cần thêm vòng validation để kiểm tra độ chính xác của phân tích.
No-Go khi use case không tạo ra giá trị thực tế, chi phí triển khai cao hơn lợi ích, hoặc dữ liệu đầu vào quá thiếu chất lượng để AI phân tích đáng tin cậy.
6) Problem Statement

SMEs và freelancer bán hàng trên thương mại điện tử hiện chưa có một giải pháp AI phù hợp về chi phí và chiều sâu để phân tích hành vi khách hàng từ comment. Trong khi đó, comment là một nguồn dữ liệu quan trọng phản ánh cảm xúc, nhu cầu, nỗi lo và ý định mua của khách hàng. Nếu khai thác tốt dữ liệu này, người bán có thể hiểu khách hàng sâu hơn, tối ưu nội dung bán hàng, cải thiện sản phẩm và tăng hiệu quả chuyển đổi. Vì vậy, nhóm chọn xây dựng một hệ thống AI tập trung vào phân tích comment nhằm biến dữ liệu thô thành insight hành động cho người bán nhỏ.