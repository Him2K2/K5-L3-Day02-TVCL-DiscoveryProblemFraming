# Báo cáo cá nhân — 2A202603358_NguyenThanhLiem

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Thanh Liêm
- MSSV: 2A202603358
- Email trường (không bắt buộc, repo có thể để public): liemt0165@gmail.com
- Tên nhóm:
- Link repo nhóm:

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi chuẩn bị commit bài nộp/code lên repo chung, tôi muốn rà soát nhanh các file đã sửa và đối chiếu với checklist bắt buộc, để không commit nhầm file rác hoặc sót file quan trọng bị trừ điểm. | Sinh viên, lập trình viên trong nhóm (3–4 người) | Mất 15–20 phút rà soát thủ công mỗi lần nộp bài; 2 lần/tuần; từng có bạn bị trừ 5 điểm vì quên đổi tên file template. |
| 2 | Pain từ người khác | Khi có thành viên mới vào nhóm làm dự án, nhóm trưởng muốn các bạn tự thiết lập đúng remote/branch và phân quyền push, để không phải ngắt quãng công việc vì trả lời đi trả lời lại các lỗi permission hay sai nhánh. | Nhóm trưởng, thành viên mới (3–4 người) | Nhóm trưởng mất 30–45 phút đầu mỗi đồ án/lab để hướng dẫn từng bạn; bằng chứng là chuỗi tin nhắn hỏi lỗi git push lúc nửa đêm. |
| 3 | Pain từ người khác | Khi trạm sạc công cộng kín chỗ vào giờ cao điểm, tài xế xe điện muốn nhận diện được các xe đã sạc đầy nhưng vẫn chiếm chỗ đỗ, để yêu cầu nhường trụ hoặc được ban quản lý điều phối sạc kịp thời mà không phải chờ đợi hàng giờ. | Tài xế xe điện cá nhân (VinFast) và taxi Xanh SM | Mất 30–60 phút chờ đợi hoặc phải chạy sang trạm khác; tình trạng xe sạc đầy chây ì diễn ra liên tục vào khung 17h–20h. |
| 4 | Lặp lại | Khi các đội thợ nội thất đến thi công lúc 8h sáng, nhân viên an ninh sảnh muốn đối chiếu nhanh danh sách công nhân với giấy phép thi công đã duyệt trên hệ thống, để cấp thẻ ra vào trong 1 phút mà không gây ùn tắc sảnh lễ tân. | Bảo vệ sảnh, lễ tân tòa nhà Vinhomes & Nhà thầu | Mỗi sáng có 30–40 công nhân xếp hàng từ 7h45–8h30; mất 3–5 phút/người dò sổ đăng ký giấy; thường xuyên tắc thang máy vận chuyển. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi cư dân gửi hàng chục phản ánh sự cố (mất nước, hỏng đèn, tiếng ồn, rác thải) mỗi ngày trên App, nhân viên ban quản lý muốn phân loại mức độ khẩn cấp và chuyển đúng bộ phận xử lý, để giải quyết sự cố trong 30 phút mà không phải đọc thủ công từng phiếu. | Nhân viên CSKH/Ban quản lý Vinhomes, Cư dân | Tiếp nhận 50–80 phản ánh/ngày/cụm tòa; mất 10–15 phút/phiếu đọc mô tả, xem ảnh và chuyển tiếp; 15% phản ánh bị gán nhầm đội xử lý. |
| 6 | Tốn thời gian | Khi bệnh nhân chuẩn bị ra viện, bác sĩ điều trị muốn trích xuất nhanh các chỉ số lâm sàng và kết quả xét nghiệm từ bệnh án điện tử, để soạn thảo bản tóm tắt hồ sơ xuất viện (Discharge Summary) bằng ngôn ngữ phổ thông, giúp bệnh nhân hiểu rõ tình trạng bệnh mà bác sĩ không mất 30 phút viết tay. | Bác sĩ điều trị, Bệnh nhân xuất viện (Vinmec) | Bác sĩ mất 25–35 phút/hồ sơ xuất viện; trung bình 5–10 bệnh nhân xuất viện/khoa/ngày; chiếm dụng thời gian khám bệnh nhân mới. |
| 7 | Pain từ người khác | Khi có học sinh xin nghỉ ốm hoặc đổi điểm đón đột xuất lúc sáng sớm, cô giám sát xe buýt muốn danh sách tuyến đón được cập nhật tự động theo thứ tự lộ trình, để tài xế không phải dừng chờ vô ích làm muộn giờ học của cả xe. | Giám sát xe buýt (Vinschool), Tài xế, Phụ huynh | Tuyến có 15–20 học sinh; mỗi sáng có 2–3 phụ huynh báo nghỉ gấp qua tin nhắn riêng; xe buýt bị trễ 10–15 phút vào giờ cao điểm nếu phải dừng chờ. |
| 8 | Cần đọc, tổng hợp nhiều thông tin | Khi giáo viên nhắn tin báo sự cố trong giờ dạy ở các cơ sở, điều phối viên trung tâm muốn phân loại nhanh nội dung (lỗi phần mềm/máy tính, hỏng máy chiếu/điều hòa, hay thiếu tài khoản) và chuyển ngay đến đúng người phụ trách, để sự cố được xử lý trong vòng 5 phút mà không phải lướt đọc thủ công từng nhóm chat. | Điều phối viên học vụ, Giáo viên trung tâm tin học | Trung tâm có hơn 100 cơ sở với 500+ lớp/ngày; phát sinh 50-60 sự cố/ngày; khâu đọc và forward thủ công mất 10–15 phút/sự cố; 20% tin nhắn bị sót. |
| 9 | Tốn thời gian | Khi một giáo viên gặp sự cố đột xuất không thể đứng lớp (ốm, kẹt xe, việc khẩn), quản lý đào tạo muốn tìm nhanh các giáo viên đang có lịch rảnh và ở gần cơ sở đó nhất, để gửi lời mời nhận lớp thay thế trong 10 phút mà không phải gọi điện dò hỏi từng người. | Quản lý đào tạo, Đội ngũ giáo viên/trợ giảng | Phát sinh rải rác tùy khu vực, mất 10–20 phút để kiểm tra lại lịch của giáo viên, sau khi gửi yêu cầu còn mất thêm thời gian di chuyển. |
| 10 | Lặp lại | Khi bắt đầu và kết thúc mỗi ca dạy tại cơ sở, giáo viên muốn ghi nhận nhanh tình trạng thiết bị phòng máy và tóm tắt tiến độ bài học hôm nay, để trung tâm nắm bắt chất lượng và thiết bị hỏng mà giáo viên không phải mất 20 phút gõ báo cáo dài dòng vào form. | Giáo viên đứng lớp, Bộ phận Quản lý chất lượng (QA) | Mỗi giáo viên dạy 2–3 ca/ngày; mất 15–20 phút/ngày gõ lại các trường thông tin lặp lại vào form. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý giữ lại:** Sau khi tự scan các vấn đề gặp phải trong việc làm đồ án nhóm và quản lý vận hành đào tạo, tôi có dùng AI để mở rộng góc nhìn sang các mô hình vận hành quy mô lớn và giữ lại ý #3 (chiếm chỗ trạm sạc xe điện), #5 (phân loại phản ánh cư dân) và #6 (tóm tắt bệnh án xuất viện) vì đây là các nỗi đau rất thực tế, có quy trình và đối tượng chịu ảnh hưởng rõ ràng.
- **Ý loại bỏ:** Loại bỏ các gợi ý của AI như "Trợ lý AI tự động lập trình và review toàn bộ dự án" hay "Chatbot tự động tư vấn pháp lý" vì phạm vi quá rộng, thiếu quy trình thực tế có thể kiểm chứng trong buổi lab và không có baseline đo lường cụ thể.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Phân loại và điều phối sự cố từ nhóm chat các cơ sở (#8) | Quy trình rõ, diễn ra hàng ngày ở 5 cơ sở, bottleneck phân loại thủ công làm gián đoạn giờ học, vừa sức phân tích trong buổi lab. | Giáo viên có chịu nhắn tin theo mẫu quy định không hay vẫn nhắn tự do ngắn gọn ("phòng 301 hỏng máy")? |
| 2 | Tìm và điều phối giáo viên dạy thay khẩn cấp theo lịch và vị trí (#9) | Tác động lớn (ảnh hưởng trực tiếp đến việc lớp có bị hủy hay không), số liệu thời gian đo được rõ ràng (10–20p kiểm tra + thời gian di chuyển). | Việc giáo viên từ chối nhận lớp (bận việc đột xuất) có dự đoán trước được không hay vẫn cần con người gọi điện thuyết phục? |
| 3 | Nhận diện và xử lý xe sạc đầy chiếm chỗ tại trạm sạc công cộng (#3) | Nỗi đau lớn của cộng đồng xe điện, tần suất cao vào giờ cao điểm, có bối cảnh thực tế rõ ràng. | Dữ liệu trạng thái sạc từ trụ sạc và xe có được cấp quyền truy cập để hệ thống bên ngoài nhận biết kịp thời không? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi giáo viên nhắn tin báo sự cố trong giờ dạy ở các cơ sở, điều phối viên trung tâm muốn phân loại nhanh nội dung (lỗi phần mềm/máy tính, hỏng máy chiếu/điều hòa, hay thiếu tài khoản) và chuyển ngay đến đúng người phụ trách, để sự cố được xử lý trong vòng 5 phút mà không phải lướt đọc thủ công từng nhóm chat. |
| Actor | Phòng giáo vụ (1–2 người) và Giáo viên đứng lớp tại 5 cơ sở trung tâm tin học |
| Thời điểm / bối cảnh | Trong các ca học (sáng 8h–11h30, chiều 14h–17h30, tối 18h–21h), khi lớp đang học thì phát sinh sự cố kỹ thuật/phòng học |
| Quy trình hiện tại (3–7 bước) | 1. Giáo viên phát hiện sự cố, nhắn tin mô tả kèm ảnh vào nhóm chat Zalo/Telegram riêng của cơ sở đó (1')<br>2. Điều phối viên trung tâm đọc tin nhắn trong các nhóm chat cơ sở (3')<br>3. Điều phối viên phòng giáo vụ đọc nội dung, xác định loại sự cố: IT phần mềm, Kỹ thuật phần cứng, hay Học vụ (4')<br>4. Điều phối viên tìm người/bộ phận phụ trách cơ sở đó và copy forward tin nhắn, tag tên người phụ trách (3')<br>5. Kỹ thuật viên/Học vụ xác nhận tiếp nhận và đến phòng xử lý (4') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 và 4: Khâu đọc lọc tin nhắn giữa các cuộc hội thoại và forward thủ công mất 7–8 phút, dễ bị sót tin nhắn khi có nhiều lớp cùng báo sự cố đầu ca |
| Impact (nếu không giải thì sao) | Mỗi ngày có 8–12 sự cố trên hàng chục cơ sở; khi xử lý chậm trễ khiến học viên mất thời gian (tiết học chỉ 45p), gián đoạn bài giảng và ảnh hưởng uy tín trung tâm |
| Success metric (baseline → target) | Baseline: 12–15 phút từ lúc báo đến khi kỹ thuật nhận việc; 20% tin nhắn bị phản hồi trễ.<br>Target: Giảm thời gian điều phối xuống dưới 3 phút; tỷ lệ phân loại đúng và chuyển ngay đạt > 95%.<br>Cách đo: Bấm giờ từ timestamp tin nhắn báo của giáo viên đến timestamp kỹ thuật viên bấm nhận việc trên hệ thống trong 2 tuần pilot. |
| Phương án không dùng AI | Dùng Google Form hoặc bot cú pháp lệnh cố định (ví dụ gõ `/baoloi [Phong] [LoaiLoi]`) để tự route tin nhắn theo từ khóa. Nhược điểm: Giáo viên lúc đang đứng lớp rất ngại mở form hoặc nhớ đúng cú pháp lệnh. |
| Giả thuyết về AI (nếu có) | AI đọc hiểu ngôn ngữ tự nhiên từ tin nhắn chat của giáo viên (kể cả viết tắt, chụp ảnh màn hình lỗi), tự động trích xuất: [Cơ sở], [Phòng], [Loại sự cố], [Mức độ khẩn cấp] và tự động route thông báo đến đúng nhóm kỹ thuật. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 15 phút/sự cố

[1. GV nhắn chat cơ sở: 1']
→ [2. Điều phối viên check chat: 3']
→ [3. Đọc hiểu & phân loại loại lỗi: 4'] ← BOTTLENECK
→ [4. Tìm người & forward thủ công: 3'] ← BOTTLENECK
→ [5. Kỹ thuật viên xác nhận & tới xử lý: 4']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi một giáo viên gặp sự cố đột xuất không thể đứng lớp (ốm, kẹt xe, việc khẩn), quản lý đào tạo muốn tìm nhanh các giáo viên đang có lịch rảnh và ở gần cơ sở đó nhất, để gửi lời mời nhận lớp thay thế trong 10 phút mà không phải gọi điện dò hỏi từng người. |
| Actor | Quản lý đào tạo / Điều phối lịch giảng và Đội ngũ giáo viên/trợ giảng (30–50 người) |
| Thời điểm / bối cảnh | Khoảng 30–60 phút trước giờ vào ca học (hoặc ngay đầu ca), giáo viên gọi điện/nhắn tin báo hủy ca khẩn cấp |
| Quy trình hiện tại (3–7 bước) | 1. Quản lý tiếp nhận thông tin xin nghỉ đột xuất của giáo viên (2')<br>2. Mở file Excel thời khóa biểu toàn trung tâm, dò tìm danh sách giáo viên có chuyên môn dạy môn này và đang trống lịch ở ca đó (10')<br>3. Lọc tiếp xem giáo viên nào đang dạy ca liền trước ở cơ sở gần đó hoặc có địa chỉ gần cơ sở phát sinh sự cố (5')<br>4. Gọi điện thoại hoặc nhắn tin riêng tuần tự cho từng giáo viên theo danh sách ưu tiên để mời dạy thay (15')<br>5. Nhận xác nhận đồng ý của một giáo viên, bàn giao giáo án và cập nhật lại lịch (3') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2, 3 và 4: Mất 10–20 phút kiểm tra lại lịch của giáo viên và vị trí cơ sở; sau khi gửi yêu cầu gọi tuần tự từng người rất mất thời gian; sau đó còn mất thêm thời gian di chuyển của giáo viên nhận lớp |
| Impact (nếu không giải thì sao) | Phát sinh rải rác tùy khu vực (3–5 ca/tuần); mất 30–45 phút điều phối; nhiều ca tìm không kịp người khiến lớp phải tự học hoặc trung tâm phải hủy ca, sắp xếp học bù tốn chi phí |
| Success metric (baseline → target) | Baseline: Mất 30–45 phút để tìm và chốt được người dạy thay; tỷ lệ hủy lớp do không tìm được người là ~15%.<br>Target: Giảm thời gian tìm và gửi yêu cầu xuống dưới 5 phút, chốt người dạy thay trong vòng 15 phút; tỷ lệ hủy lớp giảm về 0%.<br>Cách đo: Ghi nhận thời gian từ lúc nhận báo nghỉ đến lúc có giáo viên bấm nhận lớp trên bảng log điều phối. |
| Phương án không dùng AI | Quản lý lịch trên Google Sheets / Notion có bộ lọc tự động theo ca rảnh và cơ sở; gửi tin nhắn broadcast vào nhóm chung "Tìm người dạy thay". Nhược điểm: Nhắn nhóm chung dễ bị trôi, GV ít chú ý, không tính được khoảng cách di chuyển thực tế. |
| Giả thuyết về AI (nếu có) | Hệ thống dựa trên lịch giảng, khoảng cách di chuyển và lịch sử nhận lớp để tự động gợi ý top 3 ứng viên phù hợp nhất và gửi thông báo mời nhận ca tuần tự với nút xác nhận nhanh 1 chạm. |
| Cảm nhận nhanh | Rule (hoặc Workflow đơn giản) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 35 phút/lần điều phối

[1. Nhận báo nghỉ gấp: 2']
→ [2. Mở Excel dò lịch rảnh môn học: 10'] ← BOTTLENECK
→ [3. Tra cứu vị trí/cơ sở gần: 5']
→ [4. Gọi điện tuần tự từng GV: 15']     ← BOTTLENECK
→ [5. Chốt người & gửi giáo án: 3']
(Chưa tính thời gian GV di chuyển tới cơ sở)
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi trạm sạc công cộng kín chỗ vào giờ cao điểm, tài xế xe điện muốn nhận diện được các xe đã sạc đầy nhưng vẫn chiếm chỗ đỗ, để yêu cầu nhường trụ hoặc được ban quản lý điều phối sạc kịp thời mà không phải chờ đợi hàng giờ. |
| Actor | Tài xế xe điện cá nhân (VinFast VF 3, VF 5, VF 8), tài xế taxi Xanh SM & Nhân viên an ninh/vận hành bãi đỗ xe |
| Thời điểm / bối cảnh | Giờ cao điểm 17h–20h tại các trạm sạc chung cư (Vinhomes Smart City/Ocean Park) hoặc TTTM Vincom |
| Quy trình hiện tại (3–7 bước) | 1. Tài xế đến trạm sạc, thấy toàn bộ trụ sạc đều có xe đỗ (1')<br>2. Tài xế đỗ xe chờ hoặc xuống xe đi bộ quanh các trụ để nhìn màn hình trụ xem xe nào đã sạc 100% hoặc cắm súng nhưng không sạc (10')<br>3. Tìm số điện thoại dán trên kính xe hoặc nhờ bảo vệ bãi xe phát loa thông báo chủ xe xuống đánh xe đi (12')<br>4. Chờ chủ xe ra di chuyển xe hoặc bảo vệ giải quyết (20')<br>5. Lùi xe vào trụ sạc trống và cắm súng sạc (2') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 và 3: Việc phải đi kiểm tra thủ công màn hình từng trụ sạc và chờ đợi liên hệ chủ xe chiếm chỗ mất 20–25 phút, gây ức chế và tranh chấp giữa các tài xế |
| Impact (nếu không giải thì sao) | Mất 30–60 phút cho mỗi lần sạc; lãng phí công suất trạm sạc trong giờ cao điểm; gây xung đột giữa xe cá nhân và xe taxi công nghệ; ảnh hưởng trải nghiệm sử dụng xe điện |
| Success metric (baseline → target) | Baseline: Thời gian chờ trung bình 45 phút/xe vào giờ cao điểm; tỷ lệ bức xúc phản ánh chiếm chỗ cao.<br>Target: Giảm thời gian phát hiện trụ trống/xe đầy xuống dưới 3 phút; giải phóng trụ sạc trong vòng 10 phút sau khi sạc đầy.<br>Cách đo: Thống kê thời gian chiếm trụ sau khi pin đầy (idle time) và thời gian chờ của xe trên ứng dụng trạm sạc. |
| Phương án không dùng AI | Áp dụng phí phạt đỗ xe quá giờ tự động (tính tiền theo phút sau khi sạc đầy 10 phút); bảo vệ bãi xe dán vé cảnh báo. Nhược điểm: Nhiều người chấp nhận trả phí phạt để có chỗ đỗ qua đêm, hoặc xe xăng vào đỗ thì không phạt qua app được. |
| Giả thuyết về AI (nếu có) | Camera AI tại trạm sạc kết hợp cảm biến trụ sạc nhận diện biển số xe sạc đầy quá hạn hoặc xe xăng đỗ sai chỗ, tự động kích hoạt loa thông báo tại chỗ và gửi thông báo khẩn cấp đến app của chủ xe. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 45 phút

[1. Đến trạm, thấy kín chỗ: 1']
→ [2. Đi bộ dò màn hình từng trụ sạc: 10'] ← BOTTLENECK
→ [3. Tìm số liên hệ / báo bảo vệ: 12']   ← BOTTLENECK
→ [4. Chờ chủ xe ra đánh xe đi: 20']
→ [5. Lùi vào và cắm sạc: 2']
```

### Card muốn pitch nhất

- Card số: 1 (Phân loại và điều phối sự cố từ nhóm chat các cơ sở)
- Vì sao: Quy trình rất rõ, bottleneck cụ thể đo được bằng phút (mất 7–8 phút phân loại & chuyển tiếp thủ công), tần suất cao (8–12 sự cố/ngày), phạm vi vừa vặn cho buổi lab và có thể so sánh sâu sắc giữa phương án Rule vs Workflow AI.
- Câu hỏi muốn nhóm phản biện: "Nếu trung tâm áp dụng một biểu mẫu Google Form bắt buộc hoặc bot gõ lệnh cố định (Rule) thay vì cho giáo viên gõ chat tự do, thì giáo viên có chịu dùng không và liệu phương án No AI / Rule đó đã đủ giải quyết bài toán mà không cần đến AI chưa?"

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| AI nhận xét rằng metric ở Card #1 ban đầu ghi chung chung "giảm thời gian chờ", chưa có baseline và cách đo cụ thể | Đồng ý | Đã bổ sung baseline cụ thể: "12–15 phút từ lúc báo đến khi nhận việc; 20% tin nhắn bị trễ" và target "dưới 3 phút; tỷ lệ đúng > 95%", kèm cách đo đối chiếu timestamp tin nhắn trong 2 tuần pilot. |
| AI hoài nghi liệu Card #2 (tìm giáo viên dạy thay) có thật sự cần đến AI hay chỉ là bài toán lọc dữ liệu bảng tính (Rule-based)? | Đồng ý | Đã chỉnh trường "Cảm nhận nhanh" về mức **Rule (hoặc Workflow đơn giản)** và nêu rõ phương án No AI là bộ lọc lịch giảng Google Sheets + thông báo tự động. |
| AI chỉ ra Card #3 (trạm sạc) phụ thuộc vào phần cứng và quyền can thiệp vào hệ thống V-Green, khó pilot thực tế trong phạm vi lab | Đồng ý | Đã bổ sung rủi ro về quyền truy cập dữ liệu vào cột "Điều còn chưa chắc" trong bảng chọn top 3 và ưu tiên chọn Card #1 để pitch với nhóm. |

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
| CP1 Scan | Mở rộng góc nhìn sang các bối cảnh thực tế lớn (hệ sinh thái Vingroup, vận hành đào tạo đa cơ sở), và hỗ trợ chuẩn hóa các ý tưởng của tôi về đúng định dạng Job Story. | • Cung cấp khung cấu trúc chuẩn "Khi... tôi muốn... để..." không bị lẫn giải pháp.<br>• Gợi ý mở rộng sang các bài toán thực tế như trạm sạc xe điện VinFast, xử lý phản ánh cư dân Vinhomes. | • AI tự ý đưa vào các số liệu giả định/cảm tính không có căn cứ (tự thêm "tỷ lệ nộp báo cáo đúng giờ chỉ đạt 60%" vào bài toán giáo viên).<br>• Gợi ý một số bài toán quá vĩ mô/solution trá hình như "Trợ lý AI quản lý toàn diện dự án". | • Tôi đã yêu cầu loại bỏ số liệu 60% cảm tính ở bài toán 10.<br>• Tôi tự sửa lại đúng dấu hiệu thực tế của bài toán tìm giáo viên dạy thay (#9): "Phát sinh rải rác tùy khu vực, mất 10–20 phút để kiểm tra lịch của giáo viên, sau khi gửi yêu cầu còn mất thêm thời gian di chuyển".<br>• Chủ động loại bỏ bài toán tìm quyết định cũ (#3 cũ) vì phạm vi rộng và khó đo lường. |
| CP2 Problem Card | Đóng vai Product Manager hoài nghi để phản biện, bóc tách quy trình hiện tại thành các bước cụ thể và tìm điểm nghẽn (bottleneck) cho 3 bài toán tôi chọn (#8, #9, #3). | • Giúp mô hình hóa quy trình thành chuỗi 5 bước rõ ràng kèm thời gian ước tính.<br>• Chỉ ra chính xác các bước bottleneck (khâu đọc/lọc tin nhắn ở Card #1, khâu dò lịch và gọi điện tuần tự ở Card #2). | • AI có xu hướng thích "thần thánh hóa AI": ở Card #2 (tìm GV dạy thay), AI định hướng dùng AI để dự đoán và ghép đôi thông minh, trong khi thực tế chỉ cần logic lọc bảng tính.<br>• Với Card #3 (trạm sạc), AI bỏ qua rào cản về quyền truy cập phần cứng và dữ liệu đóng của hệ thống sạc công cộng. | • Tôi đã ép chặt cảm nhận can thiệp của Card #2 về mức Rule (hoặc Workflow đơn giản) thay vì dùng AI phức tạp, nêu rõ giải pháp No AI là bộ lọc Google Sheets.<br>• Bổ sung rào cản truy cập dữ liệu trạm sạc vào cột "Điều còn chưa chắc" của Card #3.<br>• Ép chuẩn lại Success Metric của Card #1: có baseline đo bằng tin nhắn thật trong 2 tuần pilot thay vì mục tiêu chung chung. |
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
