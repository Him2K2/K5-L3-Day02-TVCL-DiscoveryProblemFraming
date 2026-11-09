# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:TVCL
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch


|  # | Người đưa ra     | Candidate (Job Story ngắn)                                            | Actor                                                                   | Bottleneck                                                                                                                          | Câu hỏi phản biện nhận được (ai hỏi)                                                                                                                                                                                                                      |
| -: | -------------------- | ---------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
|  1 | Nguyễn Thanh Liêm  | Phân loại và điều phối sự cố từ nhóm chat các cơ sở       | giáo viên                                                             | sai sót và tìm kiếm lâu tin nhắn trong group                                                                                  | vũ hỏi rằng để ai đọc vào tin nhắn chat thì giải quyết vấn đề bảo mật thông tin, và quản lý thông tin nhảy cảm như thế nào khi ai đọc chat                                                                                            |
|  2 | Nguyễn Thanh Liêm  | phân loại chuyển ca dạy cho giáo viên khác khi có sự cố      | giáo viên                                                             | dò thủ công lịch học, gọi để xác nhận                                                                                     | vũ hỏi về vấn đề sự đồng ý của giáo viên khi được ai giao ca nếu không có cuộc gọi và thỏa thuận thực tế từ giáo viên đó, nếu như giáo viên đó chưa chuẩn bị cho buổi dạy đột xuất về tài liệu và kịch bản dạy |
|  3 | Nguyễn thanh Liêm  | Khi trạm sạc công cộng kín chỗ vào giờ cao điểm              | tài xế xe                                                             | di chuyển kiểm chứng từng trụ sạc                                                                                             | vũ hỏi liệu khách hàng có đồng ý với việc thêm các thiết bị như camera và loa thông báo cho các trụ sạc hay không nó sẽ rất tốn kém                                                                                                    |
|  4 | Nguyễn Thế Cường | Khi đánh giá video camera trước, tôi muốn biết kết quả biển | Kỹ sư phát triển và kiểm thử CV                                  | Bước nhận diện/hậu xử lý có thể sai; khâu gây trễ chưa đo, chưa kết luận                                           | Liêm hỏi trong tình trạng ban đêm thì camera có thể nhận dạng tốt hình ảnh. và thực sự rằng so với mắt thường thì ai phát hiện và phản hồi nhanh hơn con người không                                                               |
|  5 | Cường              | Đối chiếu hóa đơn sạc                                           | Nhân viên đối soát                                                 | Ghép và kiểm lệch, chưa đo phút/lô                                                                                          | liêm hỏi có thực sự tạo ra thêm doanh thu khi triển khai                                                                                                                                                                                                   |
|  6 | Cường              | Phân loại mô tả lỗi xe                                            | Nhân viên hỗ trợ kỹ thuật                                         | Đọc và phân loại triệu chứng; chưa đo giây/phiếu                                                                         | liêm khi các triệu chứng của nó có thể dẫn đến từ nhiều lỗi thì tiêu chí ưu tiên để chọn nơi chuyển phiếu ưu tiên là gì?                                                                                                              |
|  7 | Hồ Xuân Vũ        | Google Maps sai đường                                               | Người tham gia giao thông                                            | việc phải dừng xe hỏi người dân hoặc dò dẫm thực tế mất 5–7 phút giữa lòng đường, gây ùn tắc và nguy hiểm. | cường hỏi phương thức triển khai phương án như thế nào                                                                                                                                                                                                |
|  8 | Hồ Xuân Vũ        | chấm công bằng vân tay                                             | nhân viên, sếp                                                       | Khâu xếp hàng chờ đợi và chạm tay vào thiết bị chung gây chậm trễ và nguy cơ lây bệnh.                            | doanh nghiệp có thực sự muốn triển khai, trong khi hình thức cũ đã đáp ứng được nhiệm vụ điểm danh cho doanh nghiệp. mà phải bỏ đi để thay bằng camera thông minh                                                                    |
|  9 | Hồ Xuân Vũ        | thủ tục hành cho cựu sinh viên, sinh viên                        | sinh viên, cửu sinh viên                                             | lục lỏi các hồ sơ cũ, đối chiếu dữ liệu thủ công để xác thực và tạo phiếu yêu cầu                             | cường hỏi với tệp người dùng ít, và khách hàng ít thì nó thực sự khả thi trong thực tế                                                                                                                                                         |
| 10 | trí                 | Phân loại & Định tuyến ticket (Lăng kính: Lặp lại)            | Nhân viên tiếp nhận / Điều phối viên tổng đài CSKH           | đọc nội dung xem hình ảnh đính kèm để tạo ticket. chuyển sai ticket cho bên không có trách nhiệm                   | có thực sự phải tạo nhiều ticket đến nổi phải dùng đến ai                                                                                                                                                                                             |
| 11 | trí                 | Xác định thông tin thiếu sót                                     | Nhân viên CSKH / Kỹ thuật viên tiếp nhận                         | phải kiểm tra lại sự đầy đủ của thông tin                                                                                 | trường hợp này cũng ít khi xảy ra có thực sự cần giải quyết như vậy                                                                                                                                                                                 |
| 12 | trí                 | Bàn giao bối cảnh xử lý                                           | Điều phối viên ca trước & Kỹ thuật viên hiện trường ca sau. | Đọc lại toàn bộ lịch sử & log trao đổi                                                                                     | thực tế khi giao ca thì công việc chưa làm xong phải thực hiện cho xong hay lại phải làm cho xong mới đổi?                                                                                                                                         |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A | | |
| B | | |
| C | | |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: 
├── Opportunity A: 
├── Opportunity B: 
└── Opportunity C: 
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

-

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |

**Candidate được chọn:**

**Vì sao chọn:**

**Vì sao loại các candidate còn lại:**

**Xử lý bất đồng (nếu có):**

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
