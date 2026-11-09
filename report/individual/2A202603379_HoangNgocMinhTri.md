# Báo cáo cá nhân — 2A202603379_HoangNgocMinhTri

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Hoang Ngoc Minh Tri
- MSSV: 2A202603379
- Email trường (không bắt buộc, repo có thể để public): 26ai.trihnm@vinuni.edu.vn
- Tên nhóm: TVCL 
- Link repo nhóm: https://github.com/Him2K2/K5-L3-Day02-TVCL-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi tiếp nhận một phản ánh mới từ cư dân/khách hàng, tôi muốn nắm rõ ngay loại sự cố và khu vực phát sinh, để chuyển chính xác đến bộ phận xử lý chuyên trách mà không cần đọc đi đọc lại nhiều lần. | Nhân viên tiếp nhận / Điều phối viên |Qua quan sát thực tế trong 1 ca trực 8h, tiếp nhận trung bình 120 ticket; nhân viên phải thực hiện thao tác đọc và xác định bộ phận thủ công trùng lặp 100% số ticket. |
| 2 | Tốn thời gian |Khi thông tin sự cố do cư dân cung cấp bị thiếu sót (như thiếu số căn hộ, thiếu hình ảnh hiện trạng), tôi muốn biết chính xác thông tin nào còn thiếu, để phản hồi yêu cầu bổ sung ngay mà không làm gián đoạn hay kéo dài thời gian xử lý. | Nhân viên CSKH / Cư dân Vinhomes | Đo đạc trên 30 ticket bị trả lại: thời gian xử lý kéo dài trung bình từ 15 phút lên 180 phút do mất 3-4 lượt nhắn tin/gọi điện hỏi lại thông tin ban đầu.|
| 3 | Cần đọc/tổng hợp nhiều thông tin |Khi xử lý một ticket kéo dài qua nhiều ca trực hoặc trao đổi nhiều lượt, tôi muốn nắm bắt ngay các dữ kiện quan trọng chính, để đưa ra phương án giải quyết mà không bỏ sót bối cảnh lịch sử. | Trưởng nhóm vận hành / Kỹ thuật viên| Theo dõi 15 ticket phức tạp: mỗi nhân viên tiếp quản mất trung bình 8–12 phút chỉ để đọc lại toàn bộ lịch sử trò chuyện và ghi chú cũ trước khi xử lý.|
| 4 | Pain từ người khác | Khi sự cố được chuyển giao sang đội kỹ thuật hoặc bên thứ ba, tôi muốn người tiếp nhận sau hiểu rõ toàn bộ diễn biến đã xảy ra, để cư dân không phải giải thích lại từ đầu. | Đội kỹ thuật hiện trường / Cư dân| Ghi nhận 12 trường hợp phản ánh cư dân bức xúc: có 8/12 trường hợp cư dân phàn nàn vì phải nhắc lại cùng một nội dung sự cố cho 2-3 người khác nhau.|
| 5 | Lặp lại / Pain từ người khác | Khi có nhiều cư dân cùng phản ánh về một sự cố chung (như mất nước cục bộ, hỏng thang máy), tôi muốn nhận biết các phản ánh này có cùng nguyên nhân, để xử lý đồng bộ và thông báo nhất quán cho toàn bộ cư dân liên quan. | Điều phối viên / Cư dân phân khu | Ghi nhận tại ca trực khi xảy ra sự cố kỹ thuật chung: có 45 ticket gửi về riêng lẻ cho cùng 1 vấn đề, dẫn đến 5 kỹ thuật viên bị phân công trùng lặp vào cùng 1 địa điểm.|
| 6 | Thiếu hụt dữ liệu hiện trường | Khi đi kiểm tra các hạng mục bảo trì tại các tầng hầm tòa nhà, tôi muốn cập nhật trực tiếp tình trạng hỏng hóc kèm hình ảnh thực tế ngay trên thiết bị di động, để ban quản lý nắm bắt tiến độ chính xác mà không phải chờ ghi chép giấy tờ cuối ngày. | Kỹ thuật viên bảo trì / Giám sát tòa nhà | Quan sát thực tế: Kỹ thuật viên mất trung bình 45 phút cuối ca chỉ để lập biên bản giấy và nhập lại vào máy tính, gây chậm trễ 100% các báo cáo nhanh cho cấp trên. |
| 7 | Chênh lệch thời gian phản hồi | Khi nhận được phản ánh về việc thẻ cư dân hoặc thẻ xe không nhận diện được tại cổng ra vào vào giờ cao điểm sáng, tôi muốn nhanh chóng xác minh trạng thái kích hoạt của thẻ, để giải tỏa dòng xe đang ùn tắc trước sảnh mà không gây bức xúc. | Nhân viên an ninh cổng / Cư dân | Ghi nhận thực tế tại sảnh tòa nhà vào khung giờ 7:30 - 8:30 sáng: xảy ra 6-8 trường hợp ùn tắc cục bộ kéo dài từ 3-5 phút mỗi lượt do phải kiểm tra thủ công danh sách thẻ lỗi.|
| 8 | Nút thắt phân bổ tài nguyên | Khi có lịch đăng ký sử dụng phòng sinh hoạt cộng đồng hoặc khu vực BBQ trùng nhau từ nhiều hộ dân, tôi muốn dễ dàng đối chiếu lịch trống và quy chế ưu tiên, để sắp xếp lịch cho thuê công bằng và tránh tranh chấp. |Nhân viên dịch vụ tiện ích / Ban quản lý | Thống kê trong tháng: Ghi nhận 14 khiếu nại liên quan đến việc trùng lịch đặt tiện ích do sổ tay ghi nhận thủ công không cập nhật kịp thời giữa các ca trực.|
| 9 | Phân mảnh kênh thông tin| Khi ban quản lý cần thông báo khẩn về việc cắt nước bảo trì đến toàn bộ cư dân một tòa nhà, tôi muốn kiểm soát tỷ lệ cư dân đã đọc và xác nhận thông tin, để chủ động hỗ trợ những hộ chưa nắm bắt kịp thời. | Ban quản lý / Truyền thông tòa nhà | Khảo sát từ đợt thông báo sửa chữa tháng trước: Chỉ có khoảng 60% cư dân phản hồi qua nhóm chat Zalo/thông báo giấy, khiến đội ngũ vận hành phải gọi điện thoại trực tiếp cho hơn 40 hộ còn lại (tốn ~3 giờ gọi).|
| 10 | Gánh nặng kiểm toán / Báo cáo định kỳ | Khi phải tổng hợp các số liệu phản ánh và kết quả xử lý sự cố để báo cáo với chủ đầu tư hàng tháng, tôi muốn trích xuất toàn bộ dữ liệu phân loại theo nhóm sự cố và thời gian xử lý, để hoàn thành báo cáo đúng hạn mà không phải rà soát hàng trăm dòng dữ liệu thủ công. | Trưởng bộ phận vận hành / Quản lý tòa nhà | Quan sát thực tế: Mỗi cuối tháng, quản lý phải mất trọn 2 ngày làm việc (khoảng 14-16 tiếng) chỉ để lọc, đếm và vẽ biểu đồ thủ công từ các file ghi chú rời rạc.|

