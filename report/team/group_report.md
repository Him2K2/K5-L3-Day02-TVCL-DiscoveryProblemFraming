# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: TVCL
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Phân loại và định tuyến thông minh phản ánh của cư dân đến đúng bộ phận chuyên trách trên ứng dụng Vinhomes Resident.
- Quyết định cuối: Not Yet (Chi tiết tại Mục 8)

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
| 10 | Minh Trí                 | Phân loại & Định tuyến ticket (Lăng kính: Lặp lại)            | Nhân viên tiếp nhận / Điều phối viên tổng đài CSKH           | đọc nội dung xem hình ảnh đính kèm để tạo ticket. chuyển sai ticket cho bên không có trách nhiệm                   | có thực sự phải tạo nhiều ticket đến nổi phải dùng đến ai                                                                                                                                                                                             |
| 11 | Minh Trí                 | Xác định thông tin thiếu sót                                     | Nhân viên CSKH / Kỹ thuật viên tiếp nhận                         | phải kiểm tra lại sự đầy đủ của thông tin                                                                                 | trường hợp này cũng ít khi xảy ra có thực sự cần giải quyết như vậy                                                                                                                                                                                 |
| 12 | Minh Trí                 | Bàn giao bối cảnh xử lý                                           | Điều phối viên ca trước & Kỹ thuật viên hiện trường ca sau. | Đọc lại toàn bộ lịch sử & log trao đổi                                                                                     | thực tế khi giao ca thì công việc chưa làm xong phải thực hiện cho xong hay lại phải làm cho xong mới đổi?                                                                                                                                         |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| **A — Phân loại & Định tuyến yêu cầu/sự cố (Triage & Routing)** | Candidate #1 (Liêm), #4 (Trí), #5 (Trí), #6 (Trí), #9 (Cường) | Gom thông tin văn bản/hình ảnh phản ánh từ người dùng (ngôn ngữ tự nhiên, không cấu trúc), đọc hiểu nội dung, phân loại mức độ khẩn cấp và định tuyến chính xác đến đúng bộ phận chuyên trách để xử lý. |
| **B — Giao thông, Định vị & Thị giác máy tính (Mobility & Vision)** | Candidate #3 (Liêm), #7 (Cường), #11 (Vũ) | Thu thập và xử lý tín hiệu không gian/hình ảnh thực tế (camera, bản đồ, trạng thái trụ sạc) để cảnh báo sai lệch hoặc tối ưu di chuyển. |
| **C — Thủ tục hành chính & Vận hành nội bộ (Operations & Admin)** | Candidate #2 (Liêm), #8 (Cường), #10 (Vũ), #12 (Vũ) | Đối soát dữ liệu bảng tính, lịch trình, đối chiếu quy định thủ tục giấy tờ và quy trình vận hành giữa các bộ phận. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```
OUTCOME: Giảm thời gian phản hồi và tỷ lệ chuyển sai bộ phận khi xử lý phản ánh của cư dân Vinhomes
├── Opportunity A: Cư dân mô tả bằng câu chữ tự do, không theo cấu trúc, thiếu thông tin số phòng/vị trí cụ thể
├── Opportunity B: Danh mục phân loại phòng ban nội bộ bị chồng chéo (Kỹ thuật điện/nước vs Bảo trì tòa nhà)
└── Opportunity C: Điều phối viên đọc thủ công từng ticket, mở ảnh đối chiếu và chuyển tiếp bằng tay tạo điểm nghẽn
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- ✗ **"Chatbot AI tự động trả lời cư dân"**  
  → Đây là Solution (công cụ AI), không phải nhu cầu hay nỗi đau (User Need / Pain Point) của người dùng.

- ✗ **"Bắt buộc cư dân tự chọn phòng ban qua cây thư mục (dropdown) trên App"**  
  → Đây là Solution (thay đổi giao diện ứng dụng), thậm chí còn làm tăng gánh nặng cho cư dân vì họ không nắm rõ cơ cấu tổ chức và chức năng của từng phòng ban trong ban quản lý.

- ✗ **"Hệ thống tự động giao việc trực tiếp cho kỹ thuật viên mà không cần người duyệt"**  
  → Đây là Solution (tính năng tự động hóa), vi phạm ranh giới an toàn vận hành (Human-in-the-Loop), khi loại bỏ bước kiểm duyệt và phê duyệt của con người.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **#4. Phân loại phản ánh cư dân Vinhomes (Trí)** | 5 | 5 | 5 | 5 | 5 | 5 | 5 | **35** |
| **#1. Phân loại sự cố chat các cơ sở (Liêm)** | 5 | 5 | 5 | 5 | 5 | 5 | 4 | **34** |
| **#10. Thủ tục hành chính sinh viên (Vũ)** | 4 | 4 | 3 | 3 | 4 | 3 | 4 | **25** |
| **#7. Nhận diện biển báo xe tự hành CV (Cường)** | 2 | 3 | 2 | 2 | 1 | 2 | 2 | **14** |

**Candidate được chọn:**  
**Candidate #4: Phân loại và định tuyến phản ánh của cư dân đến đúng bộ phận chuyên trách trên ứng dụng Vinhomes Resident** (kết hợp các bài học về xử lý tin nhắn/sự cố từ Candidate #1 của Liêm).

