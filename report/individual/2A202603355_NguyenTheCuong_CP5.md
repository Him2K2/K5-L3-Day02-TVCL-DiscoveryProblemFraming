# CP5 — Quy trình trước/sau và Problem Statement v0

- Người tổng hợp: Nguyễn Thế Cường — 2A202603355.
- Nhóm: TVCL.
- Đề tài: Phân loại và chuyển phản ánh cư dân đến đúng bộ phận.
- Căn cứ: bài cá nhân của Hoàng Ngọc Minh Trí, [CP3](../team/cp3-hoi-tu-nhom.md) và [CP4](../team/cp4-kiem-chung-research.md).

> Đây là bản dự thảo để nhóm rà soát. Quy trình hiện tại và số liệu được kế thừa từ bài Trí, chưa đối chiếu phiếu quan sát gốc. CP4 chưa có phỏng vấn mới, nên CP5 chưa phải kết luận sau kiểm chứng. Quy trình tương lai và thời gian dự kiến bên dưới chưa được thử nghiệm. Bản này đặt trong individual theo cách tổ chức bài hiện tại; khi nhóm chốt cần tổng hợp vào báo cáo nhóm chung.

## 1. Quy trình hiện tại

Khi nhận phản ánh, nhân viên phải đọc nội dung, xem ảnh và tra đơn vị phụ trách rồi mới chuyển ticket. Nếu mô tả khó hiểu hoặc trách nhiệm phòng ban chưa rõ, nhân viên có thể phải hỏi thêm trước khi chuyển.

```text
HIỆN TẠI — 4.5 phút/ticket theo bài Trí, cần xác nhận lại

[1 Tiếp nhận ticket: 0.5'] → [2 Đọc mô tả và xem ảnh: 2.0'] ← BOTTLENECK THEO BÀI NGUỒN
→ [3 Xác định loại sự cố và tra đơn vị: 1.0']
→ [4 Gán nhãn, ưu tiên và đơn vị: 0.5'] → [5 Lưu và chuyển ticket: 0.5']
```

`'` là phút. Tổng trên là thời gian thao tác theo bài nguồn, chưa bao gồm thời gian chờ cư dân bổ sung hoặc chờ bộ phận nhận xử lý.

| Bước | Actor | Input | Output và chuyển giao | Thời gian/tần suất |
|---:|---|---|---|---|
| 1. Tiếp nhận | Nhân viên CSKH | Thông báo phản ánh mới | Ticket được mở → bước đọc nội dung | 0.5 phút/ticket theo bài Trí |
| 2. Đọc và xem ảnh | Nhân viên CSKH | Mô tả, ảnh và vị trí nếu có | Nội dung sự cố được hiểu sơ bộ → bước phân loại | 2.0 phút/ticket theo bài Trí |
| 3. Xác định đơn vị | Nhân viên CSKH | Nội dung sự cố, danh mục và trách nhiệm phòng ban | Nhóm sự cố và đơn vị dự kiến → bước gán thông tin | 1.0 phút/ticket theo bài Trí |
| 4. Gán thông tin | Nhân viên CSKH | Nhóm sự cố, quy định ưu tiên, đơn vị dự kiến | Ticket có nhãn và đơn vị tiếp nhận → bước lưu/chuyển | 0.5 phút/ticket theo bài Trí |
| 5. Lưu và chuyển | Nhân viên CSKH; bộ phận nhận | Ticket đã phân loại | Ticket chuyển tới Kỹ thuật/Dịch vụ/An ninh theo danh mục | 0.5 phút/ticket theo bài Trí |

**Bước nghẽn theo bài nguồn:** bước 2, chiếm khoảng 44% tổng thời gian thao tác. Tuy nhiên, thời gian đọc lâu chưa chứng minh nguyên nhân nằm ở cách cư dân diễn đạt; danh mục chồng chéo hoặc thông tin thiếu cũng có thể khiến nhân viên phải đọc lại. Cần kiểm tra riêng bước 2 và bước 3 trước khi chọn cách cải thiện.

Bài nguồn nêu 120 ticket/ca 8 giờ. Nếu nhân 120 với 4.5 phút sẽ thành 540 phút; vì chưa rõ số người và cách đo, không dùng phép nhân này để khẳng định mức quá tải hoặc số giờ tiết kiệm.

