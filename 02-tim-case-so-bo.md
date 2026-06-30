# Bước 2 — Tìm case study sơ bộ (Media / News / Social / Political Assistant)

Tìm 7 case sơ bộ trong ngành (đề bài yêu cầu 5-8), liệt kê nguồn cụ thể để tự kiểm tra lại, sau đó lọc xuống 3 case mạnh nhất để làm Brief Case + Harm Map ở Bước 3-4.

## Danh sách 7 case sơ bộ

### 1. AI Democracy Projects / Proof News — chatbot trả lời sai về bầu cử Mỹ 2024
- Tóm tắt: 5 chatbot lớn (Gemini, GPT-4, Llama 2, Mixtral...) trả lời sai hơn nửa câu hỏi về thủ tục bầu cử
- Số liệu: có (tỉ lệ sai cụ thể theo từng model)
- Nguồn:
  - CBS News: https://www.cbsnews.com/news/ai-chatbots-inaccurate-election-information-proof-news/
  - NBC News: https://www.nbcnews.com/tech/tech-news/ai-chatbots-got-questions-2024-election-wrong-27-time-study-finds-rcna155640
  - Fortune: https://fortune.com/2024/02/27/election-misinformation-genai-chatbots-google-openai/
- **Quyết định: Giữ — Case 1**

### 2. Grok (xAI) đăng nội dung bài Do Thái, ca ngợi Hitler trên X
- Tóm tắt: sau bản cập nhật lỗi, Grok đăng hàng loạt nội dung cực đoan trong 16 giờ
- Số liệu: có (thời lượng sự cố, phản ứng của 2 quốc gia)
- Nguồn:
  - CNN Business: https://www.cnn.com/2025/07/12/tech/xai-apology-antisemitic-grok-social-media-posts
  - NPR: https://www.npr.org/2025/07/09/nx-s1-5462609/grok-elon-musk-antisemitic-racist-content
  - TIME: https://time.com/7301206/elon-musk-antisemitic-posts-ai-chatbot-grok-response/
- **Quyết định: Giữ — Case 2**

### 3. Sports Illustrated đăng bài với tác giả AI giả mạo
- Tóm tắt: bài đánh giá sản phẩm gắn tên/ảnh tác giả không có thật do AI tạo
- Số liệu: có (số bài bị gỡ, số vụ tương tự cùng năm trong ngành)
- Nguồn:
  - Futurism (điều tra gốc): https://futurism.com/sports-illustrated-ai-generated-writers
  - CNN Business: https://www.cnn.com/2023/11/27/media/sports-illustrated-deletes-articles-fake-author-names-ai-profile-photos/index.html
  - NPR: https://www.npr.org/2023/11/28/1215693615/sports-illustrated-is-accused-of-posting-articles-by-writers-created-by-ai
- **Quyết định: Giữ — Case 3**

### 4. Microsoft Tay — chatbot bị dạy nói phân biệt chủng tộc, bài Do Thái (2016)
- Tóm tắt: chatbot Twitter bị người dùng "huấn luyện" nói nội dung phân biệt chủng tộc, ca ngợi Hitler, bị gỡ trong vòng 16-24 giờ
- Số liệu: có nhưng case khá cũ (2016)
- Nguồn:
  - CBS News: https://www.cbsnews.com/news/microsoft-shuts-down-ai-chatbot-after-it-turned-into-racist-nazi/
  - TechCrunch: https://techcrunch.com/2016/03/24/microsoft-silences-its-new-a-i-bot-tay-after-twitter-users-teach-it-racism/
  - AI Incident Database: https://incidentdatabase.ai/cite/6/
- **Quyết định: Loại** — case cũ (2016), trùng failure mode (Misuse/jailbreak + Bias) với Case 2 (Grok), giữ 1 case đại diện cho nhóm lỗi này là đủ

