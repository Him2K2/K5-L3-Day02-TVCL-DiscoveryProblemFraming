# CP4 — Kiểm chứng và tìm hiểu giải pháp có sẵn

Tiếp nối [CP3](cp3-hoi-tu-nhom.md), phần này tập trung vào bài của Trí: **phân loại và chuyển phản ánh cư dân đến đúng bộ phận ngay từ lần đầu**. Trước khi chọn cách giải, cần biết nhân viên thực sự mất thời gian ở đâu và vì sao có ticket bị chuyển sai.

> Trạng thái: đã tổng hợp dữ liệu được mô tả trong bài Trí và đọc tài liệu giải pháp có sẵn. Chưa có cuộc phỏng vấn, survey hoặc thử nghiệm mới. Các bảng kế hoạch không được tính là kết quả kiểm chứng đã hoàn thành.

## 1. Những điều đang biết và còn chưa chắc

| Nội dung trong bài Trí | Có thể sử dụng ở mức nào? | Cần làm rõ |
|---|---|---|
| 120 ticket trong một ca trực 8 giờ | Thông tin quan sát được bài nguồn báo cáo | Một hay nhiều nhân viên? Ca nào, ngày nào, lấy mẫu ra sao? |
| 4.5 phút tiếp nhận một ticket; riêng đọc mô tả/ảnh là 2 phút | Baseline được đề xuất từ quan sát thủ công, chưa đối chiếu phiếu gốc | Bài nhắc 20 ca quan sát: “ca” là ca trực hay trường hợp? Có tính thời gian chờ không? |
| Khoảng 12% ticket chuyển sai bộ phận | Ước tính, chưa coi là tỷ lệ được xác nhận | Mẫu số, định nghĩa chuyển sai và người xác nhận bộ phận đúng |
| Danh mục phòng ban có thể chồng chéo | Giả thuyết nguyên nhân từ phản biện trong bài | Có ticket cụ thể nào mà hai bộ phận cùng có thể phụ trách? |
| Mục tiêu dưới 1.5 phút/ticket và chuyển sai dưới 3% | Mục tiêu đề xuất | Có phù hợp khối lượng công việc và mức sai chấp nhận được không? |

Một điểm cần kiểm tra: 120 × 4.5 = **540 phút thao tác**, trong khi một ca 8 giờ là 480 phút. Điều này chưa chứng minh bài nguồn sai vì có thể nhiều người cùng xử lý hoặc cách tính thời gian khác nhau. Tuy nhiên, phải làm rõ trước khi dùng số liệu để tính mức quá tải hoặc thời gian tiết kiệm.

## 2. Assumption Map

Điểm 1–5 dưới đây là đánh giá sơ bộ để xếp thứ tự kiểm chứng. Ở cột bằng chứng, 1 là rất ít và 5 là đã có bằng chứng rõ. Nhóm cần điều chỉnh sau khi xem dữ liệu gốc.

| # | Giả định | Loại | Quan trọng | Đã có bằng chứng | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| A1 | Việc đọc và xác định đơn vị tiếp nhận thực sự chiếm phần lớn thời gian thao tác | Value | 5 | 2 | Có — xem phiếu quan sát và bấm giờ lại |
| A2 | Có đủ ticket được phép sử dụng, đã ẩn danh và xác nhận được đơn vị xử lý đúng | Feasibility | 5 | 1 | Có — xác nhận quyền dữ liệu và nhãn |
| A3 | Chuyển sai chủ yếu do khó hiểu mô tả, không phải trách nhiệm phòng ban chưa rõ | Value | 5 | 1 | Có — rà các ca chuyển sai/chồng chéo |
| A4 | Danh mục rõ hơn và biểu mẫu/Rule vẫn chưa giải quyết đủ khó khăn | Value | 5 | 1 | Có — thử cách đơn giản trước |
| A5 | Nhân viên kiểm tra và sửa được gợi ý mà không mất thêm nhiều thời gian | Usability | 4 | 1 | Sau A1–A4 — quan sát review mẫu |
| A6 | Đơn vị vận hành có người quản lý danh mục, dữ liệu và chi phí duy trì | Viability | 4 | 1 | Xác nhận với người phụ trách |