**Nếu có dùng AI để gợi ý thêm:**
- sau khi scan thì giữ lại các ý như là: góc nhìn sáng tạo hướng vào thực trạng vận hành thực tế như: sự thiếu hụt dữ liệu hiện trường, độ trễ thời gian xử lý sự cố ngoài cổng. Bỏ các ý như: câu mang tính định hướng giải pháp kỹ thuật (như "tôi muốn hệ thống tự động gửi thông báo qua SMS" hay "tôi muốn dùng AI phân tích dữ liệu"), vì các dấu hiệu đã được dựa trên bối cảnh thực tế kèm dữ liệu thật

-

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Phân loại & Định tuyến ticket (Lăng kính: Lặp lại) |  Tần suất xuất hiện 100% trên mọi ticket; ảnh hưởng trực tiếp đến thời gian chờ ban đầu của cư dân; quy trình hiện tại có các bước phân loại thủ công rõ ràng.| Chưa đo đạc chính xác tỷ lệ phân loại sai giữa các phòng ban chuyên trách vào các ngày nghỉ/lễ. |
| 2 |Xác định thông tin thiếu sót | Gây ra độ trễ lớn nhất trong quy trình xử lý (từ vài phút kéo dài thành nhiều giờ); tiêu tốn nhiều lượt tương tác phản hồi qua lại. | Chưa rõ tỷ lệ cư dân chủ động cung cấp lại thông tin ngay sau tin nhắn nhắc nhở là bao nhiêu %.|
| 3 | Bàn giao bối cảnh xử lý | Ảnh hưởng trực tiếp tới trải nghiệm cư dân (phải giải thích lại nhiều lần); dễ gây hiểu nhầm hoặc bỏ sót chi tiết kỹ thuật giữa các ca trực. |Mức độ đầy đủ của nhật ký ghi chú hiện tại giữa các ca trực chưa được chuẩn hóa theo mẫu cố định. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story |Khi có phản ánh mới từ cư dân gửi đến hệ thống, tôi muốn biết chính xác nhóm sự cố và đơn vị xử lý chuyên trách, để ticket được chuyển đúng nơi ngay trong lần đầu tiên mà không cần đọc thủ công trùng lặp. |
| Actor | Nhân viên tiếp nhận / Điều phối viên tổng đài CSKH |
| Thời điểm / bối cảnh | Giờ cao điểm ca sáng (7:30 - 9:00) và ca tối (18:30 - 20:00), trung bình 120 ticket/ca trực. |
| Quy trình hiện tại (3–7 bước) | 
1. Tiếp nhận notification ticket mới trên phần mềm (0.5 phút)

