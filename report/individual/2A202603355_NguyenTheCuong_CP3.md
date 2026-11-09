# CP3 — Hội tụ nhóm: Xử lý phản ánh cư dân

Bài của Trí đưa ra ba vấn đề trong quá trình xử lý phản ánh: chuyển ticket đúng bộ phận, phát hiện thông tin còn thiếu và bàn giao cho ca sau. Phần này đặt ba vấn đề cạnh nhau để xem nên tập trung vào đâu trước.

> Đây là bản phân tích dựa trên bài cá nhân của Hoàng Ngọc Minh Trí, chưa phải kết quả họp nhóm. Điểm số và hướng lựa chọn là đề xuất để nhóm thảo luận. Các số liệu được trích từ bài Trí, chưa đối chiếu với log hoặc phiếu quan sát gốc.

## 1. Ba vấn đề được đưa ra

| Mã | Candidate | Ai gặp vấn đề? | Bước đang vướng |
|---|---|---|---|
| T1 | Phân loại và chuyển phản ánh đúng bộ phận | Nhân viên tiếp nhận, điều phối viên CSKH | Đọc mô tả và xem ảnh mất khoảng 2 phút trong tổng 4.5 phút tiếp nhận một ticket, theo bài Trí |
| T2 | Xác định thông tin còn thiếu trong ticket | Nhân viên CSKH, kỹ thuật viên tiếp nhận | Phải kiểm tra, hỏi bổ sung rồi chờ cư dân trả lời; thời gian chờ được báo cáo là 30–180 phút |
| T3 | Bàn giao đủ bối cảnh xử lý cho ca sau | Điều phối viên ca trước, kỹ thuật viên ca sau | Phải đọc lại lịch sử trao đổi; Card 3 ghi 4 phút đọc trong tổng 11 phút bàn giao một ticket |

Ba vấn đề nằm ở các thời điểm khác nhau: khi tiếp nhận, khi làm rõ thông tin và khi chuyển người xử lý. Vì vậy, cần chọn một điểm để làm sâu trước, thay vì ôm toàn bộ quy trình trong một buổi lab.

```text
Pitch top 3 → Gom cluster → Cây OST → Chấm điểm và thống nhất chọn 1
   12 phút      5 phút        5 phút                   8 phút
```

Hiện mới có ba card từ bài Trí, chưa đủ 9–12 candidate của một nhóm 3–4 người. Phần pitch và phản biện sẽ do các thành viên tự thực hiện, sau đó bổ sung kết quả vào mục 6.

## 2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Hiểu phản ánh và chuyển đúng nơi | T1 — Phân loại và định tuyến phản ánh | Nhân viên phải hiểu nội dung cư dân gửi rồi tra xem bộ phận nào phụ trách |
| B — Làm rõ thông tin ban đầu | T2 — Xác định thông tin còn thiếu | Thiếu vị trí, mô tả hoặc ảnh khiến nhân viên phải hỏi lại và chờ bổ sung |
| C — Giữ đủ thông tin khi bàn giao | T3 — Bàn giao bối cảnh xử lý | Lịch sử trao đổi dài, thông tin rải rác khiến ca sau mất công đọc lại hoặc hỏi lại cư dân |

Điểm chung là người tiếp nhận cần đủ thông tin để xử lý đúng. Tuy nhiên, nguyên nhân và cách đo của từng vấn đề khác nhau; chưa nên gộp chúng thành một bài toán lớn.

## 3. Opportunity Solution Tree rút gọn

T1 là card Trí muốn trình bày nhất trong bài cá nhân. Cây dưới đây làm rõ các khó khăn cần kiểm tra nếu tiếp tục theo hướng này.

```text
OUTCOME: Giảm thời gian tiếp nhận và chuyển phản ánh đúng bộ phận
         từ 4.5 phút xuống dưới 1.5 phút/ticket,
         đồng thời đưa tỷ lệ chuyển sai xuống dưới 3%
├── Opportunity: Mất thời gian đọc mô tả và xem ảnh để hiểu sự cố
├── Opportunity: Chưa rõ bộ phận phụ trách khi danh mục sự cố chồng chéo
└── Opportunity: Phải tra cứu đơn vị xử lý và gán lại thông tin cho từng ticket
     ✗ "Chatbot tiếp nhận cư dân"   ← giải pháp, chưa đưa vào tầng nhu cầu
     ✗ "Mô hình phân loại tự động"  ← giải pháp, chưa đưa vào tầng nhu cầu
     ✗ "Form chọn nhóm sự cố"       ← giải pháp, chưa đưa vào tầng nhu cầu
```

Mốc 4.5 phút được lấy từ bài Trí và cần kiểm tra lại cách đo. Tỷ lệ chuyển sai khoảng 12% trong bài nguồn vẫn là ước tính. Hai mục tiêu dưới 1.5 phút và dưới 3% là mức đề xuất, chưa phải kết quả đã đạt. Việc danh mục phòng ban chồng chéo cũng cần kiểm chứng trước khi coi là nguyên nhân chính.

## 4. Chấm điểm shortlist

Bảng dưới dùng thang 1–5 để so sánh ba hướng. Đây là điểm tham khảo do AI hỗ trợ từ bài viết; nhóm cần tự chấm lại dựa trên dữ liệu và khả năng thực hiện của mình.

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được 4 mức | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| T1 — Phân loại và định tuyến phản ánh | 5 | 5 | 3 | 5 | 4 | 5 | 3 | **30** |
| T2 — Xác định thông tin còn thiếu | 5 | 5 | 3 | 4 | 5 | 4 | 3 | **29** |
| T3 — Bàn giao bối cảnh xử lý | 5 | 4 | 3 | 4 | 4 | 5 | 3 | **28** |