**Vì sao chọn:**  
1. Đạt điểm tuyệt đối (35/35), đáp ứng hoàn hảo cả 7 tiêu chí đánh giá của lab.  
2. Nỗi đau có thật với tần suất rất lớn (khoảng 120 ticket/ca trực 8 tiếng tại các khu đô thị lớn như Vinhomes Smart City/Ocean Park).  
3. Các chỉ số đo lường rất cụ thể: thời gian đọc/xử lý giảm từ 4.5 phút xuống < 1 phút/ticket; tỷ lệ gán nhầm phòng ban giảm từ 12% xuống < 3%.  
4. Có tính khả thi cao nhất để kiểm chứng ở CP4: nhóm có thể phỏng vấn ngay các bạn học trong lớp đang sinh sống tại các khu chung cư Vinhomes.  
5. Khung bài toán rất mẫu mực để so sánh sâu sắc giữa giải pháp No AI (chuẩn hóa danh mục phòng ban) vs Rule (bắt từ khóa) vs Workflow AI (trợ lý gợi ý phân loại có con người kiểm duyệt).

**Vì sao loại các candidate còn lại:**  
- **Loại Candidate #7 (Nhận diện biển báo của Cường):** Đây là bài toán thuần về tối ưu thuật toán Computer Vision, không phải bài toán tái định hình quy trình vận hành người dùng (Discovery & Problem Framing). Dữ liệu video xe tự hành là tài sản bảo mật nội bộ của VinFast, nhóm không thể tiếp cận dữ liệu thật hay chuyên gia thật để phỏng vấn ở CP4.  
- **Loại Candidate #10 (Thủ tục hành chính sinh viên của Vũ):** Tần suất phát sinh của cựu sinh viên rất thấp (1–2 lần/năm). Nút thắt lớn nhất khiến thủ tục kéo dài 2–3 ngày nằm ở quy chế hành chính bắt buộc phải có chữ ký tươi và con dấu đỏ của trường đại học, AI không thể tự động hóa khâu ký duyệt pháp lý này (Rủi ro Viability cao).  
- **Hội tụ Candidate #1 (Sự cố cơ sở của Liêm) vào Candidate #4:** Candidate #1 có cùng pattern *Ticket Triage & Routing* với Candidate #4, nhưng bối cảnh App Vinhomes Resident của Candidate #4 có quy mô số lượng ticket lớn hơn, quy trình chuẩn mực hơn và thuận tiện phỏng vấn người dùng thật hơn.

**Xử lý bất đồng:**  
Ban đầu Cường muốn chọn bài nhận diện biển báo xe vì đúng chuyên môn Computer Vision. Nhóm đã cùng phân tích rubric yêu cầu phỏng vấn người thật (The Mom Test) ở CP4 và so sánh 4 mức can thiệp ở CP6; Cường đã đồng ý rằng bài toán xe tự hành không khả thi để kiểm chứng trong thời gian 4 tiếng của lab và hoàn toàn đồng thuận chọn bài toán phản ánh cư dân của Trí.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Cư dân thường xuyên gặp tình trạng phản ánh gửi qua App bị chậm trễ (trên 2 tiếng) hoặc bị chuyển sai bộ phận kỹ thuật, khiến họ phải nhắc lại nội dung nhiều lần. | Value | 5 | 2 | **Có** |
| 2 | Điều phối viên Ban quản lý muốn hệ thống AI gợi ý phòng ban và mức độ khẩn cấp để họ bấm duyệt (Human-in-the-loop), chứ không muốn AI tự động giao việc trực tiếp cho kỹ thuật viên. | Usability | 5 | 2 | **Có** |
| 3 | Mô tả văn bản ngắn (kể cả viết tắt, tiếng lóng) kèm hình ảnh chụp sự cố của cư dân chứa đủ ngữ cảnh để mô hình AI phân loại chính xác vào đúng nhóm chuyên trách (Điện nước, Vệ sinh, An ninh, Bảo trì). | Feasibility | 4 | 3 | Không |
| 4 | Việc bắt buộc cư dân tự chọn phòng ban qua menu thả xuống (dropdown) trên App sẽ khiến cư dân chọn bừa hoặc gây ức chế, vì cư dân không hiểu cơ cấu tổ chức nội bộ của ban quản lý. | Value / Usability | 5 | 2 | **Có** |
| 5 | Ban quản lý chấp nhận tích hợp công cụ AI phân loại vào phần mềm vận hành nếu hệ thống bảo đảm che mờ thông tin cá nhân (PII: số điện thoại, số căn hộ) trước khi xử lý. | Viability | 4 | 3 | Không |

*Điền 5 giả định; ưu tiên kiểm chứng các ô Quan trọng cao (4–5) nhưng Bằng chứng còn thấp (1–2).*

**Giả định nhóm kiểm chứng trong buổi này:**
- **Giả định #1 (Value):** Kiểm chứng hành vi thật của cư dân: họ đã từng bị phản hồi chậm, chuyển nhầm người hoặc phải giải thích lại sự cố bao giờ chưa, mất bao lâu?
- **Giả định #4 (Usability / Non-AI):** Kiểm chứng xem khi gửi phản ánh, cư dân muốn gõ tự do/chụp ảnh gửi nhanh hay sẵn sàng tự phân loại qua cây danh mục phức tạp?

### 3.2. Kiểm chứng

**Cách đã dùng:** Rà soát và phân tích các bài đánh giá (Reviews & Customer Feedback) công khai của cư dân trên Google Play Store và Apple App Store cho ứng dụng Vinhomes Resident.

#### Review Snapshot #1 — Vấn đề đồng bộ và xử lý dịch vụ kéo dài