### 5. Google AI Overviews đưa thông tin sai trong kết quả tìm kiếm (2024)
- Tóm tắt: AI Overviews gợi ý cho keo vào pizza, ăn đá mỗi ngày, nói sai về tổng thống Mỹ
- Số liệu: có ví dụ cụ thể nhưng thiếu số liệu thống kê tổng thể (chủ yếu là case viral lẻ tẻ)
- Nguồn:
  - Live Science: https://www.livescience.com/technology/artificial-intelligence/googles-ai-tells-users-to-add-glue-to-their-pizza-eat-rocks-and-make-chlorine-gas
  - MIT Technology Review: https://www.technologyreview.com/2024/05/31/1093019/why-are-googles-ai-overviews-results-so-bad/
- **Quyết định: Loại** — thiếu số liệu định lượng tổng thể mạnh bằng 3 case đã chọn (chủ yếu dựa vào ví dụ viral trên mạng xã hội)

### 6. Google Gemini tạo ảnh lịch sử sai lệch chủng tộc (2/2024)
- Tóm tắt: Gemini tạo ảnh nhân vật lịch sử (lính Đức Quốc xã, Founding Fathers Mỹ) với chủng tộc sai lệch lịch sử, Google phải tạm dừng tính năng
- Số liệu: có (Google chính thức tạm dừng tính năng tạo ảnh người)
- Nguồn:
  - NBC News: https://www.nbcnews.com/tech/tech-news/google-making-changes-gemini-ai-portrayed-people-color-inaccurately-rcna140007
  - CNBC: https://www.cnbc.com/2024/02/22/google-pauses-gemini-ai-image-generator-after-inaccuracies.html
  - Al Jazeera: https://www.aljazeera.com/news/2024/3/9/why-google-gemini-wont-show-you-white-people
- **Quyết định: Loại** — bản chất lỗi (guardrail/bias bị chỉnh sai hướng) khá giống case Grok (Case 2), giữ Grok làm đại diện vì mức độ harm nghiêm trọng hơn (nội dung thù ghét thật so với lỗi tạo ảnh)

### 7. NewsGuard — chatbot AI lặp lại tuyên truyền tin giả mạng lưới Pravda (Nga)
- Tóm tắt: 10 chatbot lớn (ChatGPT, Gemini, Copilot, Grok, Claude...) lặp lại narrative tuyên truyền từ mạng lưới Pravda thân Nga trung bình 33% số lần được hỏi
- Số liệu: có (33% / 33.55%, 450 câu trả lời được kiểm thử, 3,6 triệu bài viết tuyên truyền năm 2024)
- Nguồn:
  - NewsGuard (báo cáo gốc): https://www.newsguardtech.com/special-reports/moscow-based-global-news-network-infected-western-artificial-intelligence-russian-propaganda/
  - The Hill: https://thehill.com/policy/technology/5181257-ai-chatbots-infected-with-russian-disinformation-study/
  - Forbes: https://www.forbes.com/sites/torconstantino/2025/03/10/russian-propaganda-has-now-infected-western-ai-chatbots---new-study/
- **Quyết định: Loại** — gần giống Case 1 về bản chất (misinformation do thiếu grounding/dễ bị thao túng nguồn dữ liệu), giữ Case 1 làm đại diện cho nhóm lỗi "misinformation lan rộng do thiếu grounding"

## Lý do chọn 3 case cuối cùng (Case 1, 2, 3)

Ba case được giữ lại vì: (a) mỗi case minh hoạ một **failure mode và layer lỗi khác nhau** (Hallucination/Grounding — Misuse+Bias/Safety — Misuse/UX), tránh trùng lặp với các case bị loại (case 4, 6 trùng nhóm với case 2; case 7 trùng nhóm với case 1); (b) cả 3 đều có số liệu định lượng rõ ràng và nguồn sơ cấp/chất lượng cao, đủ dữ kiện điền Harm Map Worksheet đầy đủ; (c) trải dài về thời gian (2023–2025) và loại tổ chức (báo chí truyền thống, social platform, nghiên cứu độc lập có quan chức bầu cử tham gia), cho góc nhìn toàn diện hơn về ngành.