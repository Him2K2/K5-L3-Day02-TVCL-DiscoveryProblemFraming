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
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