## 2. Quy trình tương lai đề xuất

Trước tiên cần thống nhất danh mục sự cố và đơn vị phụ trách. Sau đó thử biểu mẫu và Rule làm đối chứng. Chỉ thử hỗ trợ phân loại nội dung nếu cách đơn giản vẫn còn nhiều trường hợp khó; chưa chốt mức can thiệp AI ở CP5.

### 2.1. Các bước và vai trò

| Bước | Ai/cách xử lý | Input | Output | Ngân sách thời gian đề xuất |
|---:|---|---|---|---|
| 1. Mở và kiểm tra dữ liệu | Rule | Ticket, trường bắt buộc theo loại phản ánh | Đủ dữ liệu hoặc danh sách trường thiếu | 0.1 phút |
| 2. Chuẩn bị phương án phân loại | Rule; AI chỉ thử nếu cần | Ticket đủ dữ liệu và danh mục đã khóa | Nhóm sự cố, đơn vị gợi ý và căn cứ; có thể trả “chưa xác định” | 0.2 phút |
| 3. Kiểm tra và quyết định | Nhân viên CSKH | Nội dung gốc và gợi ý | Phân loại được duyệt/sửa hoặc chuyển xử lý thủ công | 0.8 phút |
| 4. Lưu và chuyển sau duyệt | Rule thực hiện theo xác nhận của nhân viên | Ticket đã được duyệt | Ticket chuyển đúng đơn vị; có log thao tác và người duyệt | 0.3 phút |

Tổng ngân sách mục tiêu: **1.4 phút/ticket đủ thông tin, thuộc danh mục đã thống nhất**. Đây là cách phân bổ mục tiêu để thử, không phải kết quả đo. Thời gian nhân viên phát hiện và sửa gợi ý phải nằm trong phép đo. Ticket thiếu thông tin hoặc chưa rõ đơn vị đi theo nhánh riêng và vẫn phải được báo cáo, không loại âm thầm để làm đẹp chỉ số.

```text
TƯƠNG LAI — mục tiêu 1.4 phút/ticket thông thường, chưa thử nghiệm

[1 Kiểm tra trường dữ liệu: 0.1']                          ← RULE
→ [2 Chuẩn bị nhóm sự cố và đơn vị gợi ý: 0.2']             ← RULE / AI NẾU CẦN THỬ
→ [3 Nhân viên xem nội dung gốc, duyệt hoặc sửa: 0.8']      ← CON NGƯỜI
→ [4 Lưu và chuyển theo xác nhận: 0.3']                    ← RULE

Thiếu thông tin → Nhân viên yêu cầu bổ sung; ghi riêng thời gian chờ.
Không rõ đơn vị / gợi ý không phù hợp → Nhân viên phân loại thủ công hoặc hỏi điều phối.
Rule/AI lỗi → Dùng danh mục và quy trình thủ công hiện tại; lưu lý do quay về.
```

### 2.2. Ranh giới và phương án quay về

- Nhân viên phải kiểm tra và xác nhận trước khi chuyển ticket trong pilot. AI, nếu được thử, chỉ gợi ý nhãn/đơn vị từ danh mục đã duyệt.
- Không tự tạo dữ kiện, sửa mô tả gốc, tự thêm phòng ban hoặc suy ra thông tin còn thiếu. Giữ nội dung gốc để đối chiếu.
- Không tự đóng ticket, nhắn cho cư dân hoặc thay đổi mức ưu tiên. Ưu tiên áp dụng theo quy định hiện có và người có trách nhiệm xác nhận.
- Trường hợp không rõ trách nhiệm, ngoài danh mục hoặc có dấu hiệu khẩn cấp đi theo quy trình chuyển cấp hiện hành; không chờ gợi ý AI để tiếp tục xử lý.
- Khi công cụ lỗi, nhân viên dùng danh mục và cách làm thủ công. Nếu chính danh mục còn mâu thuẫn, hỏi điều phối/người phụ trách để chốt đơn vị; không ép mô hình đoán.
- Chỉ dùng ticket được phép sử dụng, đã ẩn thông tin nhận diện khi đưa vào môi trường thử nghiệm. Không tải dữ liệu cư dân lên dịch vụ bên ngoài khi chưa có quyền phù hợp.

