# Bước 5 (phần cá nhân) — Tổng hợp pattern rủi ro ngành Media / News / Social / Political Assistant

Ba case trên cho thấy ngành media/political assistant có pattern rủi ro khác biệt rõ rệt so với các ngành "thể chất" như y tế hay mobility: **Severity tức thời thấp hơn nhưng Scale và Frequency lại rất cao**, vì sản phẩm vận hành trên nền tảng có hàng trăm triệu đến hàng tỷ người dùng và nội dung lan truyền gần như tức thì.

**Failure mode lặp lại nhiều nhất:** Hallucination (case 1 — bịa thông tin bầu cử) và Misuse/jailbreak kết hợp Bias (case 2 — Grok bị khai thác để tạo nội dung bài Do Thái). Cả hai đều cho thấy mô hình dễ bị đẩy lệch khi thiếu grounding chắc chắn (dữ liệu bầu cử theo từng bang) hoặc khi lớp guardrail/safety bị thay đổi mà không kiểm thử kỹ.

**Layer hay bắt đầu lỗi:** phân bố đều ở cả ba lớp — Grounding (case 1, thiếu dữ liệu xác thực theo thời gian thực), Safety (case 2, guardrail bị nới lỏng do thay đổi cấu hình), và UX (case 3, thiếu disclosure về nguồn gốc nội dung do AI tạo). Điều này cho thấy rủi ro trong ngành không tập trung ở một điểm kỹ thuật duy nhất mà trải dài toàn bộ pipeline, từ dữ liệu đầu vào đến cách trình bày đầu ra cho người dùng cuối.

**Harm chính:** misinformation và mất niềm tin công chúng là hai harm lens xuất hiện ở cả 3 case, đúng với gợi ý ban đầu của ngành. Đặc biệt, case Grok cho thấy harm có thể leo thang từ "thông tin sai" sang "dignity loss/kích động thù ghét" — mức Severity Critical hiếm gặp trong ngành này nhưng khi xảy ra thì hậu quả xã hội rất khó đảo ngược.

**Nếu là team sản phẩm, điều cần sửa trước:** ưu tiên xây cơ chế grounding thời gian thực cho các chủ đề nhạy cảm về quyền công dân (bầu cử), thiết lập quy trình review/staging bắt buộc trước khi đẩy bất kỳ thay đổi nào vào lớp safety/system prompt của chatbot công khai, và bắt buộc disclosure rõ ràng khi nội dung có sự tham gia của AI — đây là ba điểm chặn rẻ nhất nhưng giảm được phần lớn rủi ro quan sát được trong cả 3 case.