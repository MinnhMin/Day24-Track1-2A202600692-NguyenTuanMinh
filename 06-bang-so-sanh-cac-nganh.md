# Bước 6 — Bảng so sánh Risk Profile giữa các ngành (file tổng hợp của nhóm)

> Lưu ý: Đây là file dùng chung cho cả bàn — sau khi mỗi thành viên share case của mình (Bước 5), điền tiếp các dòng còn lại của bảng dưới. Hàng "Media / news / social / political assistant" đã được điền sẵn dựa trên 3 case ở trên, dùng làm tham chiếu.

<!-- [Antigravity COMMENT]: Bổ sung danh sách các case study được chia sẻ bởi các thành viên trong bàn theo Bước 5 và yêu cầu trong file PDF hướng dẫn -->
## 1. Danh sách các case study được chia sẻ bởi các thành viên trong bàn

| Thành viên | Ngành | Các case study chính đã chia sẻ |
|---|---|---|
| **Đỗ Tuấn Đạt** | Y tế / symptom checker / health assistant | 1. **Epic Sepsis Model**: AI cảnh báo nhiễm trùng huyết sai lệch.<br>2. **IBM Watson for Oncology**: Gợi ý phác đồ điều trị ung thư không an toàn.<br>3. **NEDA Tessa chatbot**: Đưa lời khuyên ăn uống độc hại cho người rối loạn ăn uống. |
| **Đặng Trần Đạt** | Content creator | 1. **Getty Images v. Stability AI**: Bản quyền hình ảnh huấn luyện AI.<br>2. **CNET AI-generated articles**: Bịa thông tin tài chính cá nhân trong bài viết SEO.<br>3. **Taylor Swift AI deepfake**: Ảnh khâu dâm giả danh chân dung người thật lan truyền. |
| **Cao Văn Hảo** | Media / news / social / political assistant | 1. **CNET AI finance articles**: Sai sót trong xuất bản nội dung tài chính.<br>2. **Biden AI robocall NH**: Giọng nói AI giả dạng tổng thống để phá hoại bầu cử.<br>3. **Facebook/Meta Rohingya hate speech**: Thuật toán khuếch đại ngôn từ thù ghét sắc tộc. |
| **Nguyễn Tuấn Minh** (Tôi) | Media / news / social / political assistant | 1. **AI Democracy Projects/Proof News**: Chatbot AI trả lời sai thông tin bầu cử Mỹ 2024.<br>2. **Grok antisemitic incident**: Chatbot tự tạo nội dung bài Do Thái.<br>3. **Sports Illustrated fake authors**: Sử dụng tác giả AI giả mạo không công bố. |
| **Đàm Xuân Giáp** | Content creator | 1. **NYT v. OpenAI & Microsoft**: Bản quyền nội dung báo chí dùng train LLM.<br>2. **"Heart on My Sleeve"**: Deepfake giọng ca sĩ Drake và The Weeknd.<br>3. **CNET AI articles**: Bài viết SEO tài chính chứa thông tin sai lệch. |

<br>

<!-- [Antigravity COMMENT]: Bổ sung kết quả phân tích các ngành HR, Giáo dục, Y tế, Mobility và Content creator từ hoạt động thảo luận nhóm và các repo thành viên -->
## 2. Bảng so sánh Risk Profile giữa các ngành

