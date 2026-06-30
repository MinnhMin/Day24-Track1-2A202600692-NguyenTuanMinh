# Day24-Track1-MaHV-HoVaTen

Bài nộp Day 24 Lab — Case Study Hunt và Harm Map theo ngành.

- **Học viên:** Nguyễn Tuấn Minh
- **Mã học viên:** 2A202600692
- **Ngành đã chọn:** Media / News / Social / Political
- **Ngày nộp:** 30/06/2026

## Mục tiêu bài lab

Tìm case study AI có thật trong ngành đã chọn, tóm tắt fact/số liệu/nguồn, phân tích bằng Harm Map (failure mode, layer lỗi, harm, Severity, Scale, Probability, Frequency), và so sánh risk profile với các ngành khác mà cả bàn đã làm.

## Cây thư mục

```
Day24-Track1-MaHV-HoVaTen/
├── README.md
├── 01-industry-risk-snapshot.md
├── 02-tim-case-so-bo.md
├── brief-case-harm-map/
│   ├── case-1-election-chatbot-misinformation.md
│   ├── case-2-grok-antisemitic-incident.md
│   └── case-3-sports-illustrated-fake-authors.md
├── 05-tong-hop-pattern-nganh.md
└── 06-bang-so-sanh-cac-nganh.md
```

## Cấu trúc repo (theo đúng 6 bước của đề bài)

| File / Thư mục | Tương ứng bước | Nội dung |
|---|---|---|
| `01-industry-risk-snapshot.md` | Bước 1 | Chấm điểm Risk Profile sơ bộ của ngành Media trước khi tìm case (Low/Medium/High/Critical cho 6 câu hỏi + risk profile tổng thể) |
| `02-tim-case-so-bo.md` | Bước 2 | 7 case sơ bộ kèm nguồn để tự kiểm tra, lọc xuống 3 case mạnh nhất + lý do giữ/loại từng case |
| `brief-case-harm-map/case-1-election-chatbot-misinformation.md` | Bước 3 & 4 | Brief Case + Harm Map — chatbot AI trả lời sai thông tin bầu cử Mỹ 2024 (AI Democracy Projects / Proof News, 2/2024) |
| `brief-case-harm-map/case-2-grok-antisemitic-incident.md` | Bước 3 & 4 | Brief Case + Harm Map — Grok (xAI) đăng nội dung bài Do Thái trên X (7/2025) |
| `brief-case-harm-map/case-3-sports-illustrated-fake-authors.md` | Bước 3 & 4 | Brief Case + Harm Map — Sports Illustrated đăng bài với tác giả AI giả mạo (11/2023) |
| `05-tong-hop-pattern-nganh.md` | Bước 5 (phần cá nhân) | Đoạn tổng hợp ngắn về pattern rủi ro của ngành Media, rút ra từ 3 case trên |
| `06-bang-so-sanh-cac-nganh.md` | Bước 6 | Bảng so sánh risk profile giữa 6 ngành — **hiện là bản nháp/phân tích thử** dựa trên suy luận chung, cần thay bằng case thật của các thành viên cùng bàn trước khi hoàn thiện |


## Tóm tắt nhanh 3 case đã chọn

| # | Case | Thời điểm | Số liệu chính | Severity | Scale | Failure mode chính |
|---|---|---|---|---|---|---|
| 1 | Chatbot trả lời sai thông tin bầu cử Mỹ | 2/2024 | Tỉ lệ sai 27%–65% tùy mô hình (Gemini sai gần 2/3 câu hỏi) | High | High | Hallucination |
| 2 | Grok đăng nội dung bài Do Thái trên X | 7/2025 | Sự cố kéo dài 16 giờ; Ba Lan báo cáo EU, Thổ Nhĩ Kỳ chặn truy cập | Critical | High | Misuse/jailbreak + Bias |
| 3 | Sports Illustrated dùng tác giả AI giả mạo | 11/2023 | Nhiều bài bị gỡ; vụ thứ 3 cùng năm trong ngành báo chí (sau CNET, Gannett) | Medium | Medium | Misuse (giả danh tác giả) |

## Cách kiểm tra lại nguồn

Mỗi case trong `brief-case-harm-map/` và mỗi case sơ bộ trong `02-tim-case-so-bo.md` đều có link nguồn gốc (báo chí uy tín: CNN, NBC, NPR, CBS, Futurism, TIME, Fortune...). Trước khi nộp, hãy tự mở lại từng link, đối chiếu đúng các bước trong checklist kiểm nguồn của đề bài:

1. Đã mở nguồn thật chưa?
2. Số liệu nằm ở đâu trong nguồn?
3. Mốc thời gian có đúng không?
4. Đây là nguồn gốc hay nguồn trích lại?
5. Nếu có 2 nguồn, chúng có mâu thuẫn nhau không?

(Riêng case 3 có một điểm cần lưu ý khi đối chiếu: Arena Group/Sports Illustrated phủ nhận nội dung do AI viết, trong khi Futurism khẳng định có dấu hiệu AI — đã ghi rõ trong phần "Ghi chú độ tin cậy" của case này.)

## Việc còn cần làm trước khi nộp

1. Đổi tên thư mục/repo theo đúng mã học viên + họ tên thật, điền thông tin ở đầu README.
2. Tự kiểm tra lại từng nguồn theo checklist ở trên trước khi chốt nộp.
3. Hoàn thiện file `06-bang-so-sanh-cac-nganh.md`: thay 5 hàng còn lại (HR, Giáo dục, Y tế, Mobility, Content creator) bằng case thật của từng thành viên sau khi cả bàn share xong (Bước 5-6).
4. Đẩy repo lên GitHub (hoặc nền tảng được yêu cầu) và lấy link để nộp.
5. Kiểm tra lại không có API key, token, credential, hoặc dữ liệu cá nhân nhạy cảm nào trong repo.

## Lưu ý

- Không dùng ChatGPT, Claude, Perplexity làm nguồn của case — đúng yêu cầu đề bài, mọi case đều dẫn nguồn báo chí/điều tra gốc.
- Repo này không chứa bất kỳ API key, token, credential hay dữ liệu cá nhân nhạy cảm nào.