T1 có người thực hiện và các bước khá rõ, có thể đo thời gian tiếp nhận và tỷ lệ chuyển đúng bộ phận. Bài này cũng cho phép thử nhiều cách đơn giản trước: sửa danh mục, làm biểu mẫu hoặc dùng Rule. Nếu vẫn còn khó ở bước đọc hiểu mô tả thì mới xem xét hỗ trợ phân loại.

T2 dễ thử trên một mẫu nhỏ bằng checklist hoặc trường bắt buộc. Điểm cần lưu ý là thời gian chờ phụ thuộc vào lúc cư dân trả lời; giảm thời gian nhân viên thao tác chưa chắc làm toàn bộ ticket nhanh hơn tương ứng.

T3 có ý nghĩa với việc giao ca, nhưng số đo cần làm rõ hơn. CP1 trong bài Trí ghi 8–12 phút đọc lịch sử, còn CP2 ghi 4 phút đọc và 11 phút cho cả lượt bàn giao. Có thể đây là hai nhóm mẫu hoặc hai phạm vi đo khác nhau, cần kiểm tra trước khi chọn baseline.

Cả ba được chấm 3 ở phần bằng chứng vì chưa có dữ liệu gốc để đối chiếu. Điểm hiểu domain cũng tạm để 3 do chưa có thông tin của toàn nhóm. Chênh lệch một hoặc hai điểm chỉ giúp mở cuộc thảo luận, chưa đủ để chốt lựa chọn.

## 5. Hướng đề xuất chọn

**Chọn đề xuất: T1 — Phân loại và định tuyến phản ánh cư dân.**

T1 đáng làm trước vì đây là bước đầu tiên khi nhận một phản ánh. Nếu chuyển sai ngay từ đầu, ticket phải đi qua thêm người và cư dân phải chờ lâu hơn. Phạm vi cũng có thể thu hẹp: chọn một nhóm sự cố, xác định rõ các đơn vị phụ trách rồi đo thời gian và độ chính xác khi phân loại. Trong bài cá nhân, Trí cũng ưu tiên Card 1 vì lý do này.

**Vì sao tạm chưa chọn hai hướng còn lại:**

- **T2 — Thông tin còn thiếu:** vẫn đáng giải quyết, nhưng cần tách phần nhân viên xử lý và phần chờ cư dân. Có thể giữ làm bước tiếp theo; nếu biểu mẫu và checklist đã đủ thì không cần thêm AI.
- **T3 — Bàn giao bối cảnh:** cần có lịch sử ticket được phép sử dụng và cách kiểm tra bản bàn giao có bỏ sót thông tin hay không. Trước mắt nên làm rõ số đo và phạm vi bàn giao rồi mới cân nhắc thử nghiệm.

Lựa chọn T1 hiện là đề xuất từ tài liệu. Nhóm cần kiểm tra khả năng lấy mẫu ticket và thống nhất lại sau khi trao đổi, thay vì chọn chỉ vì T1 cao điểm nhất.

## 6. Bất đồng và nội dung cần nhóm xác nhận

**Bất đồng:** chưa có ghi nhận từ buổi họp, nên phần này để nhóm bổ sung theo diễn biến thật.

Một câu hỏi cần bàn kỹ là: nếu chuẩn hóa lại danh mục phòng ban và biểu mẫu tiếp nhận, nhân viên còn gặp khó khi phân loại không? Nếu vướng mắc nằm ở trách nhiệm chồng chéo giữa các bộ phận thì chỉ làm cho bước đọc nhanh hơn sẽ chưa giải quyết được vấn đề.

| Nội dung | Ghi nhận sau buổi thảo luận |
|---|---|
| Ngày họp, người trình bày và thành viên tham dự | [Cần điền] |
| Câu hỏi phản biện và người đặt câu hỏi | [Ghi câu hỏi thực tế] |
| Điểm nhóm chấm lại và lý do thay đổi | [Cần xác nhận] |
| Candidate cuối cùng và lý do chọn | [Cần xác nhận] |
| Ý kiến khác và cách nhóm xử lý | [Bổ sung nếu có] |

## 7. Việc cần kiểm tra ở CP4

Nếu nhóm chọn T1, bước tiếp theo là kiểm tra những điểm còn chưa chắc:

1. Xem lại phiếu quan sát để hiểu mốc 4.5 phút/ticket và 2 phút đọc nội dung được đo thế nào. Bài Trí có nhắc 20 ca quan sát; cần làm rõ “ca” là ca trực hay trường hợp xử lý.
2. Đếm lại số ticket chuyển sai trên một mẫu có đơn vị phụ trách được xác nhận, thay cho tỷ lệ 12% ước tính.
3. Tìm các trường hợp danh mục chồng chéo để xem nhân viên mất thời gian vì đọc mô tả hay vì không rõ trách nhiệm phòng ban.
4. Phỏng vấn người tiếp nhận ngoài nhóm về một ticket khó gần đây: họ đã làm gì, tra cứu ở đâu và mất bao lâu.
5. Thử danh mục rõ hơn, biểu mẫu hoặc checklist trước khi quyết định có cần AI hỗ trợ hay không.

Ở CP3, đầu ra cần chốt là một vấn đề để kiểm chứng. Problem Statement sẽ được viết sau khi có thêm bằng chứng và phân tích quy trình ở CP4–CP5.

## 8. Tài liệu sử dụng

- Bài cá nhân `2A202603379_HoangNgocMinhTri.md` do học viên cung cấp, mục CP1–CP2; file gốc hiện chưa được sao chép vào repo.
- [Worksheet — hướng dẫn CP3](../../docs/01-worksheet.md).
- [Bài làm mẫu](../../docs/02-deliverable-example.md).