2. Mở chi tiết, đọc nội dung mô tả và xem hình ảnh cư dân gửi (2.0 phút)

3. Xác định loại sự cố và tra cứu đơn vị phụ trách (Kỹ thuật/Dịch vụ/An ninh) (1.0 phút)

4. Chọn thuộc tính ưu tiên và gán tag/đơn vị xử lý (0.5 phút)

5. Lưu và chuyển giao ticket (0.5 phút)|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2  - Tốn 2.0 phút/ticket do mô tả cư dân dài dòng hoặc không rõ ràng, chiếm >44% tổng thời gian xử lý ban đầu.|
| Impact (nếu không giải thì sao) | Tồn đọng ticket giờ cao điểm, nhân viên bị quá tải thao tác lặp đi lặp lại. |
| Success metric (baseline → target) | 
1. Baseline (Hiện tại): 4.5 phút/ticket tiếp nhận; Tỷ lệ chuyển sai bộ phận ~12% (ước tính).

2. Target (Mục tiêu): < 1.5 phút/ticket tiếp nhận; Tỷ lệ chuyển sai bộ phận < 3%.|
| Phương án không dùng AI |Xây dựng biểu mẫu đăng ký dạng Dropdown/Form bắt buộc cư dân chọn sẵn Phân loại + Khu vực trước khi ấn gửi. (Đánh giá: Khả thi một phần, nhưng cư dân có thể chọn sai nhóm do không nắm rõ chuyên môn). |
| Giả thuyết về AI (nếu có) | Phân tích cú pháp text + OCR hình ảnh để gợi ý sẵn nhãn sự cố và phòng ban đề xuất cho nhân viên duyệt 1-click.|
| Cảm nhận nhanh | Workflow / Human-in-the-loop |

Quy trình nháp hiện tại:

```
CURRENT — 4.5 phút / ticket
[1. Tiếp nhận ticket: 0.5 min]
  ↓
[2. Đọc nội dung & xem ảnh đính kèm: 2.0 min] ← BOTTLENECK
  ↓
[3. Xác định loại sự cố & tra đơn vị phụ trách: 1.0 min]
  ↓
[4. Gán nhãn ưu tiên & chọn phòng ban: 0.5 min]
  ↓
[5. Chuyển giao ticket: 0.5 min]

```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi tiếp nhận ticket sự cố thiếu thông tin chi tiết (như không có vị trí chính xác, thiếu hình ảnh hiện trạng), tôi muốn xác định ngay các trường dữ liệu còn thiếu, để gửi yêu cầu bổ sung cho cư dân chính xác ngay từ đầu. |
| Actor | Nhân viên CSKH / Kỹ thuật viên tiếp nhận. |
| Thời điểm / bối cảnh |Đơn phản ánh sự cố điện/nước/kỹ thuật phát sinh trong căn hộ hoặc khu vực công cộng. |
| Quy trình hiện tại (3–7 bước) | 
1. Tiếp nhận ticket đã qua phân loại (0.5 phút)

2. Kiểm tra độ đầy đủ của dữ liệu (Vị trí, mô tả, ảnh hiện trạng, SĐT liên hệ) (1.5 phút)

3. Soạn tin nhắn/gọi điện yêu cầu cư dân bổ sung thông tin (2.0 phút)

4. Tạm dừng ticket, chờ phản hồi từ cư dân (Thời gian chờ: 30 - 180 phút)

5. Đọc thông tin bổ sung và cập nhật lại vào ticket (1.0 phút)|
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 & 3 - Kiểm tra thủ công và phản hồi qua lại tốn 3.5 phút xử lý + thời gian chết kéo dài từ 30-180 phút chờ cư dân trả lời.|
| Impact (nếu không giải thì sao) |Kéo dài SLA giải quyết sự cố, cư dân cảm thấy phiền phức khi bị hỏi lại nhiều lần. |
| Success metric (baseline → target) | 
1. Baseline (Hiện tại): 25% số ticket bị trễ do thiếu thông tin ban đầu; thời gian làm rõ trung bình 120 phút.

2. Target (Mục tiêu): Giảm số ticket cần hỏi lại xuống < 8%; thời gian làm rõ bổ sung xuống < 15 phút.|
| Phương án không dùng AI |Thêm các trường dữ liệu bắt buộc trên App cư dân khi tạo ticket theo từng loại dịch vụ. (Đánh giá: Rất hiệu quả, có thể giải quyết 70% vấn đề mà chưa cần tới AI). |
| Giả thuyết về AI (nếu có) | AI tự động phát hiện mô tả quá ngắn hoặc ảnh mờ ngay lúc cư dân bấm "Gửi" trên ứng dụng và đưa ra gợi ý nhắc nhở tức thì. |
| Cảm nhận nhanh | Rule-based / Non-AI |

Quy trình nháp hiện tại:

```
CURRENT — 5.0 phút xử lý (+30 đến 180 phút chờ cư dân)
[1. Tiếp nhận ticket phân loại: 0.5 min]
  ↓
[2. Kiểm tra độ đầy đủ của thông tin: 1.5 min] ← BOTTLENECK
  ↓
[3. Soạn phản hồi yêu cầu bổ sung: 2.0 min]
  ↓
[4. Tạm dừng ticket - Chờ cư dân phản hồi: 30-180 min]
  ↓
[5. Cập nhật thông tin mới & mở lại ticket: 1.0 min]
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuyển giao sự cố chưa giải quyết xong sang ca trực mới hoặc đội kỹ thuật chuyên sâu, tôi muốn tóm tắt đầy đủ lịch sử đã kiểm tra và các bước đã xử lý, để người tiếp nhận sau hiểu ngay bối cảnh mà không cần hỏi lại cư dân. |
| Actor | Điều phối viên ca trước & Kỹ thuật viên hiện trường ca sau. |
| Thời điểm / bối cảnh | Thời điểm giao ca (14:00 và 22:00) hoặc khi chuyển ticket từ CSKH sang Đội Kỹ thuật chuyên trách. |
| Quy trình hiện tại (3–7 bước) |
1. Rà soát các ticket chưa hoàn thành (Pending/In-Progress) cuối ca (2.0 phút)

2. Đọc lại toàn bộ lịch sử trao đổi, ghi chú nội bộ và nhật ký xử lý (4.0 phút)

3. Tóm tắt nội dung và ghi chú bàn giao (Handover note) (3.0 phút)

4. Nhân viên ca mới đọc nhận bàn giao và xác nhận (2.0 phút) |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2  - Mất 4.0 phút/ticket để tổng hợp dữ liệu từ nhiều tin nhắn trao đổi rải rác giữa cư dân và ca trước.|
| Impact (nếu không giải thì sao) | Trôi thông tin, ca sau xử lý sai lệch so với cam kết của ca trước, cư dân bị gọi hỏi lại thông tin cũ gây bức xúc.|
| Success metric (baseline → target) | 
1. Baseline (Hiện tại): Mất 11 phút cho 1 lượt bàn giao ticket phức tạp; 15% cư dân phản ánh bị hỏi trùng thông tin.

2. Target (Mục tiêu): Giảm thời gian tổng hợp bàn giao xuống < 3 phút; giảm phản ánh bị hỏi trùng xuống < 2%.|
| Phương án không dùng AI | Quy định mẫu biên bản bàn giao cố định gồm 3 mục: Hiện trạng - Việc đã làm - Việc cần làm tiếp. (Đánh giá: Tốt nhưng vẫn tốn công gõ thủ công).|
| Giả thuyết về AI (nếu có) | Trích xuất tự động chuỗi hội thoại thành 3 dòng tóm tắt bối cảnh gắn trực tiếp vào Ticket.|
| Cảm nhận nhanh | Workflow / Agent |

Quy trình nháp hiện tại:

```
CURRENT — 11.0 phút / ticket bàn giao
[1. Rà soát ticket chưa xong: 2.0 min]
  ↓
[2. Đọc lại toàn bộ lịch sử & log trao đổi: 4.0 min] ← BOTTLENECK
  ↓
[3. Soạn nội dung bàn giao ca: 3.0 min]
  ↓
