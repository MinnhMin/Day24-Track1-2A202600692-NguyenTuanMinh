# Case 1 — Chatbot AI trả lời sai thông tin bầu cử Mỹ 2024

## Brief Case

| Field | Nội dung |
|---|---|
| Tên case | AI Democracy Projects / Proof News — Election Chatbot Inaccuracy |
| Ngành | Media / News / Social / Political assistant |
| Tổ chức / sản phẩm | Google Gemini, OpenAI GPT-4, Meta Llama 2, Mistral Mixtral, Anthropic Claude (5 mô hình được kiểm thử) |
| Use case AI | Người dùng hỏi chatbot các câu hỏi thực tế về quy trình bầu cử sơ bộ Mỹ 2024 (nơi bỏ phiếu, cách đăng ký, deadline...) |
| Thời điểm | Tháng 2/2024 (công bố trước Super Tuesday) |
| Case xảy ra chuyện gì? | Tổ chức AI Democracy Projects và Proof News, phối hợp với các quan chức bầu cử lưỡng đảng, kiểm thử 5 chatbot AI bằng câu hỏi thực tế về bầu cử. Kết quả: hơn một nửa câu trả lời không chính xác, có trường hợp bịa ra dịch vụ "bỏ phiếu qua SMS" không tồn tại ở California. Ở Nevada, 4/5 chatbot khẳng định sai rằng cử tri sẽ không được đăng ký cùng ngày dù luật bang cho phép từ 2019. |
| Stakeholder bị ảnh hưởng | Cử tri phổ thông (đặc biệt người dựa vào chatbot thay vì nguồn chính thức), cơ quan bầu cử bang, quy trình dân chủ nói chung |
| Số liệu chính | Gemini sai gần 2/3 số câu trả lời (~65%); một nghiên cứu liên quan (GroundTruthAI) ghi nhận tỉ lệ sai trung bình 27% trên 2.784 câu trả lời từ 216 câu hỏi; nghiên cứu của Center for Democracy & Technology ghi nhận hơn 1/3 trong 77 câu hỏi có thông tin sai |
| Trích nguồn ngắn | Theo điều tra của AI Democracy Projects/Proof News, Gemini, Llama 2 và Mixtral có tỉ lệ trả lời sai cao nhất, Gemini sai gần hai phần ba câu hỏi. |
| Nguồn 1 | CBS News, "AI chatbots are serving up wildly inaccurate election information, new study says" — 28/02/2024 — https://www.cbsnews.com/news/ai-chatbots-inaccurate-election-information-proof-news/ |
| Nguồn 2 | NBC News, "AI chatbots got questions about the 2024 election wrong 27% of the time, study finds" — 07/06/2024 — https://www.nbcnews.com/tech/tech-news/ai-chatbots-got-questions-2024-election-wrong-27-time-study-finds-rcna155640 |
| Ghi chú độ tin cậy | Primary/high-quality: nghiên cứu được thực hiện bởi tổ chức phi lợi nhuận chuyên trách (Proof News, CDT) phối hợp quan chức bầu cử thật; 2 nguồn độc lập không mâu thuẫn, chỉ khác về tỉ lệ % cụ thể do phương pháp/thời điểm khảo sát khác nhau. |

## Harm Map Worksheet

| Trường | Nội dung |
|---|---|
| High-risk moment | Cử tri hỏi chatbot về thủ tục/nơi/điều kiện bỏ phiếu gần ngày bầu cử, không kiểm tra lại với nguồn chính thức |
| Stakeholder bị ảnh hưởng | Cử tri (đặc biệt cử tri lần đầu, ít thời gian tra cứu), tính toàn vẹn của quy trình bầu cử |
| Failure mode | Hallucination (bịa dịch vụ bỏ phiếu SMS không tồn tại) |
| Layer bắt đầu lỗi | Grounding (mô hình không được kết nối với dữ liệu bầu cử cập nhật, chính xác theo từng bang) |
| Harm xảy ra là gì? | Cử tri bị hướng dẫn sai dẫn đến mất quyền bỏ phiếu hoặc bỏ phiếu sai quy trình |
| Harm lens | Misinformation; Opportunity loss (mất cơ hội thực hiện quyền bầu cử) |
| Severity | High — mất quyền bầu cử là hậu quả nghiêm trọng dù không gây hại thể chất trực tiếp |
| Scale | High — hàng triệu cử tri Mỹ có thể tiếp cận các chatbot phổ biến này trong mùa bầu cử |
| Probability | High — nghiên cứu cho thấy tỉ lệ sai từ 27% đến hơn 50% tùy mô hình và bộ câu hỏi |
| Frequency | Medium-High — lỗi lặp lại nhất quán qua nhiều lần hỏi cùng câu hỏi, không phải ngẫu nhiên hiếm gặp |
| Vì sao? | Severity cao vì ảnh hưởng quyền công dân cốt lõi và khó "sửa lại" sau khi cử tri đã bỏ lỡ deadline; Scale cao vì các chatbot này có hàng trăm triệu người dùng hoạt động; Probability/Frequency cao vì nhiều nghiên cứu độc lập, ở nhiều thời điểm khác nhau đều cho kết quả tỉ lệ sai đáng kể, cho thấy đây là vấn đề mang tính hệ thống chứ không phải lỗi đơn lẻ. |