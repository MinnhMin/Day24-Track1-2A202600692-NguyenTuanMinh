# Case 3 — Sports Illustrated đăng bài với tác giả AI giả mạo

## Brief Case

| Field | Nội dung |
|---|---|
| Tên case | Sports Illustrated AI-generated fake authors |
| Ngành | Media / News / Social / Political assistant (lấn sang Content creator, nhưng trọng tâm là khủng hoảng niềm tin báo chí) |
| Tổ chức / sản phẩm | Sports Illustrated (do The Arena Group vận hành), nội dung do bên thứ ba AdVon Commerce sản xuất |
| Use case AI | Viết bài đánh giá sản phẩm (product review) và tạo ảnh chân dung "tác giả" bằng AI để đăng kèm bài, tạo cảm giác bài viết do nhà báo thật viết |
| Thời điểm | Phát hiện và công bố tháng 11/2023 |
| Case xảy ra chuyện gì? | Trang Futurism điều tra và phát hiện Sports Illustrated đăng nhiều bài viết dưới tên tác giả không tồn tại ngoài đời (vd. "Drew Ortiz"), kèm ảnh đại diện do AI tạo, được tìm thấy đang rao bán trên các chợ ảnh AI. Khi Futurism liên hệ chất vấn, các "tác giả" này lặng lẽ biến mất khỏi website, bài viết được gán lại cho tác giả AI khác mà không có ghi chú giải trình. Arena Group phủ nhận nội dung do AI viết, đổ lỗi cho nhà thầu AdVon dùng "bút danh", nhưng thừa nhận và chấm dứt hợp tác với AdVon. |
| Stakeholder bị ảnh hưởng | Độc giả Sports Illustrated, đội ngũ nhà báo thật của SI (bị liên đới mất uy tín), ngành báo chí nói chung |
| Số liệu chính | Ít nhất nhiều bài viết bị gỡ sau điều tra; đây là vụ thứ 3 trong năm 2023 cùng dạng (sau CNET đầu năm 2023 và Gannett/Reviewed tháng 10/2023) — cho thấy một mẫu hình lặp lại trong ngành |
| Trích nguồn ngắn | Theo điều tra của Futurism, ảnh đại diện của "tác giả" Drew Ortiz trùng khớp với ảnh đang được rao bán trên một trang web chuyên cung cấp ảnh chân dung do AI tạo. |
| Nguồn 1 | Futurism, "Sports Illustrated Published Articles by Fake, AI-Generated Writers" — 27/11/2023 — https://futurism.com/sports-illustrated-ai-generated-writers |
| Nguồn 2 | CNN Business, "Sports Illustrated deletes articles published under fake author names and AI-generated profile photos" — 27/11/2023 — https://www.cnn.com/2023/11/27/media/sports-illustrated-deletes-articles-fake-author-names-ai-profile-photos/index.html |
| Ghi chú độ tin cậy | High-quality secondary (Futurism là nguồn điều tra gốc, có phỏng vấn nguồn tin nội bộ); CNN/NPR/PBS là nguồn thứ cấp xác nhận lại và bổ sung phát ngôn chính thức từ Arena Group — có một điểm mâu thuẫn nhỏ: Arena Group phủ nhận "AI viết nội dung" trong khi Futurism khẳng định có dấu hiệu nội dung do AI tạo, cần ghi rõ đây là tranh cãi chưa được phân xử dứt khoát. |

## Harm Map Worksheet

| Trường | Nội dung |
|---|---|
| High-risk moment | Độc giả đọc bài đánh giá sản phẩm tin rằng tác giả là nhà báo/chuyên gia thật, dựa vào đó để quyết định mua hàng hoặc tin tưởng thương hiệu SI |
| Stakeholder bị ảnh hưởng | Độc giả bị đánh lừa về nguồn gốc nội dung; nhà báo thật tại SI bị liên đới mất uy tín nghề nghiệp |
| Failure mode | Misuse (sử dụng AI để tạo danh tính giả nhằm tăng độ tin cậy giả tạo cho nội dung thương mại) |
| Layer bắt đầu lỗi | UX (lớp hiển thị/trình bày — không có disclosure rằng tác giả/ảnh là do AI tạo, đánh lừa nhận thức người đọc) |
| Harm xảy ra là gì? | Xói mòn niềm tin công chúng vào báo chí; độc giả ra quyết định mua sắm dựa trên "uy tín" giả của tác giả không có thật |
| Harm lens | Misinformation (về nguồn gốc và độ tin cậy nội dung); Dignity loss (đối với nhà báo thật bị liên đới) |
| Severity | Medium — không gây hại thể chất hay tài chính trực tiếp lớn, nhưng làm tổn hại nghiêm trọng uy tín một thương hiệu báo chí lâu đời và niềm tin vào ngành |
| Scale | Medium — ảnh hưởng độc giả của một ấn phẩm cụ thể (SI) và lan ra dư luận ngành báo chí Mỹ nói chung, không phải toàn cầu/mọi người dùng |
| Probability | High — đây là mô hình kinh doanh có chủ đích (dùng bút danh + ảnh AI) lặp lại nhiều lần với nhiều "tác giả" khác nhau trên cùng một trang, không phải sự cố ngẫu nhiên |
| Frequency | High — đã xảy ra lặp lại ở ít nhất 3 tổ chức báo chí khác nhau trong cùng năm (CNET, Gannett/Reviewed, Sports Illustrated), cho thấy đây là một mẫu hình lan rộng trong ngành chứ không phải case đơn lẻ |
| Vì sao? | Severity ở mức Medium vì hậu quả chủ yếu là tổn hại uy tín/niềm tin (recoverable theo thời gian) chứ không phải tổn hại không thể đảo ngược như case bầu cử hay Grok; Scale Medium vì giới hạn trong phạm vi độc giả một ấn phẩm dù tác động lan ra ngành; Probability và Frequency đều cao vì đây là hành vi có chủ đích, lặp lại có hệ thống ở nhiều tổ chức, khác với lỗi kỹ thuật ngẫu nhiên. |