| Trường | Nội dung |
|---|---|
| **Người được hỏi (vai trò, nguồn)** | Cư dân tòa BE4, khu đô thị Vinhomes (Đánh giá Google Play · Hoa Như · 25/08/2026) |
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Quy trình đồng bộ App mất nhiều thời gian 1 tuần trời ko làm nổi thẻ ra vào và thẻ gửi xe. Mỗi tối mất 32k tiền gửi xe. Dịch vụ quá tệ tòa Be4"* |
| **Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra?** | Cư dân đăng ký làm thẻ gửi xe và thẻ ra vào qua app, nhưng hệ thống xử lý kéo dài cả tuần không xong, không có bộ phận nào phản hồi nguyên nhân. |
| **Hiện đang xử lý bằng cách nào (workaround)?** | Chấp nhận gửi xe trả phí vé lượt bên ngoài (mất 32k/tối) trong thời gian chờ đợi ban quản lý xử lý. |
| **Mất bao lâu, bao lần?** | Kéo dài 1 tuần lễ; phát sinh chi phí thiệt hại tài chính thực tế mỗi ngày. |
| **Insight / opportunity rút ra** | Độ trễ xử lý các yêu cầu dịch vụ của cư dân gây thiệt hại kinh tế và bức xúc thật. Các yêu cầu về thẻ/tiện ích bị tắc nghẽn ở khâu đối soát và chuyển tiếp giữa BQL và bộ phận vận hành bãi đỗ xe. |

#### Review Snapshot #2 — Ý kiến gửi qua app không được phản hồi & Kênh hotline thay thế

| Trường | Nội dung |
|---|---|
| **Người được hỏi (vai trò, nguồn)** | Cư dân căn hộ Vinhomes (Đánh giá App Store · Ethanvo & Thu Huyen Nguyen trên Google Play) |
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"App vô nghĩa vì ý kiến cư dân cũng k được giải quyết, cđt nên xóa app"* và *"App luôn liên tục bị lỗi và không có cách nào liên hệ hỗ trợ từ app."* |
| **Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra?** | Gửi phản ánh/góp ý qua ứng dụng nhưng không nhận được giải quyết hoặc trạng thái xử lý; không tìm thấy đầu mối liên hệ hỗ trợ trực tiếp trên giao diện ticket. |
| **Hiện đang xử lý bằng cách nào (workaround)?** | Nhà phát triển hướng dẫn cư dân chuyển sang gọi Tổng đài Chăm sóc Khách hàng 1900 2323 89 (nhánh 4) để gửi ảnh và mô tả sự việc. |
| **Mất bao lâu, bao lần?** | Tình trạng lặp lại qua nhiều phiên bản cập nhật; cư dân phải thoát app hoặc gọi điện thoại ngoài ứng dụng. |
| **Insight / opportunity rút ra** | Cư dân mất niềm tin vào nút gửi phản ánh trên app vì không thấy trạng thái định tuyến minh bạch. Khi app không phản hồi kịp, cư dân buộc phải chuyển kênh sang hotline thoại làm tăng tải cho tổng đài viên. |

#### Bảng tổng hợp kiểm chứng qua Review:

| Nguồn | Số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| **Google Play (Vinhomes Resident)** | 2 review tiêu biểu (Hoa Như, Thu Huyen Nguyen) | Cư dân bức xúc vì ý kiến gửi qua app bị chậm trễ hoặc không được giải quyết; phát sinh chi phí thật (32k/tối) do quy trình kéo dài cả tuần. | Review không chỉ nói về hỏng hóc kỹ thuật trong nhà (điện nước) mà phản ánh rất nhiều về **dịch vụ thẻ/đỗ xe** và thủ tục hành chính. |
| **Apple App Store (Vinhomes Resident)** | 2 review tiêu biểu (Viet Ne 217, Ethanvo) | Các lỗi dịch vụ (như đăng ký khuôn mặt/intercom cho khách) bị kéo dài "mãi không khắc phục"; người dùng lúng túng khi không biết kênh nào đang tiếp nhận. | **Tín hiệu phản bác quan trọng:** Ban quản lý có kênh Hotline hỗ trợ trực tiếp (1900 2323 89 nhánh 4) song song; nhiều trường hợp cư dân được điều hướng gọi tổng đài thay vì xử lý hoàn toàn trên app. |

*Ảnh chụp minh chứng đánh giá thực tế của cư dân từ Google Play Store và Apple App Store:*
![Đánh giá cư dân trên Google Play](../assets/review_cu_dan.png)
![Đánh giá cư dân trên App Store](../assets/review_cu_dan_2.png)