## 3. Bảng before/after

| Chỉ số | Trước, theo bài Trí | Sau, mục tiêu đề xuất | Cách kiểm tra |
|---|---|---|---|
| Số bước chính | 5 | 4 với ticket thông thường | Đếm cùng phạm vi từ mở đến chuyển ticket |
| Tổng thời gian thao tác | 4.5 phút/ticket, cần xác nhận | Dưới 1.5 phút; ngân sách thử 1.4 phút | Đo từ mở đến chuyển, tách khoảng chờ; tính cả sửa gợi ý |
| Bước cần nhân viên thao tác | Cả 5 bước | 1 bước duyệt chính; ca ngoại lệ có thể cần thêm thao tác | Quan sát thực tế, không coi số bước giảm là bằng chứng tiết kiệm thời gian |
| Tỷ lệ chuyển sai lần đầu | Khoảng 12%, chỉ là ước tính | Dưới 3%, cần nhóm xác nhận ngưỡng | Dùng đơn vị đúng do người phụ trách xác nhận |
| Bước nghẽn | Đọc/xem ảnh, có thể kèm tra cứu trách nhiệm | Có thể chuyển sang bước duyệt/sửa gợi ý | Bấm giờ riêng từng khâu |
| Ticket thiếu thông tin/chưa rõ đơn vị | Chưa có thống kê cùng phạm vi | Báo số lượng và thời gian riêng | Không bỏ các ca khó khỏi báo cáo tổng |
| Rủi ro mới | Phân loại thủ công có thể chậm hoặc sai | Tin gợi ý quá mức, Rule xung đột, danh mục lỗi thời, thêm thời gian sửa | So đối chứng, kiểm log và cho phép quay về thủ công |

Không chuyển các mục tiêu ở cột “Sau” thành số liệu đạt được trước khi pilot có kết quả. Chưa có cơ sở tính mức giảm chi phí hoặc quy đổi số giờ tiết kiệm cho cả ca.

## 4. Problem Statement v0

| Trường | Nội dung |
|---|---|
| **Actor** | Nhân viên tiếp nhận và điều phối phản ánh cư dân, chịu trách nhiệm xác định loại sự cố và chuyển tới bộ phận phù hợp |
| **Quy trình** | Tiếp nhận ticket → đọc mô tả/ảnh → tra nhóm sự cố và trách nhiệm phòng ban → gán nhãn/đơn vị → lưu và chuyển |
| **Bottleneck** | Theo bài Trí, đọc mô tả/ảnh mất 2 phút trong tổng 4.5 phút/ticket. Chưa rõ bao nhiêu thời gian do đọc hiểu, thiếu dữ liệu hay danh mục trách nhiệm chồng chéo |
| **Impact** | Tiếp nhận lâu làm tăng thời gian trước khi phản ánh tới đúng người xử lý; chuyển sai có thể gây chuyển lại và chậm xử lý. Quy mô tác động cần xác nhận bằng ticket thực tế |
| **Success Metric** | Baseline thời gian được báo cáo: 4.5 phút/ticket, cần xác minh; target dưới 1.5 phút. Tỷ lệ chuyển sai hiện tại chưa xác nhận (12% là ước tính), target đề xuất dưới 3%. Đo trên ticket trong phạm vi đã khóa, gồm thời gian kiểm tra/sửa; báo riêng thời gian chờ, ca ngoại lệ và số mẫu |
| **Boundary** | Chỉ nghiên cứu bước tiếp nhận–phân loại–chuyển giao, chưa gồm xử lý/đóng sự cố. Chưa có quyền tự động chuyển hoặc gửi phản hồi trong pilot; con người xác nhận đơn vị và ưu tiên. Nếu thử AI, chỉ được gợi ý trong danh mục, không tự thêm thông tin hoặc quyết định ngoài phạm vi |

Problem Statement mô tả khó khăn và kết quả cần đạt; chưa quy định phải dùng mô hình phân loại. Quy trình tương lai ở mục 2 chỉ là một phương án để kiểm tra, có thể đổi nếu CP4 cho thấy nguyên nhân khác.