| Ngành | Harm dễ gặp nhất | Failure mode hay lặp lại | Layer hay bắt đầu lỗi | Risk profile tổng thể | Vì sao? |
|---|---|---|---|---|---|
| **HR / tuyển dụng** | Opportunity loss (mất cơ hội), dignity loss, fairness/legal harm | Bias/fairness, proxy discrimination, over-reliance vào score | Data, Model, UX, Policy | **High** | AI ảnh hưởng trực tiếp đến cơ hội việc làm và phát triển nghề nghiệp. Sự thiên lệch (bias) trong lọc hồ sơ hoặc chấm điểm có thể loại bỏ ứng viên đủ điều kiện một cách oan uổng và tạo rủi ro pháp lý cho doanh nghiệp. |
| **Giáo dục / AI tutor** | Misinformation, over-reliance (quá phụ thuộc), unequal support | Hallucination, sycophancy, harmful learning shortcut | Model, UX, Grounding | **Medium-High** | AI tutor giúp cá nhân hóa việc học nhưng dễ bịa tin (hallucination) khiến học sinh hiểu sai kiến thức, hoặc có xu hướng chiều lòng (sycophancy) làm giảm tư duy phản biện. Học sinh có thể lạm dụng để chép bài thay vì tự học. |
| **Y tế / symptom checker / health assistant** | Injury, delayed intervention (chậm can thiệp), harmful advice, privacy loss | Harmful advice, false negative, over-reliance, escalation failure | Safety, Grounding, Model, UX, Governance | **Critical** | Lỗi sai có thể dẫn tới hậu quả về thể chất nguy hại (bỏ sót triệu chứng nhiễm trùng huyết sepsis, phác đồ điều trị ung thư không an toàn, lời khuyên ăn kiêng độc hại cho người rối loạn ăn uống). Đòi hỏi tính bảo mật dữ liệu y tế cực kỳ cao và cơ chế chuyển tiếp sang bác sĩ thật. |
| **Mobility / autonomous driving** | Physical injury (chấn thương thể chất), system reliability harm | Perception failure, planning failure, escalation/fail-safe failure | Sensor, Model, Safety, System architecture | **Critical** | Vận hành trực tiếp thiết bị cơ giới trong môi trường thực tế, sai sót lập tức đe dọa sinh mạng con người (tai nạn va chạm). Cần kiểm thử an toàn cực kỳ khắt khe, lớp phòng vệ vật lý (fail-safe) và hệ thống dự phòng tốt. |
| **Media / news / social / political assistant** | Misinformation, mất niềm tin công chúng, dignity loss khi leo thang (vd. nội dung thù ghét) | Hallucination; Misuse/jailbreak kết hợp Bias/fairness | Trải đều: Grounding, Safety, UX | **High** | Scale và Frequency rất cao do quy mô người dùng nền tảng lớn và tốc độ lan truyền; Severity thường ở mức Medium–High nhưng có thể leo thang lên Critical khi guardrail bị lỗi (case Grok); hậu quả khó đảo ngược hoàn toàn vì nội dung đã lan truyền không thể thu hồi triệt để. |
| **Content creator** | Copyright harm (bản quyền), reputation harm, misinformation, privacy/dignity loss | Hallucination, plagiarism/provenance failure, misuse/deepfake, over-reliance | Data governance, Grounding, Editorial QA, Safety, Platform moderation | **High** | Quy mô sản xuất và phân phối nội dung AI cực nhanh và lớn. Rủi ro tranh chấp bản quyền tác phẩm (vụ kiện tranh chấp tranh/ảnh/nhạc AI) và việc lạm dụng deepfake/synthetic media làm suy giảm nghiêm trọng uy tín cá nhân/thương hiệu. |

<br>

<!-- [Antigravity COMMENT]: Bổ sung phần tổng hợp ngắn so sánh risk profile giữa các ngành từ thảo luận của nhóm (giải quyết 6 câu hỏi thảo luận trong file PDF hướng dẫn) -->
## 3. Đoạn tổng hợp ngắn về risk profile giữa các ngành

- **Severity cao nhất:** Ngành **Y tế** và **Mobility** có mức độ nghiêm trọng tiềm năng cao nhất vì lỗi hệ thống có thể trực tiếp đe dọa đến tính mạng, sức khỏe vật lý (physical harm) của con người và rất khó đảo ngược hậu quả. Ngành **Media** cũng có thể chạm mức Critical khi tin giả kích hoạt bạo lực ngoài đời thực hoặc phá hoại quy trình dân chủ (bầu cử).
- **Scale lớn nhất:** Ngành **Media** và **Content creator** dẫn đầu do nội dung do AI tạo ra có thể lan truyền qua mạng xã hội, công cụ tìm kiếm và các kênh phân phối tự động hóa đến hàng triệu người dùng trong tích tắc (blast radius cực rộng).
- **Probability hoặc Frequency cao nhất:** Ngành **Content creator** và **Giáo dục** có tần suất xảy ra cao nhất vì người dùng tương tác liên tục hàng giờ (tạo nội dung hàng loạt, học sinh hỏi đáp hàng ngày). Nếu mô hình có thiên hướng hallucination hoặc sycophancy, lỗi sẽ lặp lại với tần suất rất cao.
- **Xử lý dữ liệu nhạy cảm rõ nhất:** Ngành **Y tế** (bệnh án bệnh nhân) và **HR** (lương, giới tính, thông tin nhân thân ứng viên) xử lý nhiều dữ liệu nhạy cảm pháp lý nhất. Kế đó là **Content creator** và **Media** khi dùng giọng nói, hình ảnh chân dung người thật (dễ vướng deepfake không đồng thuận).
- **Cần human-in-the-loop rõ nhất:** Ngành **Y tế, Mobility và HR** cần sự giám sát của con người nghiêm ngặt nhất ở khâu quyết định cuối cùng (chẩn đoán bệnh, điều khiển xe, tuyển dụng). Với **Media và Content creator**, sự can thiệp của con người (Editorial QA) là thiết yếu trước khi xuất bản nội dung nhạy cảm liên quan bầu cử, y tế hoặc thương hiệu.
- **Cần bar "được ship" (Release bar) cao nhất:** Ngành **Y tế** và **Mobility** bắt buộc phải có tiêu chuẩn xuất xưởng khắt khe nhất để phòng ngừa các rủi ro nguy hiểm đến tính mạng. Tiếp theo là **HR** (đảm bảo tính công bằng pháp lý) và **Media** (đảm bảo thông tin xác thực).