**Nhóm đã sửa problem thế nào sau kiểm chứng:**  
1. **Mở rộng phạm vi phân loại (Category Scope):** Ban đầu nhóm chỉ dự định phân loại các sự cố hỏng hóc kỹ thuật (điện, nước, điều hòa). Sau khi đọc review thực tế, nhóm nhận thấy nhu cầu phản ánh của cư dân phân bổ rất nhiều vào mảng **Dịch vụ cư dân & Tiện ích số (thẻ xe, thẻ ra vào, intercom, rác thải)**. Do đó, nhóm bổ sung danh mục định tuyến bao gồm cả 4 mảng nghiệp vụ cốt lõi của ban quản lý.  
2. **Xác lập Ranh giới (Boundary) & Kênh khẩn cấp:** Từ phản hồi của nhà phát triển về việc gọi Hotline 1900 2323 89 (nhánh 4), nhóm xác định rõ: **Hệ thống AI chỉ đóng vai trò phân loại và định tuyến các phản ánh phi khẩn cấp trên App**. Nếu phát hiện sự cố khẩn cấp hoặc lỗi hệ thống nghiêm trọng, giao diện sẽ kích hoạt nút gọi ngay đến Hotline tổng đài thay vì để ticket rơi vào hàng đợi xử lý.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
|Công cụ 1: Zendesk Support | [https://www.zendesk.com/service/help-center/ticketing-system/](https://www.zendesk.com/service/help-center/ticketing-system/) |Tự động định tuyến ticket và gắn nhãn ưu tiên dựa trên từ khóa. | Hệ thống quy tắc (triggers/automations) cực kỳ mạnh mẽ, tích hợp sẵn AI gợi ý câu trả lời.|Chi phí bản quyền cao, cấu hình phức tạp và không tối ưu sẵn cho đặc thù văn hóa/ngôn ngữ tiếng Việt lóng/viết tắt của cư dân chung cư. |Không nên xây dựng hệ thống rule quá cứng nhắc mà cần kết hợp lớp AI linh hoạt để hiểu ngữ cảnh tiếng Việt tự nhiên. |
|Freshdesk |[https://www.freshworks.com/freshdesk/](https://www.freshworks.com/freshdesk/) |Phân loại tự động | Giao diện trực quan, tính năng "Freddy AI" hỗ trợ gợi ý phân loại ticket khá tốt.|Khó tùy biến sâu theo luồng phê duyệt đặc thù (Human-in-the-loop nhiều cấp) của Ban quản lý Vinhomes |

---

## 4. Quy trình trước/sau (CP5)

**Người tổng hợp:** Nguyễn Thế Cường — 2A202603355, nhóm TVCL.

**Nguồn tổng hợp:** Nguyễn Thế Cường cung cấp, kế thừa mô tả và số liệu từ bài Hoàng Ngọc Minh Trí.

### 4.1. Quy trình hiện tại

Khi nhận phản ánh, nhân viên phải đọc nội dung, xem ảnh và tra đơn vị phụ trách rồi mới chuyển ticket. Nếu mô tả khó hiểu hoặc trách nhiệm phòng ban chưa rõ, nhân viên có thể phải hỏi thêm trước khi chuyển.

```
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

### 4.2. Quy trình tương lai đề xuất

Trước tiên cần thống nhất danh mục sự cố và đơn vị phụ trách. Sau đó thử biểu mẫu và Rule làm đối chứng. Chỉ thử hỗ trợ phân loại nội dung nếu cách đơn giản vẫn còn nhiều trường hợp khó; chưa chốt mức can thiệp AI ở CP5.

#### Các bước và vai trò

| Bước | Actor | Input | Output | Ngân sách thời gian đề xuất |
|---:|---|---|---|---|
| 1. Mở và kiểm tra dữ liệu | Rule | Ticket, trường bắt buộc theo loại phản ánh | Đủ dữ liệu hoặc danh sách trường thiếu | 0.1 phút |
| 2. Chuẩn bị phương án phân loại | Rule; AI chỉ thử nếu cần | Ticket đủ dữ liệu và danh mục đã khóa | Nhóm sự cố, đơn vị gợi ý và căn cứ; có thể trả “chưa xác định” | 0.2 phút |
| 3. Kiểm tra và quyết định | Nhân viên CSKH | Nội dung gốc và gợi ý | Phân loại được duyệt/sửa hoặc chuyển xử lý thủ công | 0.8 phút |
| 4. Lưu và chuyển sau duyệt | Rule thực hiện theo xác nhận của nhân viên | Ticket đã được duyệt | Ticket chuyển đúng đơn vị; có log thao tác và người duyệt | 0.3 phút |

Tổng ngân sách mục tiêu: **1.4 phút/ticket đủ thông tin, thuộc danh mục đã thống nhất**. Đây là cách phân bổ mục tiêu để thử, không phải kết quả đo. Thời gian nhân viên phát hiện và sửa gợi ý phải nằm trong phép đo. Ticket thiếu thông tin hoặc chưa rõ đơn vị đi theo nhánh riêng và vẫn phải được báo cáo, không loại âm thầm để làm đẹp chỉ số.

```
TƯƠNG LAI — mục tiêu 1.4 phút/ticket thông thường, chưa thử nghiệm

[1 Kiểm tra trường dữ liệu: 0.1']                          ← RULE
→ [2 Chuẩn bị nhóm sự cố và đơn vị gợi ý: 0.2']             ← RULE / AI NẾU CẦN THỬ
→ [3 Nhân viên xem nội dung gốc, duyệt hoặc sửa: 0.8']      ← CON NGƯỜI
→ [4 Lưu và chuyển theo xác nhận: 0.3']                    ← RULE

Thiếu thông tin → Nhân viên yêu cầu bổ sung; ghi riêng thời gian chờ.
Không rõ đơn vị / gợi ý không phù hợp → Nhân viên phân loại thủ công hoặc hỏi điều phối.
Rule/AI lỗi → Dùng danh mục và quy trình thủ công hiện tại; lưu lý do quay về.
```

#### Ranh giới và phương án quay về

- Nhân viên phải kiểm tra và xác nhận trước khi chuyển ticket trong pilot. AI, nếu được thử, chỉ gợi ý nhãn/đơn vị từ danh mục đã duyệt.
- Không tự tạo dữ kiện, sửa mô tả gốc, tự thêm phòng ban hoặc suy ra thông tin còn thiếu. Giữ nội dung gốc để đối chiếu.
- Không tự đóng ticket, nhắn cho cư dân hoặc thay đổi mức ưu tiên. Ưu tiên áp dụng theo quy định hiện có và người có trách nhiệm xác nhận.
- Trường hợp không rõ trách nhiệm, ngoài danh mục hoặc có dấu hiệu khẩn cấp đi theo quy trình chuyển cấp hiện hành; không chờ gợi ý AI để tiếp tục xử lý.
- Khi công cụ lỗi, nhân viên dùng danh mục và cách làm thủ công. Nếu chính danh mục còn mâu thuẫn, hỏi điều phối/người phụ trách để chốt đơn vị; không ép mô hình đoán.
- Chỉ dùng ticket được phép sử dụng, đã ẩn thông tin nhận diện khi đưa vào môi trường thử nghiệm. Không tải dữ liệu cư dân lên dịch vụ bên ngoài khi chưa có quyền phù hợp.

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---|---|---|
| Số bước chính | 5 | 4 với ticket thông thường | Đếm cùng phạm vi từ mở đến chuyển ticket |
| Tổng thời gian thao tác | 4.5 phút/ticket, cần xác nhận | Dưới 1.5 phút; ngân sách thử 1.4 phút | Đo từ mở đến chuyển, tách khoảng chờ; tính cả sửa gợi ý |
| Bước cần nhân viên thao tác | Cả 5 bước | 1 bước duyệt chính; ca ngoại lệ có thể cần thêm thao tác | Quan sát thực tế, không coi số bước giảm là bằng chứng tiết kiệm thời gian |
| Tỷ lệ chuyển sai lần đầu | Khoảng 12%, chỉ là ước tính | Dưới 3%, cần nhóm xác nhận ngưỡng | Dùng đơn vị đúng do người phụ trách xác nhận |
| Bước nghẽn | Đọc/xem ảnh, có thể kèm tra cứu trách nhiệm | Có thể chuyển sang bước duyệt/sửa gợi ý | Bấm giờ riêng từng khâu |
| Ticket thiếu thông tin/chưa rõ đơn vị | Chưa có thống kê cùng phạm vi | Báo số lượng và thời gian riêng | Không bỏ các ca khó khỏi báo cáo tổng |
| Rủi ro mới | Phân loại thủ công có thể chậm hoặc sai | Tin gợi ý quá mức, Rule xung đột, danh mục lỗi thời, thêm thời gian sửa | So đối chứng, kiểm log và cho phép quay về thủ công |

Không chuyển các mục tiêu ở cột “Sau” thành số liệu đạt được trước khi pilot có kết quả. Chưa có cơ sở tính mức giảm chi phí hoặc quy đổi số giờ tiết kiệm cho cả ca.

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Nhân viên tiếp nhận và điều phối phản ánh cư dân, chịu trách nhiệm xác định loại sự cố và chuyển tới bộ phận phù hợp |
| **Quy trình** | Tiếp nhận ticket → đọc mô tả/ảnh → tra nhóm sự cố và trách nhiệm phòng ban → gán nhãn/đơn vị → lưu và chuyển |
| **Bottleneck** | Theo bài Trí, đọc mô tả/ảnh mất 2 phút trong tổng 4.5 phút/ticket. Chưa rõ bao nhiêu thời gian do đọc hiểu, thiếu dữ liệu hay danh mục trách nhiệm chồng chéo |
| **Impact** | Tiếp nhận lâu làm tăng thời gian trước khi phản ánh tới đúng người xử lý; chuyển sai có thể gây chuyển lại và chậm xử lý. Quy mô tác động cần xác nhận bằng ticket thực tế |
| **Success Metric** | Baseline thời gian được báo cáo: 4.5 phút/ticket, cần xác minh; target dưới 1.5 phút. Tỷ lệ chuyển sai hiện tại chưa xác nhận (12% là ước tính), target đề xuất dưới 3%. Đo trên ticket trong phạm vi đã khóa, gồm thời gian kiểm tra/sửa; báo riêng thời gian chờ, ca ngoại lệ và số mẫu |
| **Boundary** | Chỉ nghiên cứu bước tiếp nhận–phân loại–chuyển giao, chưa gồm xử lý/đóng sự cố. Chưa có quyền tự động chuyển hoặc gửi phản hồi trong pilot; con người xác nhận đơn vị và ưu tiên. Nếu thử AI, chỉ được gợi ý trong danh mục, không tự thêm thông tin hoặc quyết định ngoài phạm vi |

Problem Statement mô tả khó khăn và kết quả cần đạt; chưa quy định phải dùng mô hình phân loại. Quy trình tương lai ở mục 4.2 chỉ là một phương án để kiểm tra, có thể đổi nếu CP4 cho thấy nguyên nhân khác.

### 5.1. Cách đo cần thống nhất trước pilot

1. Chốt tập ticket được phép dùng, thời gian lấy mẫu, nhóm sự cố và phiên bản danh mục. Người có trách nhiệm nghiệp vụ xác nhận nhãn đúng; ca chưa thống nhất nhãn phải được ghi riêng.
2. Ghi thời gian mở, đọc/tra cứu, duyệt/sửa và chuyển ticket. Báo thời gian thao tác trung bình theo ticket, phân bố thời gian và số mẫu; báo thời gian chờ riêng.
3. Tỷ lệ chuyển sai lần đầu = số ticket chuyển sai / số ticket xác nhận được đơn vị đúng. Phân biệt chuyển sai với chuyển nhiều cấp hợp lệ; báo tỷ lệ chưa xác định được nhãn.
4. So quy trình hiện tại với biểu mẫu/danh mục/Rule trước. Nếu thử AI, dùng điều kiện tương đương và tính cả công sửa. Tránh cho một người xử lý lại cùng ticket mà không kiểm soát hiệu ứng nhớ nội dung.
5. Báo cả tỷ lệ ticket xử lý theo luồng thường và ngoại lệ. Số mẫu tối thiểu, thời gian thử và người chốt kết quả cần nhóm xác nhận trước khi chạy; chưa kết luận đạt khi các điều kiện này còn thiếu.

### 5.2. Phản biện Problem Statement v0

Các câu hỏi dưới đây do trợ lý đặt khi soạn dự thảo; nhóm đã rà soát và ghi nhận ý kiến trong bảng.

| Điểm còn yếu | Câu hỏi cần trả lời | Nội dung đã làm rõ trong bản nháp | Nhóm đồng ý? |
|---|---|---|---|
| Baseline chưa kiểm tra được | 4.5 phút đo trên bao nhiêu ticket, bởi mấy người, có tính thời gian chờ không? | Ghi rõ số kế thừa, chưa xác nhận; không dùng làm bằng chứng cải thiện đã đạt | Đồng ý |
| Chưa rõ nguyên nhân gốc | Nhân viên đọc lâu hay phân vân giữa các phòng ban? | Tách bước đọc và tra trách nhiệm; ưu tiên chuẩn hóa danh mục trước | Đồng ý |
| Mục tiêu dễ bị đạt giả | Các ca khó, thiếu thông tin hoặc phải sửa gợi ý có bị bỏ ra không? | Yêu cầu báo ngoại lệ và tính thời gian sửa; không loại ca khó âm thầm | Đồng ý |
| Chưa cần đến AI | Biểu mẫu, danh mục và Rule giải quyết được phần nào? | Giữ phương án không AI làm đối chứng; AI là nhánh thử tùy kết quả | Đồng ý với việc cần kiểm tra |
| Giảm số bước chưa chứng minh nhanh hơn | Bước review mới có mất nhiều thời gian hơn dự kiến không? | Giữ 1.4 phút là ngân sách mục tiêu, cần đo thực tế | Đồng ý |


---

## 6. Mức can thiệp AI (CP6)

1. Ma trận độ mơ hồ × độ phức tạp
Vị trí bài toán: Độ mơ hồ Trung bình - Độ phức tạp Trung bình (Medium Ambiguity, Medium Complexity).

Giải thích:

Độ mơ hồ (Ambiguity): Trung bình. Văn bản mô tả sự cố từ cư dân sử dụng từ ngữ tự do, văn phong đời thường hoặc ảnh chụp không có tiêu đề, dẫn đến việc cùng một sự cố có thể viết theo nhiều cách. Tuy nhiên, kết quả đầu ra là hệ thống danh mục phòng ban (Taxonomy) lại cố định và có quy tắc rõ ràng.

Độ phức tạp (Complexity): Trung bình. Bài toán chỉ yêu cầu trích xuất ngữ cảnh/ảnh và đối chiếu với danh mục phòng ban hiện có để đưa ra nhãn đề xuất; không đòi hỏi kết nối quá nhiều nguồn dữ liệu đa bên hay chuỗi hành động kéo dài phức tạp.

2. So sánh 4 mức độ can thiệp
|Mức can thiệp| |Phương án cụ thể cho Vinhomes| |Khi nào mức này đủ đáp ứng| |Rủi ro chính| |Có được chọn không?|
|1. No AI| |Chuẩn hóa danh mục phòng ban và tập huấn cho nhân viên CSKH tra cứu thủ công.| |Cư dân luôn mô tả chuẩn xác và khối lượng ticket ít (< 20 ticket/ngày).| |Nhân viên vẫn phải đọc 100% văn bản thô, gây nghẽn nghiêm trọng vào giờ cao điểm.| |Không|
|2. Rule| |Bắt buộc cư dân tự chọn phân loại và phòng ban qua Form Dropdown trên App trước khi bấm gửi.| |Cư dân nắm rõ chuyên môn kỹ thuật và sẵn sàng dành thời gian chọn từng mục.| |Cư dân chọn bừa mục "Khác" hoặc chọn sai do không nắm rõ chuyên môn; không xử lý được ảnh chụp.| |Không|
|3. Workflow| |AI đọc mô tả text + OCR ảnh để gợi ý 1 nhãn phân loại & phòng ban, nhân viên CSKH chỉ cần nhìn gợi ý và bấm 1-click để duyệt hoặc chỉnh sửa.| |Cần xử lý nhanh dữ liệu thô nhưng bắt buộc kiểm soát rủi ro phân loại sai trước khi chuyển giao.| |AI có thể gợi ý sai nếu mô tả quá mờ nát, nhưng nhân viên sẽ phát hiện và sửa được ngay lập tức.| |CHỌN|
|4. Agent| |AI tự động chuyển thẳng ticket đến đội kỹ thuật mà không cần nhân viên CSKH kiểm duyệt.| |Mô hình đạt độ chính xác gần như tuyệt đối (> 99.5%) và bài toán không có rủi ro khẩn cấp về an toàn.| |Rủi ro tự động chuyển nhầm các ca khẩn cấp (chập điện, cháy nổ), gây nguy hiểm hoặc làm rối loạn đội kỹ thuật.| |Không|

==> Lý do chọn mức 3: Mức Rule (Mức 2) không giải quyết được các mô tả tự do và ảnh chụp của cư dân. Mức Agent (Mức 4) quá mạo hiểm vì rủi ro chuyển sai sự cố khẩn cấp. Mức Workflow là điểm cân bằng hoàn hảo: vừa giải phóng >70% thời gian đọc của nhân viên, vừa giữ sự kiểm soát an toàn của con người.

3. AI Canvas rút gọn
Prediction (Dự đoán): Gợi ý Nhóm sự cố (Kỹ thuật/Dịch vụ/An ninh) và Đơn vị phụ trách dựa trên text mô tả + OCR ảnh đính kèm.

Judgment (Đánh giá của con người): Nhân viên CSKH đối chiếu gợi ý của AI với nội dung ticket thực tế để bấm duyệt hoặc đổi nhãn nếu AI đoán sai.

Action (Hành động): Đổi trạng thái ticket và định tuyến dữ liệu đến phần mềm của phòng ban được chọn.

Outcome (Kết quả mong muốn): Rút ngắn thời gian tiếp nhận ban đầu xuống < 1.5 phút/ticket, giảm tỷ lệ phân loại sai xuống < 3%.

Input (Dữ liệu đầu vào): Đoạn văn bản mô tả của cư dân, ảnh chụp sự cố, lịch sử các ticket đã được gán nhãn chuẩn trong quá khứ.

Feedback (Phản hồi cải tiến): Mọi thao tác nhân viên bấm chỉnh sửa khi AI đoán sai sẽ được lưu lại làm log dữ liệu để re-train (huấn luyện lại) mô hình.

4. Hai câu hỏi của Google PAIR
- Người dùng cần Augmentation (Hỗ trợ) hay Automation (Tự động hóa)?

Trả lời: Cần Augmentation (Hỗ trợ). Nhân viên CSKH vẫn là người chịu trách nhiệm chính cho việc định tuyến ticket. AI chỉ đóng vai trò trợ lý đọc nhanh và đưa ra gợi ý sẵn để nhân viên giảm bớt thao tác lặp đi lặp lại.

- Loại lỗi nào tồi tệ hơn và thiết kế hệ thống phản ứng như thế nào?
1. Trả lời: Lỗi bỏ sót ca khẩn cấp / gợi ý sai phòng ban làm trễ hạn giải quyết sự cố nghiêm trọng tồi tệ hơn nhiều so với việc nhân viên phải tốn 2 giây để bấm sửa nhãn.
2. Thiết kế phản ứng:
    + AI được cài đặt bộ lọc từ khóa ưu tiên (như "cháy", "khói", "mất điện toàn bộ", "mất nước hệ thống") để luôn gắn cờ [KHẨN CẤP] lên hàng đầu.

    + Khi độ tin cậy của AI < 60%, giao diện không gợi ý ép buộc mà hiển thị cảnh báo để nhân viên tự đọc kỹ.

## Mục 7: Problem Statement v1 + Tiêu chí đánh giá (CP6)
1. Bảng Problem Statement 
+ Actor: Nhân viên điều phối / CSKH tổng đài tại khu đô thị Vinhomes.

+ Quy trình: Tiếp nhận, đọc hiểu nội dung phản ánh thô và thực hiện phân loại, định tuyến ticket cho các yêu cầu gửi về trong giờ cao điểm.

+ Bottleneck: Bước đọc mô tả dài dòng, thiếu cấu trúc và tra cứu danh mục phân loại chồng chéo tốn trung bình 2.0 phút cho mỗi ticket (chiếm >44% thời gian xử lý ban đầu).

+ Impact: Gây ùn tắc hàng đợi ticket giờ cao điểm, tăng tỷ lệ chuyển nhầm bộ phận (~12%), kéo dài thời gian chờ phản hồi của cư dân.

- Success Metric:
    + Baseline: Thời gian xử lý tiếp nhận ban đầu là 4.0 phút/ticket; Tỷ lệ chuyển sai bộ phận là 12%.

    + Target: Giảm thời gian xử lý ban đầu xuống < 1.5 phút/ticket; Giảm tỷ lệ chuyển sai bộ phận xuống < 3%.

    + Phương pháp đo: Thống kê tự động thời gian từ lúc ticket tạo đến khi nhân viên bấm xác nhận chuyển giao trên log phần mềm ca trực.

+ Boundary: AI chỉ được gợi ý, không được tự động định tuyến các ca khẩn cấp hoặc tự ý đóng ticket mà không qua sự xác nhận của nhân viên.

+ AI Intervention Point: Bước 2 của quy trình (Đọc nội dung, OCR ảnh và gợi ý 1-click nhãn phân loại).

+ Mức chọn: Workflow.

+ Rủi ro & Người kiểm tra: Rủi ro AI đoán sai do mô tả viết tắt/ảnh mờ -> Người kiểm tra: Nhân viên điều phối ca trực xem xét và bấm duyệt cuối cùng.

2. Điểm thay đổi so với v0 và Lý do
 + Thay đổi: Bổ sung rõ giới hạn cứng (Boundary) về việc cấm AI tự động định tuyến các ticket có từ khóa nguy cơ khẩn cấp và làm rõ cơ chế Fallback (chuyển về thủ công khi AI tin cậy thấp < 60%).

 + Lý do: Dựa trên kết quả phỏng vấn kiểm chứng ở CP4 và phân tích rủi ro PAIR ở CP6 cho thấy rủi ro bỏ sót ca khẩn cấp gây hậu quả lớn hơn nhiều so với thời gian duyệt ticket.

3. Bộ 4 Tiêu chí đánh giá

1. Độ chính xác gợi ý nhãn :
    + Đạt khi: AI gợi ý đúng phân loại & phòng ban phụ trách ≥ 85% trên tổng số ticket thử nghiệm.

    + Không đạt khi: Độ chính xác gợi ý < 75%.

2. Tỷ lệ nhân viên bấm sửa (Human Override Rate):
    + Đạt khi: Nhân viên chỉ phải bấm chỉnh sửa lại gợi ý của AI ≤ 15% tổng số ticket.

    + Không đạt khi: Tỷ lệ bấm sửa > 25% (cho thấy gợi ý của AI làm phiền nhân viên hơn là hỗ trợ).

3. Phát hiện ca khẩn cấp:
    + Đạt khi: 100% các ticket chứa yếu tố khẩn cấp/an toàn được cắm cờ ưu tiên chính xác.

    + Không đạt khi: Bỏ sót dù chỉ 1 ticket khẩn cấp mà không cảnh báo.

4. Thời gian xử lý của nhân viên:
    + Đạt khi: Thời gian thao tác của nhân viên từ lúc mở ticket đến khi bấm chuyển giao trung bình ≤ 1.5 phút/ticket.

    + Không đạt khi: Thời gian thao tác trung bình > 2.5 phút/ticket.

## Mục 8: Quyết định (CP6)
1. Đánh giá 4 Rủi ro cốt lõi

1. Value Risk (Rủi ro về Giá trị): Medium.
    + Lý do: Nhân viên có thể phản đối nếu AI gợi ý sai nhiều làm mất công sửa. Tuy nhiên, bằng chứng CP4 cho thấy nhu cầu giảm tải giờ cao điểm là rất lớn.

2. Usability Risk (Rủi ro về Khả năng sử dụng): Low.
    + Lý do: Giao diện thiết kế dạng "1-click Approve" cực kỳ đơn giản, không làm thay đổi thói quen làm việc hiện tại của nhân viên.

3. Feasibility Risk (Rủi ro về Khả thi kỹ thuật): Medium.
    + Lý do: Cần có bộ dữ liệu ticket quá khứ được gán nhãn chuẩn của Vinhomes để huấn luyện NLP/OCR tiếng Việt.

4. Viability Risk (Rủi ro về Vận hành & Pháp lý): Low.
    + Lý do: Luôn có nhân viên kiểm duyệt (Human-in-the-loop), không vi phạm quyền riêng tư cư dân (dữ liệu được ẩn danh hóa trước khi xử lý), chi phí vận hành mô hình phân loại nhỏ là hợp lý.

2. Quyết định cuối cùng: NOT YET (Chưa triển khai ngay, cần kiểm chứng thêm)
- Lý do chọn NOT YET thay vì GO:
    + Mặc dù bài toán rất tiềm năng và có giá trị rõ ràng, nhưng nhóm hiện chưa có quyền truy cập vào tập dữ liệu log ticket thực tế của Vinhomes (khoảng 500-1000 ticket đã gán nhãn chuẩn) để đánh giá Feasibility (độ khả thi kỹ thuật của mô hình NLP tiếng Việt).

- Bước thử nghiệm nhỏ nhất tiếp theo (Smallest Next Step):
    + Thực hiện thử nghiệm trên tập mẫu 50 ticket ẩn danh giả định để đo thử độ chính xác của một mô hình NLP cơ bản trước khi đưa ra quyết định GO.

- Ngưỡng dừng:
    + Nếu qua đợt thử nghiệm nhỏ 50 ticket mà tỷ lệ gợi ý đúng của mô hình đạt < 70% hoặc thời gian phản hồi của hệ thống > 3 giây/ticket, nhóm sẽ lập tức DỪNG (STOP) dự án AI và chuyển hoàn toàn sang giải pháp Non-AI (Chuẩn hóa Form đăng ký trên App cư dân).
---

## 9. Hạn chế và hướng tiếp theo
- **Hạn chế:** 
  1. Mô hình đề xuất hiện tại mới chỉ dựa trên giả định logic và dữ liệu review công khai, chưa được kiểm chứng trên tập dữ liệu log thực tế của Vinhomes.
  2. Hệ thống chưa tích hợp xử lý tự động với các kênh khẩn cấp ngoài giờ hành chính.
- **Hướng tiếp theo:** 
  1. Triển khai thử nghiệm mô hình NLP đơn giản trên tập mẫu 50 ticket ẩn danh giả định để đánh giá độ chính xác.
  2. Phối hợp với đội ngũ vận hành thực tế để thu thập feedback cải tiến giao diện 1-click approve cho nhân viên CSKH.
-

## 10. Tài liệu tham khảo
- Google Play Store & Apple App Store — Đánh giá ứng dụng Vinhomes Resident (Truy cập tháng 10/2026).
- Google PAIR (People + AI Research) — Guidelines for Human-AI Interaction.
- Tài liệu hướng dẫn Day 02 AI Product Scoping Lab (VinUni & Vingroup).
-