[4. Nhân viên ca mới tiếp nhận & đọc lại: 2.0 min]
```

### Card muốn pitch nhất

- Card số: Problem Card 1: Phân loại và Định tuyến phản ánh
- Vì sao: 
1. Đây là "điểm đầu vào" của toàn bộ hệ thống vận hành. Giải quyết tốt bài toán này sẽ tạo tác động dây chuyền tích cực cho các bước sau.

2. Có tần suất xảy ra cao nhất và chỉ số đo lường (SLA/Thời gian) rất rõ ràng.
- Câu hỏi muốn nhóm phản biện: Nếu chúng ta thay đổi giao diện App cư dân để họ tự chọn nhóm sự cố qua dạng cây thư mục chính xác hơn, liệu giải pháp Quy trình/Rule này có đủ đáp ứng mà KHÔNG CẦN xây dựng mô hình AI phân loại hay không? Điểm gãy của giải pháp Non-AI ở đây là gì?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Ở Problem Card 1, chỉ số Baseline 'Tỷ lệ chuyển sai bộ phận 12%' và 'Thời gian đọc ảnh/mô tả 2 phút' đang mang tính ước lượng cá nhân, chưa có công cụ ghi log tự động để chứng minh. Ngoài ra, việc đổ lỗi cho việc đọc mô tả lâu là do cư dân viết dài có thể không đúng; nguyên nhân gốc rễ (Root cause) có thể do danh mục phân loại phòng ban của Vinhomes quá chồng chéo (ví dụ: Sự cố điều hòa vừa thuộc Kỹ thuật điện lạnh, vừa thuộc Bảo trì tòa nhà), khiến nhân viên phân vân chứ không phải do tốc độ đọc. | Đồng ý hoàn toàn với phản biện của AI về nguyên nhân chồng chéo danh mục và việc thiếu số liệu log hệ thống chính thức. | 
1. Hiệu chỉnh thông số: Ghi rõ các số liệu thời gian (như 4.5 phút, 2.0 phút) là số liệu đo đạc mẫu qua 20 ca quan sát thủ công, chưa phải dữ liệu log từ server hệ thống.

2. Bổ sung giải pháp Non-AI: Chuẩn hóa lại danh mục cây phân loại sự cố của ban quản lý trước khi tính đến việc dùng AI phân loại.|

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card |Pitch Problem Card #1 về Phân loại & Định tuyến ticket phản ánh cư dân Vinhomes tại điểm đầu vào. |Nhóm đồng ý đưa bài toán này thành 1 trong 3 candidate chính nhờ tần suất xuất hiện 100% và chỉ số đo lường rõ ràng.|
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: Câu hỏi tôi đã đặt: "Nếu chuẩn hóa quy trình bằng cách bắt buộc cư dân chọn form mẫu sẵn trên App, liệu giải pháp Non-AI có thể giải quyết triệt để mà không cần AI không?" | Giúp nhóm không bị sa đà vào giải pháp AI ngay từ đầu, buộc nhóm phải cân nhắc kỹ phương án Rule-based và cây danh mục.|
| Nhận phản biện | Câu hỏi tôi nhận được: Câu hỏi tôi nhận được: "Lỡ nguyên nhân nghẽn không phải do đọc lâu mà do cây phân loại phòng ban bị chồng chéo làm nhân viên bối rối thì sao?"| Tôi đã sửa gì: Tôi đã sửa gì: Bổ sung nguyên nhân rủi ro cấu trúc danh mục vào báo cáo và đề xuất chuẩn hóa lại cây danh mục song song với bài toán AI.|
| Gom cluster / cây OST | Tham gia thảo luận nhóm để nhóm các nỗi đau thành 3 cụm chính và xây dựng cây Opportunity Solution Tree (OST). |Định hình Cụm 1 (Đầu vào & Phân loại) thành trọng tâm cốt lõi của báo cáo nhóm với Outcome giảm thời gian tiếp nhận ban đầu. |
| Chọn candidate problem |Cùng nhóm đánh giá và chấm điểm ưu tiên các phương án đề xuất dựa trên bảng tiêu chí tác động và độ khả thi. | Loại bỏ 2 phương án phức tạp về xử lý hình ảnh nâng cao và chẩn đoán kỹ thuật sâu, chốt chọn duy nhất bài toán Phân loại & Định tuyến ticket.|
| Kiểm chứng / research |Thực hiện khảo sát nhỏ với 2 nhân viên CSKH và rà soát các nghiên cứu về độ trễ định tuyến ticket vận hành đô thị. | Xác nhận lại giả định thời gian đọc thủ công (2.0 phút/ticket) và khoảng thời gian phản hồi chung dao động từ 2–4 giờ.|
| Quy trình nhóm |Vẽ sơ đồ quy trình hiện tại (As-Is) và đề xuất sơ đồ tương lai (To-Be) có sự tham gia của mô hình phân loại. |Xác định chính xác bước nghẽn tại khâu đọc hiểu thủ công và lồng ghép điểm kiểm duyệt con người (Human-in-the-loop). |
| Problem Statement | Cùng nhóm thảo luận viết Phát biểu bài toán v0 và tinh chỉnh thành phiên bản v1 theo cấu trúc 6 trường.| Định hình chính xác baseline 4.5 phút, mục tiêu rút xuống 1.5 phút và phương pháp đo lường qua log thời gian thực trên CRM.|
| Mức can thiệp AI |Phân tích 4 mức độ can thiệp từ Rule-based đơn thuần đến Agentic Loop tự động hoàn toàn. |Thuyết phục nhóm lựa chọn mức Workflow / Augmented (Gợi ý 1-click cho nhân viên) thay vì cho AI tự động gửi đi để đảm bảo an toàn.|
| Quyết định |Tham gia đánh giá 4 loại rủi ro (kỹ thuật, vận hành, dữ liệu, tuân thủ) để ra quyết định cuối cùng. | Nhóm thống nhất ra quyết định NOT YET (chưa triển khai ngay), yêu cầu thu thập đủ 1.000 log ticket thực tế để kiểm định baseline trước.|

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan |Gợi ý thêm các lăng kính nỗi đau trong vận hành khu đô thị lớn từ mô tả thực tế. |Giúp mở rộng góc nhìn sang các nỗi đau hiện trường như đứt gãy thông tin giao ca và chậm báo cáo. |AI hay đưa ra các giải pháp kỹ thuật viễn vông (như dùng nhận diện khuôn mặt hay AI tự động sửa chữa). |Bỏ toàn bộ các gợi ý mang tính giải pháp, giữ lại các mô tả thực trạng và số liệu đo đạc thực tế. |
| CP2 Problem Card |Phản biện tính logic của Problem Card 1 và kiểm tra xem có bị thiếu sót nguyên nhân cốt lõi không. | Chỉ ra rất đúng việc tôi đang giả định chủ quan về thời gian đọc 2.0 phút mà chưa có log CRM chính thức.|AI đề xuất thay thế toàn bộ nhân viên CSKH bằng Chatbot tự động trả lời cư dân mà không quan tâm an toàn vận hành. |Giữ nguyên quy trình con người duyệt (Human-in-the-loop) và bổ sung yêu cầu xác minh số liệu log thực tế. |
| CP4 Research |Tóm tắt các báo cáo nghiên cứu về thời gian xử lý ticket CSKH trong các ngành dịch vụ vận hành. |Giúp tổng hợp nhanh các chỉ số Benchmark thời gian xử lý ticket tiêu chuẩn trên thế giới. |Trích dẫn một số số liệu không rõ nguồn gốc và mang tính tổng quát chung chung. |Rà soát lại tài liệu, chỉ trích dẫn các con số có thể đối chiếu với thực tế vận hành tòa nhà Vinhomes.|
| CP5 Quy trình |Kiểm tra tính hợp lý của sơ đồ luồng dữ liệu As-Is và To-Be. |Gợi ý bổ sung bước xử lý ngoại lệ (Fallback) khi mô hình AI trả về độ tin cậy thấp (< 85%). |Cho rằng AI có thể phân loại chính xác 100% mọi trường hợp mà không cần luồng chuyển giao thủ công. | Bổ sung bắt buộc nhãn manual_review cho các ca có độ tin cậy thấp hoặc thuộc nhóm sự cố nhạy cảm/an ninh.|
| CP5–6 Problem Statement |Rà soát cấu trúc 6 trường của Problem Statement để đảm bảo tính chặt chẽ. |Chỉ ra điểm thiếu sót trong việc định nghĩa phương pháp đo lường (Measurement method) ở bản v0. |Viết phát biểu bài toán quá dài dòng và bị lồng ghép các từ ngữ tiếp thị giải pháp AI. |Chỉnh sửa lại ngắn gọn, bám sát các con số baseline (4.5 phút) và mục tiêu (1.5 phút) đo lường được. |
| CP6 Mức can thiệp / quyết định |Gợi ý danh mục các rủi ro kỹ thuật và vận hành khi triển khai mô hình phân loại text tiếng Việt. |Đưa ra các rủi ro thực tế về việc AI bị lừa bởi prompt injection hoặc ngôn ngữ teen/viết tắt của cư dân. |Khuyên nhóm ra quyết định GO ngay lập tức vì công nghệ LLM đã rất hiện đại. |Quyết định chọn NOT YET vì thực tế dự án chưa có bộ dữ liệu log được gán nhãn chuẩn để train/eval model. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Khi lắng nghe phần trình bày Top 3 Problem Cards của các thành viên khác trong nhóm, bài học lớn nhất mà tôi rút ra được là sự khác biệt rất lớn về góc nhìn giữa các vị trí vận hành trong cùng một hệ thống. Ban đầu, tôi chỉ tập trung duy nhất vào góc nhìn của nhân viên CSKH tại tổng đài – những người phải trực tiếp mở và đọc hàng trăm văn bản thô từ cư dân gửi về. Tuy nhiên, khi nghe các bạn phân tích bài toán dưới góc nhìn của kỹ thuật viên hiện trường hay cấp quản lý ban vận hành, tôi mới nhận ra rằng nút thắt không chỉ nằm ở khâu đọc hiểu ban đầu. Một bạn trong nhóm đã chỉ ra rằng ngay cả khi ticket được phân loại đúng phòng ban, việc thiếu thông tin chi tiết về vị trí căn hộ hoặc ảnh chụp hiện trạng mờ câm vẫn khiến kỹ thuật viên mất tới vài tiếng đồng hồ phản hồi qua lại. Điều này giúp tôi hiểu rằng một bài toán sản phẩm AI tốt không thể giải quyết đơn độc một điểm nghẽn cục bộ mà phải đặt trong toàn bộ bức tranh dòng chảy thông tin (end-to-end workflow). Ngoài ra, tôi cũng học được cách các bạn sử dụng dữ liệu thực tế để chứng minh nỗi đau thay vì chỉ dùng các câu cảm thán chung chung. Việc định lượng được số lần cư dân phàn nàn hay số phút lãng phí mỗi ca trực khiến bài toán trở nên vô cùng thuyết phục và cấp thiết.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Trong giai đoạn đầu thảo luận tại Checkpoint 3, nhóm tôi đã vướng phải tư duy "solution-first" một cách rất rõ ràng. Ngay khi chốt chọn use case phản ánh cư dân Vinhomes, phản ứng tự nhiên của cả nhóm là lập tức nhảy vào thảo luận xem nên dùng mô hình LLM nào, áp dụng công nghệ RAG hay Fine-tune Gemini để tự động trả lời và định tuyến ticket. Chúng tôi đã hào hứng vẽ ra kịch bản một hệ thống AI siêu việt có thể thay thế hoàn toàn công việc phân loại của nhân viên CSKH. Tuy nhiên, nhóm chỉ thực sự "bừng tỉnh" khi giảng viên và bước kiểm tra quy trình yêu cầu chúng tôi phải mô tả chính xác sơ đồ As-Is kèm số liệu thời gian cho từng bước thủ công. Lúc này, khi ngồi phân tích kỹ từng thao tác, chúng tôi mới nhận ra mình chưa hề đo đạc chính xác thời gian đọc mô tả tốn bao nhiêu phút, và cũng chưa xem xét liệu một cây danh mục Form/Dropdown chuẩn hóa trên App cư dân (giải pháp Non-AI) có thể giải quyết được 60-70% vấn đề hay không. Để xử lý tình trạng này, nhóm đã chủ động dừng toàn bộ việc thảo luận về công nghệ LLM, quay trở lại viết lại Job Story cho đúng đối tượng nhân viên tổng đài và thực hiện khảo sát nhỏ để đo thời gian đọc hiểu thực tế trước khi bàn tiếp về AI.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Tôi đã hoàn toàn đổi ý sau một lần bị phản biện rất gay gắt từ một bạn trong nhóm liên quan đến nguyên nhân gốc rễ của điểm nghẽn đọc ticket. Ban đầu, ở bản nháp Problem Card 1, tôi kiên quyết bảo vệ quan điểm rằng nhân viên CSKH mất trung bình 2.0 phút để xử lý một ticket là do cư dân viết quá dài dòng, diễn đạt lủng củng hoặc đính kèm quá nhiều hình ảnh không liên quan. Tôi cho rằng AI là giải pháp duy nhất để "đọc nhanh" và tóm tắt văn bản thô này. Nhưng bạn trong nhóm đã phản biện lại rằng: "Nếu danh mục phòng ban nội bộ của Vinhomes vốn đã bị chồng chéo (ví dụ: sự cố rò rỉ nước từ máy lạnh vừa thuộc đội Điện lạnh vừa thuộc đội Bảo trì tòa nhà), thì dù cư dân có viết ngắn gọn 1 câu, nhân viên vẫn phải mất 2 phút ngồi phân vân không biết tick chọn đơn vị nào!". Câu hỏi phản biện này chạm đúng vào bản chất quy trình. Tôi nhận ra mình đã đổ lỗi hoàn toàn cho đầu vào của cư dân mà bỏ qua sự bất cập trong cấu trúc danh mục nội bộ. Sau buổi họp đó, tôi đã thay đổi báo cáo cá nhân, bổ sung việc tái cấu trúc và chuẩn hóa cây phân loại phòng ban thành một điều kiện tiên quyết (Non-AI step) phải làm song song trước khi đưa mô hình AI vào gợi ý nhãn.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Kết quả kiểm chứng thực tế qua việc phỏng vấn ngắn 2 nhân viên CSKH và rà soát tài liệu vận hành đã mang lại cho tôi hai sự bất ngờ lớn. Điều bất ngờ đầu tiên là thời gian phản hồi tổng thể (Lead time) của một ticket từ lúc cư dân gửi đến khi kỹ thuật viên có mặt thực tế dao động tới 2–4 giờ, nhưng thời gian thao tác kỹ thuật thực sự để sửa chữa đôi khi chỉ mất 15 phút. Toàn bộ khoảng thời gian lãng phí còn lại nằm ở các "khoảng chết" chờ chuyển giao, trong đó khâu nằm đợi phân loại ban đầu chiếm một tỷ lệ đáng kể vào giờ cao điểm. Điều bất ngờ thứ hai liên quan đến tâm lý của chính nhân viên CSKH. Trước khi khảo sát, tôi cứ nghĩ nhân viên sẽ rất hào hứng nếu có một hệ thống AI tự động phân loại và chuyển thẳng ticket đi để họ bớt việc. Nhưng thực tế, họ lại tỏ ra vô cùng lo ngại về rủi ro nếu AI phân loại sai (ví dụ: chuyển nhầm một sự cố báo cháy giả hoặc rò rỉ khí gas thành sự cố vệ sinh thông thường), vì khi đó chính nhân viên trực ca sẽ là người chịu trách nhiệm kỷ luật. Phát hiện này đã làm thay đổi hoàn toàn thiết kế hệ thống của nhóm tôi: từ ý định tự động hóa 100% chuyển sang mô hình Human-in-the-loop (AI chỉ đóng vai trò Co-pilot gợi ý nhãn 1-click cho con người duyệt).

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Điều khó khăn nhất đối với tôi khi hoàn thiện bản Phát biểu bài toán (Problem Statement) theo cấu trúc 6 trường chính là việc phải tách biệt hoàn toàn giữa "vấn đề/điểm nghẽn" và "giải pháp kỹ thuật", đồng thời phải đưa ra được các con số baseline thực sự có căn cứ. Khi viết bản v0, tôi rất dễ bị quen tay đưa ngay các thuật ngữ như "Triển khai mô hình Gemini 2.5 Flash để tự động hóa" vào phần phát biểu bài toán. Việc kìm hãm mong muốn nói về giải pháp để chỉ tập trung mô tả nỗi đau của nhân viên CSKH khi tốn 4.5 phút cho một ticket tiếp nhận đòi hỏi sự tư duy cực kỳ kỷ luật. Bên cạnh đó, việc xác định phương pháp đo lường (Measurement method) cũng là một bài toán hóc húa. Chúng tôi phải đấu tranh xem làm sao để đo được chính xác tỷ lệ phân loại sai (hiện tại ước tính ~12%) khi hệ thống CRM cũ chưa hề có tính năng tự động ghi log thời gian phản hồi của nhân viên theo từng click. Việc phải quy đổi một nỗi đau định tính thành các chỉ số định lượng khắt khe (baseline 4.5 phút -> target 1.5 phút) chính là phần ngốn nhiều thời gian và gây tranh luận gay gắt nhất trong nhóm.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu được quay lại làm lại bài tập này từ đầu, thay đổi lớn nhất của tôi là sẽ dành ngay 2 ngày đầu tiên để đi thu thập và quan sát dữ liệu thực tế tại một ban quản lý tòa nhà thực sự thay vì dành quá nhiều thời gian ngồi giả lập các con số trên giấy. Việc có dữ liệu thực tế sớm sẽ giúp nhóm đỡ mất thời gian tranh cãi về các giả định mơ hồ. Ngoài ra, tôi sẽ phản biện nhóm một cách mạnh mẽ hơn ở hai điểm cốt lõi. Thứ nhất, tôi sẽ kiên quyết yêu cầu nhóm phải làm rõ và thử nghiệm giải pháp Non-AI (như thiết kế lại Form nhập dữ liệu chuẩn hóa trên App) một cách triệt để trước khi chấp nhận đưa AI vào phạm vi dự án. Thứ hai, ở phần đánh giá rủi ro, tôi sẽ đẩy mạnh việc phản biện về tính khả thi của dữ liệu huấn luyện (Training data). Nhóm đã quá lạc quan khi cho rằng dữ liệu ticket lịch sử của Vinhomes đã sẵn sàng để train model, trong khi thực tế dữ liệu văn bản thô của cư dân chứa rất nhiều từ viết tắt, tiếng địa phương và thông tin cá nhân (PII) chưa được làm sạch. Nếu phản biện quyết liệt hơn, nhóm sẽ định hình được một lộ trình chuẩn bị dữ liệu (Data pipeline) thực tế hơn rất nhiều.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.
Bài toán của nhóm tập trung vào điểm nghẽn tại khâu đầu vào khi nhân viên CSKH tốn trung bình 2.0 phút đọc thủ công mỗi ticket để phân loại và định tuyến phản ánh cư dân Vinhomes. Quy trình tiếp nhận hiện tại trải qua 5 bước thao tác thủ công kéo dài tổng cộng 4.5 phút/ticket, dẫn đến sự tồn đọng nghiêm trọng vào các khung giờ cao điểm. Để giải quyết, mục tiêu đo lường (metric) được đặt ra là rút ngắn tổng thời gian tiếp nhận xuống dưới 1.5 phút/ticket và giảm tỷ lệ chuyển sai bộ phận từ 12% xuống dưới 3%. Nhằm đảm bảo an toàn vận hành, ranh giới hệ thống (boundary) quy định nghiêm ngặt cấm AI tự động gửi tin nhắn hoặc tự định tuyến các ca khẩn cấp liên quan đến an ninh, cháy nổ, tài chính mà bắt buộc phải gắn thẻ duyệt. Do đó, mức độ can thiệp AI được lựa chọn là dạng Workflow / Human-in-the-loop (Mô hình đóng vai trò Co-pilot đưa ra gợi ý phân loại 1-click để nhân viên kiểm duyệt). Cuối cùng, nhóm đi đến quyết định NOT YET (chưa triển khai ngay) vì dự án hiện chưa có đủ bộ dữ liệu log thực tế được làm sạch và gán nhãn chuẩn để kiểm định mô hình.
---

## 7. Tài liệu tham khảo
Báo cáo khảo sát vận hành Ban quản lý khu đô thị Vinhomes (Dữ liệu quan sát nội bộ ca trực CSKH).

Tài liệu hướng dẫn môn học Day 02 — AI Product Scoping (Vin Smart Future Framework).

Trích dẫn Benchmark về thời gian xử lý ticket và tỷ lệ chuyển giao trong ngành Quản lý Bất động sản & Dịch vụ khách hàng (Customer Support Benchmark Report).
-
