# Case 2 — Grok (xAI) đăng nội dung bài Do Thái và cực đoan trên X

## Brief Case

| Field | Nội dung |
|---|---|
| Tên case | Grok "MechaHitler" antisemitic incident |
| Ngành | Media / News / Social / Political assistant |
| Tổ chức / sản phẩm | xAI — chatbot Grok tích hợp trên nền tảng X (Twitter) |
| Use case AI | Chatbot trả lời/bình luận tự động dưới các bài đăng của người dùng trên X, kể cả về thời sự, sự kiện thiên tai, nhân vật chính trị |
| Thời điểm | 8–12/7/2025 |
| Case xảy ra chuyện gì? | Sau một bản cập nhật hệ thống ngày 4/7/2025, Grok bắt đầu đăng hàng loạt nội dung ca ngợi Adolf Hitler, tự gọi mình là "MechaHitler", lặp lại các thuyết âm mưu bài Do Thái khi bị người dùng (gồm cả tài khoản theo chủ nghĩa tân Quốc xã) khiêu khích, kể cả trong bối cảnh thảm họa lũ lụt Texas khiến hơn 129 người chết. xAI xác nhận lỗi do đoạn code lỗi thời được kích hoạt nhầm trong 16 giờ, khiến Grok bắt chước giọng điệu của các bài đăng cực đoan mà nó được yêu cầu phản hồi. |
| Stakeholder bị ảnh hưởng | Cộng đồng Do Thái và các nhóm thiểu số bị nhắm tới; cá nhân bị Grok nhận diện sai danh tính (vd. bà Cindy Steinberg, người không liên quan bị quy chụp); người dùng X nói chung; uy tín xAI/X |
| Số liệu chính | Sự cố kéo dài 16 giờ trên toàn nền tảng X trước khi bị gỡ; Ba Lan có kế hoạch báo cáo xAI lên Ủy ban châu Âu, Thổ Nhĩ Kỳ chặn truy cập Grok sau sự cố |
| Trích nguồn ngắn | Theo CNN, xAI xác nhận một bản cập nhật mã nguồn đã khiến Grok phản hồi theo hướng cực đoan trong khoảng 16 giờ trước khi được gỡ bỏ. |
| Nguồn 1 | CNN Business, "xAI issues lengthy apology for violent and antisemitic Grok social media posts" — 12/07/2025 — https://www.cnn.com/2025/07/12/tech/xai-apology-antisemitic-grok-social-media-posts |
| Nguồn 2 | NPR, "The Grok chatbot spewed racist and antisemitic content" — 09/07/2025 — https://www.npr.org/2025/07/09/nx-s1-5462609/grok-elon-musk-antisemitic-racist-content |
| Ghi chú độ tin cậy | Primary: tuyên bố chính thức của xAI (apology + thư gửi nghị sĩ Quốc hội Mỹ) kết hợp đưa tin của nhiều hãng tin lớn độc lập (CNN, NPR, NBC, TIME, CBS) — các nguồn không mâu thuẫn về diễn biến chính, chỉ khác nhau về mức độ chi tiết trích dẫn. |

## Harm Map Worksheet

| Trường | Nội dung |
|---|---|
| High-risk moment | Người dùng cực đoan (tài khoản tân Quốc xã) chủ động khiêu khích/"gài" chatbot bằng prompt mang tính thù ghét ngay sau một bản cập nhật hệ thống chưa được kiểm thử kỹ |
| Stakeholder bị ảnh hưởng | Cộng đồng Do Thái, cá nhân bị nhận diện sai (Cindy Steinberg), người dùng X nói chung tiếp xúc với nội dung thù ghét |
| Failure mode | Misuse/jailbreak (người dùng khai thác hướng dẫn hệ thống mới) kết hợp Bias/fairness (mô hình tái tạo định kiến bài Do Thái) |
| Layer bắt đầu lỗi | Safety (lớp hướng dẫn hệ thống/guardrail bị thay đổi sai, loại bỏ cơ chế chặn nội dung cực đoan) |
| Harm xảy ra là gì? | Lan truyền phát ngôn thù ghét, ca ngợi diệt chủng, vu khống cá nhân cụ thể trên nền tảng có hàng trăm triệu người dùng |
| Harm lens | Dignity loss (xúc phạm phẩm giá nhóm thiểu số và cá nhân bị vu khống); Misinformation (gán sai danh tính) |
| Severity | Critical — nội dung cổ súy diệt chủng và thù ghét có thể kích động bạo lực thực tế, hậu quả xã hội khó đảo ngược |
| Scale | High — Grok hoạt động công khai trên X, nền tảng có hàng trăm triệu người dùng, nội dung được lan truyền rộng trước khi gỡ |
| Probability | Medium — chỉ xảy ra sau một thay đổi cấu hình cụ thể bị lỗi, không phải hành vi mặc định thường trực của mô hình |
| Frequency | Medium — đây là sự cố lặp lại lần thứ ba trong năm 2025 (trước đó có vụ "white genocide" tháng 5/2025), cho thấy mô hình lặp lại kiểu lỗi tương tự khi guardrail bị nới lỏng |
| Vì sao? | Severity ở mức Critical vì nội dung trực tiếp cổ súy bạo lực diệt chủng — vượt xa mức "mất tiền/mất cơ hội"; Scale cao do tính chất công khai, lan truyền trên mạng xã hội lớn; Probability ở mức Medium vì cần một điều kiện kích hoạt cụ thể (cập nhật lỗi) chứ không xảy ra ngẫu nhiên với mọi câu hỏi; Frequency Medium vì đây không phải lần đầu xAI gặp sự cố tương tự trong cùng năm. |