Ưu tiên A2 và A3 trước: nếu không lấy được dữ liệu hợp lệ hoặc chưa thống nhất đơn vị phụ trách, thử mô hình phân loại sẽ khó cho kết quả có ý nghĩa.

## 3. Kiểm chứng với người thật

### 3.1. Cách thực hiện đề xuất

Phỏng vấn **2–3 người ngoài nhóm**, có kinh nghiệm thực sự với quy trình này: nhân viên tiếp nhận, điều phối viên và người nhận ticket ở bộ phận kỹ thuật. Có thể hỏi bạn học nhóm khác nếu họ có trải nghiệm phù hợp. Chưa có lịch hoặc người tham gia được xác nhận.

Mỗi buổi dành khoảng 5–7 phút, hỏi về một sự việc đã xảy ra. Chỉ ghi vai trò và mã người tham gia; không đưa tên cư dân, số căn hộ, số điện thoại hoặc ảnh có thông tin riêng tư vào repo.

### 3.2. Câu hỏi phỏng vấn

1. Lần gần nhất anh/chị nhận một phản ánh khó phân loại là khi nào? Có thể kể lại từ lúc nhận đến lúc chuyển bộ phận không?
2. Trong trường hợp đó, bước nào mất nhiều thời gian nhất? Anh/chị xác định thời gian bằng cách nào?
3. Anh/chị đã tra cứu ở đâu để biết đơn vị phụ trách? Có phải hỏi thêm người khác không?
4. Lần gần nhất ticket bị chuyển lại là vì hiểu sai nội dung, thiếu thông tin hay chưa rõ trách nhiệm bộ phận?
5. Với mô tả thiếu vị trí hoặc ảnh, anh/chị đã xử lý ra sao? Thời gian thao tác và thời gian chờ là bao nhiêu?
6. Anh/chị từng thử biểu mẫu, danh mục hoặc quy tắc nào để giảm việc phân loại? Trường hợp nào vẫn không giải quyết được?

Không hỏi “Anh/chị có muốn một công cụ AI không?” hoặc dùng lời khen ý tưởng làm bằng chứng. Cần ghi cả trường hợp nhân viên xử lý nhanh, ít chuyển sai hoặc thấy cách hiện tại đã đủ tốt.

### 3.3. Interview Snapshot — mẫu để ghi sau khi hỏi

Tạo một snapshot cho mỗi người; không điền lời trích dẫn trước khi có câu trả lời thật.

| Trường | Nội dung |
|---|---|
| Mã người tham gia và vai trò | [Cần điền] |
| Ngày, hình thức hỏi và người phỏng vấn | [Cần điền] |
| Lần gần nhất gặp vấn đề: chuyện gì đã xảy ra? | [Ghi sự việc cụ thể] |
| Hiện đang xử lý bằng cách nào? | [Ghi cách làm thực tế] |
| Thời gian, tần suất và nguồn số liệu | [Tách phút thao tác khỏi phút chờ] |
| Câu nói đáng nhớ nhất, nguyên văn | [Chỉ ghi sau phỏng vấn] |
| Tín hiệu xác nhận | [Ghi nếu có] |
| Tín hiệu phản bác | [Ghi nếu có; không tạo cho đủ mục] |
| Điều cần sửa trong cách hiểu vấn đề | [Rút ra từ dữ liệu trên] |

### 3.4. Tổng hợp hiện tại

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác hoặc giới hạn |
|---|---|---|---|
| Bài cá nhân của Trí | Theo bài: quan sát thủ công 20 ca; chưa rõ đơn vị “ca” | Có mô tả quy trình và bước đọc mất thời gian | Chưa có phiếu/log gốc; tỷ lệ chuyển sai là ước tính |
| Phỏng vấn mới | 0 | Chưa có | Chưa hoàn thành kiểm chứng người dùng của CP4 |
| Thử biểu mẫu/Rule trên ticket | 0 | Chưa có | Chưa biết cách đơn giản có đủ hay không |

**Chưa có tín hiệu phản bác từ người được phỏng vấn.** Việc danh mục chồng chéo và sự chưa nhất quán của số liệu là điểm cần kiểm tra từ tài liệu, không thay thế kết quả phỏng vấn.