### Cách đo cần thống nhất trước pilot

1. Chốt tập ticket được phép dùng, thời gian lấy mẫu, nhóm sự cố và phiên bản danh mục. Người có trách nhiệm nghiệp vụ xác nhận nhãn đúng; ca chưa thống nhất nhãn phải được ghi riêng.
2. Ghi thời gian mở, đọc/tra cứu, duyệt/sửa và chuyển ticket. Báo thời gian thao tác trung bình theo ticket, phân bố thời gian và số mẫu; báo thời gian chờ riêng.
3. Tỷ lệ chuyển sai lần đầu = số ticket chuyển sai / số ticket xác nhận được đơn vị đúng. Phân biệt chuyển sai với chuyển nhiều cấp hợp lệ; báo tỷ lệ chưa xác định được nhãn.
4. So quy trình hiện tại với biểu mẫu/danh mục/Rule trước. Nếu thử AI, dùng điều kiện tương đương và tính cả công sửa. Tránh cho một người xử lý lại cùng ticket mà không kiểm soát hiệu ứng nhớ nội dung.
5. Báo cả tỷ lệ ticket xử lý theo luồng thường và ngoại lệ. Số mẫu tối thiểu, thời gian thử và người chốt kết quả cần nhóm xác nhận trước khi chạy; chưa kết luận đạt khi các điều kiện này còn thiếu.

## 5. Phản biện Problem Statement v0

Các câu hỏi dưới đây do trợ lý đặt khi soạn dự thảo; nhóm chưa xác nhận câu trả lời hoặc mức đồng ý.

| Điểm còn yếu | Câu hỏi cần trả lời | Nội dung đã làm rõ trong bản nháp |
|---|---|---|
| Baseline chưa kiểm tra được | 4.5 phút đo trên bao nhiêu ticket, bởi mấy người, có tính thời gian chờ không? | Ghi rõ số kế thừa, chưa xác nhận; không dùng làm bằng chứng cải thiện đã đạt |
| Chưa rõ nguyên nhân gốc | Nhân viên đọc lâu hay phân vân giữa các phòng ban? | Tách bước đọc và tra trách nhiệm; ưu tiên chuẩn hóa danh mục trước |
| Mục tiêu dễ bị đạt giả | Các ca khó, thiếu thông tin hoặc phải sửa gợi ý có bị bỏ ra không? | Yêu cầu báo ngoại lệ và tính thời gian sửa; không loại ca khó âm thầm |
| Chưa cần đến AI | Biểu mẫu, danh mục và Rule giải quyết được phần nào? | Giữ phương án không AI làm đối chứng; AI là nhánh thử tùy kết quả |
| Giảm số bước chưa chứng minh nhanh hơn | Bước review mới có mất nhiều thời gian hơn dự kiến không? | Giữ 1.4 phút là ngân sách mục tiêu, cần đo thực tế |

## 6. Việc cần hoàn tất trước CP6

- [ ] Hoàn thành các kiểm chứng còn thiếu của CP4 và cập nhật baseline.
- [ ] Nhóm kiểm tra từng bước hiện tại với người làm thật; xác nhận actor, input, output và thời gian.
- [ ] Chốt phạm vi, danh mục, nhãn, số mẫu, người duyệt và cách xử lý ca ngoại lệ.
- [ ] Nhóm tự rà soát Problem Statement v0, ghi phản biện đồng ý/không đồng ý và sửa gì.
- [ ] Sang CP6 mới so sánh đủ No AI / Rule / Workflow / Agent, chốt mức can thiệp, viết v1 và quyết định.

## 7. Tài liệu tham khảo

- Bài `2A202603379_HoangNgocMinhTri.md` do học viên cung cấp, Card 1 và phần phản biện; chưa sao chép bản nguồn vào repo.
- [CP3 — Hội tụ](../team/cp3-hoi-tu-nhom.md), [CP4 — Kiểm chứng và research](../team/cp4-kiem-chung-research.md).
- [Worksheet](../../docs/01-worksheet.md), [bài mẫu](../../docs/02-deliverable-example.md).