## 4. Kiểm tra dữ liệu và baseline

Nếu được đơn vị phụ trách cho phép, lấy một mẫu ticket ẩn danh để đối chiếu cách phân loại hiện tại. Chốt số mẫu và cách chọn trước khi thử; không chỉ chọn các ca dễ hoặc ca lỗi.

| Dữ liệu cần ghi | Mục đích |
|---|---|
| Mã ticket ẩn danh, nhóm sự cố, kênh tiếp nhận | Biết phạm vi và cơ cấu mẫu |
| Phút đọc/xem ảnh, tra cứu, gán nhãn và chuyển | Xác định đúng bước nghẽn |
| Thời gian chờ bổ sung, ghi riêng | Tránh lẫn với thời gian nhân viên thao tác |
| Bộ phận chuyển lần đầu và đơn vị đúng được xác nhận | Tính tỷ lệ chuyển sai lần đầu |
| Lý do chuyển lại | Tách lỗi đọc hiểu, thiếu thông tin và chồng chéo trách nhiệm |
| Phiên bản danh mục và người kiểm tra nhãn | Bảo đảm các phương án dùng chung căn cứ |

Tỷ lệ chuyển sai lần đầu = số ticket được xác nhận chuyển sai / số ticket đã xác nhận được đơn vị đúng. Báo riêng ticket chưa xác định được đơn vị; không tự coi chúng là đúng. Việc chuyển hợp lệ qua nhiều cấp theo quy trình không mặc nhiên là lỗi chuyển sai.

So sánh cách hiện tại với danh mục chuẩn hóa/biểu mẫu/Rule trên mẫu tương đương, có tính thời gian kiểm tra và sửa. Nếu cùng người làm lại cùng ticket, cần lưu ý họ đã nhớ nội dung nên có thể nhanh hơn dù phương án mới không tốt hơn.

## 5. Research giải pháp có sẵn

Ba pattern dưới đây cùng lấy từ tài liệu chính thức Zendesk để thấy một quy trình hỗ trợ có thể đi từ biểu mẫu đến Rule và AI. Đây không phải ba sản phẩm độc lập hoặc bằng chứng phải mua Zendesk. Trợ lý đã mở tài liệu ngày 09/11/2026; thành viên cần tự đọc trước khi nộp. Chưa cài đặt hoặc đo hiệu quả công cụ nào trên ticket cư dân.

| Công cụ / case / pattern | Link chính thức | Giải bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho bài Trí |
|---|---|---|---|---|---|
| Trường ticket và biểu mẫu có cấu trúc | [Ticket Fields API](https://developer.zendesk.com/api-reference/ticketing/tickets/ticket_fields/) | Thu thập thông tin ngay lúc tạo phản ánh | Có trường tùy chỉnh và khả năng hiển thị trường cho người gửi | Trường đầy đủ không có nghĩa nội dung đúng; danh mục khó hiểu vẫn khiến cư dân chọn sai | Thử chuẩn hóa nhóm sự cố và thông tin cần có trước |
| Trigger theo điều kiện và hành động | [Ticket triggers](https://support.zendesk.com/hc/en-us/articles/4408886797466-Creating-ticket-triggers-for-automatic-ticket-updates-and-notifications) | Gán và chuyển ticket dựa trên tiêu chí có sẵn | Logic rõ, dễ đối chiếu với danh mục | Rule có thể xung đột; thứ tự thực thi ảnh hưởng kết quả | Lập bảng ánh xạ nhóm sự cố–đơn vị và kiểm tra các trường hợp chồng chéo |
| Intelligent triage | [Tài liệu intelligent triage](https://support.zendesk.com/hc/en-us/articles/4964463770650-About-intelligent-triage) | Phân loại nội dung ticket, dùng nhãn trong quy trình định tuyến | Tham khảo cách tách bước phân loại khỏi bước chuyển bộ phận | Chưa chứng minh hiệu quả trên tiếng Việt, ảnh và danh mục cư dân của bài này; cần kiểm tra điều kiện sử dụng | Chỉ cân nhắc hỗ trợ phân loại khi biểu mẫu/Rule chưa đủ; nhân viên kiểm tra trong thử nghiệm |

Theo tài liệu, intelligent triage phân tích nội dung bình luận công khai để tạo phân loại; không lấy đó làm bằng chứng tính năng này tự xử lý ảnh/OCR đúng như đề xuất trong bài Trí. Năng lực ảnh cần được khảo sát riêng nếu thật sự cần.

**Điều research gợi ra:** tách ba việc — thu thập đủ dữ liệu, xác định nhóm sự cố và chuyển theo danh mục. Hai việc đầu vào có cấu trúc và ánh xạ bộ phận có thể thử bằng biểu mẫu/Rule. AI là một phương án cần so sánh cho phần mô tả khó, chưa phải kết luận bắt buộc.

## 6. Điều chỉnh cách hiểu vấn đề

Đây là điều chỉnh đề xuất sau khi rà tài liệu và research, **chưa phải thay đổi sau phỏng vấn**.

| Trước khi rà soát | Cách hiểu nên dùng tiếp | Vì sao |
|---|---|---|
| Đọc mô tả lâu nên cần phân loại tự động | Chưa biết thời gian mất ở đọc hiểu hay tra trách nhiệm; cần tách và đo | Cách giải phụ thuộc nguyên nhân |
| 12% là baseline chuyển sai | Giữ 12% là ước tính, chờ mẫu có nhãn xác nhận | Chưa rõ nguồn và mẫu số |
| 120 ticket/ca chứng minh một người bị quá tải | Làm rõ số người, thời gian và cách đếm trước | 120 × 4.5 phút vượt thời lượng một ca 8 giờ nếu chỉ một người |
| Cần một hệ thống AI nhận phản ánh | Trước hết kiểm tra danh mục và Rule; chỉ khảo sát hỗ trợ đọc mô tả nếu còn khoảng trống | Research cho thấy có sẵn các pattern đơn giản hơn |

**Câu mô tả vấn đề tạm dùng để kiểm chứng:** Khi tiếp nhận phản ánh cư dân, nhân viên cần hiểu loại sự cố và xác định đúng đơn vị phụ trách. Hiện bài Trí ghi nhận việc đọc, tra cứu và gán đơn vị tốn thời gian; mức độ chậm, tỷ lệ chuyển sai và nguyên nhân cần được xác nhận bằng quan sát và ticket thực tế.

## 7. Kết luận CP4 và việc tiếp theo

Hiện đã có danh sách giả định, kế hoạch hỏi, mẫu snapshot và research. **CP4 chưa hoàn tất** vì chưa có phỏng vấn/survey mới, dữ liệu gốc để xác nhận baseline hoặc tín hiệu phản bác từ người dùng.

- [ ] Xác nhận quyền dùng dữ liệu và người phụ trách danh mục.
- [ ] Hoàn thành 2–3 phỏng vấn ngoài nhóm hoặc survey 5–10 người phù hợp.
- [ ] Ghi snapshot có vai trò, ngày, cách hỏi và hành vi thật; giữ cả bằng chứng không ủng hộ hướng ban đầu.
- [ ] Làm rõ 120 ticket/ca, 20 ca quan sát, 4.5 phút/ticket và tỷ lệ chuyển sai.
- [ ] Tự mở nguồn research và kiểm tra biểu mẫu/Rule có thể giải phần nào.
- [ ] Ghi nhóm đã sửa problem, metric hoặc phạm vi thế nào từ kết quả thực tế.

Sau đó chuyển sang CP5 để vẽ quy trình trước/sau và viết Problem Statement v0. Nếu bằng chứng cho thấy cách hiện tại đã đủ tốt hoặc chuẩn hóa danh mục giải quyết được vấn đề, cần điều chỉnh hướng thay vì cố giữ phương án AI.

## 8. Nguồn

- Bài `2A202603379_HoangNgocMinhTri.md` do học viên cung cấp, mục CP1–CP2; chưa sao chép file gốc từ Downloads vào repo.
- [CP3 — Xử lý phản ánh cư dân](cp3-hoi-tu-nhom.md).
- [Worksheet](../../docs/01-worksheet.md), [bài mẫu](../../docs/02-deliverable-example.md).
- Ba tài liệu chính thức được dẫn trực tiếp trong bảng research.
