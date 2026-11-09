# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: TVCL
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Phân loại và định tuyến thông minh phản ánh của cư dân đến đúng bộ phận chuyên trách trên ứng dụng Vinhomes Resident.
- Quyết định cuối: Go / Not Yet / No-Go (sẽ chốt ở CP6)

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Nguyễn Thanh Liêm | Khi giáo viên nhắn tin báo sự cố trong giờ dạy ở các cơ sở, tôi muốn phân loại nhanh nội dung và chuyển ngay đến đúng người phụ trách, để sự cố được xử lý trong vòng 5 phút mà không phải lướt đọc thủ công từng nhóm chat. | Phòng giáo vụ & Giáo viên đứng lớp tại 5 cơ sở | Khâu đọc lọc tin nhắn chat và forward thủ công mất 7–8 phút/sự cố, dễ sót tin nhắn khi có nhiều lớp cùng báo lỗi đầu ca. | |
| 2 | Nguyễn Thanh Liêm | Khi một giáo viên gặp sự cố đột xuất không thể đứng lớp, tôi muốn tìm nhanh các giáo viên đang có lịch rảnh và ở gần cơ sở đó nhất, để gửi lời mời nhận lớp thay thế trong 10 phút mà không phải gọi điện dò hỏi từng người. | Quản lý đào tạo & Đội ngũ giáo viên/trợ giảng | Dò lịch rảnh trên Excel và gọi điện tuần tự từng người mất 25–30 phút; sau khi chốt còn mất thêm thời gian di chuyển của GV nhận lớp. | |
| 3 | Nguyễn Thanh Liêm | Khi trạm sạc công cộng kín chỗ vào giờ cao điểm, tôi muốn nhận diện được các xe đã sạc đầy nhưng vẫn chiếm chỗ đỗ, để yêu cầu nhường trụ hoặc được ban quản lý điều phối sạc kịp thời mà không phải chờ đợi hàng giờ. | Tài xế xe điện cá nhân (VinFast), Xanh SM & Bảo vệ bãi xe | Việc phải đi bộ kiểm tra thủ công màn hình từng trụ sạc và chờ đợi liên hệ chủ xe chiếm chỗ mất 20–25 phút/lần. | |
| 4 | Hoàng Ngọc Minh Trí | Khi tiếp nhận một phản ánh mới từ cư dân/khách hàng, tôi muốn nắm rõ ngay loại sự cố và khu vực phát sinh, để chuyển chính xác đến bộ phận xử lý chuyên trách mà không cần đọc đi đọc lại nhiều lần. | Nhân viên tiếp nhận / Điều phối viên Vinhomes & Cư dân | Đọc hiểu mô tả tự do, xem ảnh và đối chiếu danh mục phòng ban chồng chéo mất 2–4.5 phút/ticket; tỷ lệ gán nhầm 12%. | |
| 5 | Hoàng Ngọc Minh Trí | Khi thông tin sự cố do cư dân cung cấp bị thiếu sót (thiếu số căn hộ, thiếu hình ảnh hiện trạng), tôi muốn biết chính xác thông tin nào còn thiếu, để phản hồi yêu cầu bổ sung ngay mà không làm gián đoạn hay kéo dài thời gian xử lý. | Nhân viên CSKH & Cư dân Vinhomes | Mất 3–4 lượt nhắn tin/gọi điện hỏi lại thông tin ban đầu, kéo dài thời gian xử lý trung bình từ 15 phút lên 180 phút. | |
| 6 | Hoàng Ngọc Minh Trí | Khi xử lý một ticket kéo dài qua nhiều ca trực hoặc trao đổi nhiều lượt, tôi muốn nắm bắt ngay các dữ kiện quan trọng chính, để đưa ra phương án giải quyết mà không bỏ sót bối cảnh lịch sử. | Trưởng nhóm vận hành & Kỹ thuật viên | Nhân viên ca mới tiếp quản mất trung bình 8–12 phút chỉ để đọc lại toàn bộ lịch sử trò chuyện và ghi chú cũ trước khi xử lý. | |
| 7 | Nguyễn Thế Cường | Khi kiểm thử nhận diện biển báo và vạch làn trên video, tôi muốn biết kết quả nào sai hoặc đến muộn, để chọn đúng lỗi cần cải thiện mà không phải soi từng frame. | Kỹ sư CV, Kỹ sư kiểm thử xe tự hành VinFast | Phải kiểm tra thủ công từng frame video mất nhiều giờ; khâu tìm nguyên nhân gây trễ suy luận mất nhiều thời gian. | |
| 8 | Nguyễn Thế Cường | Khi đối soát một lô phiên sạc xe điện, tôi muốn tìm các phiên không khớp hóa đơn, để xử lý đúng giao dịch bị lệch mà không phải đối chiếu thủ công từng dòng. | Nhân viên đối soát, Bộ phận thanh toán VinFast | Dò thủ công từng dòng giao dịch giữa bảng kê ngân hàng và log trụ sạc mất nhiều giờ; dễ sai sót số liệu. | |
| 9 | Nguyễn Thế Cường | Khi đọc một phiếu mô tả lỗi xe từ khách hàng, tôi muốn xác định triệu chứng và bộ phận tiếp nhận, để tránh chuyển phiếu sai nhóm kỹ thuật. | Nhân viên hỗ trợ kỹ thuật, Kỹ thuật viên xưởng 3S | Đọc và phân loại triệu chứng xe từ phiếu mô tả tự do; mất thời gian đọc hiểu và dễ chuyển sai xưởng. | |
| 10 | Hồ Xuân Vũ | Khi sinh viên/cựu sinh viên làm thủ tục xin cấp giấy tờ tại trường, tôi muốn nộp và tra cứu hồ sơ online, để nhận kết quả trong ngày mà không phải đến trường xếp hàng và chờ đợi 3 ngày. | Sinh viên/cựu sinh viên & Cán bộ văn phòng một cửa | Cán bộ phải tra cứu hồ sơ/bảng điểm lưu trữ thủ công mất 2 ngày; sinh viên phải đến trực tiếp xếp hàng nộp giấy. | |
| 11 | Hồ Xuân Vũ | Khi sử dụng Google Maps mà gặp đoạn đường Hà Nội đang rào chắn thi công hoặc mới thông luồng, tôi muốn bản đồ cập nhật ngay lộ trình đúng, để không bị chỉ đường sai và đi vào ngõ cụt. | Người tham gia giao thông tại Hà Nội | Tấp xe vào lề dừng lại tìm đường thay thế và hỏi người dân mất 10–15 phút; gây nguy hiểm và trễ giờ. | |
| 12 | Hồ Xuân Vũ | Khi đến công ty chấm công bằng vân tay, tôi muốn ghi nhận chấm công nhanh và không phải chạm tay vào máy chung, để tránh nguy cơ lây bệnh truyền nhiễm và giảm ùn tắc đầu giờ. | Nhân viên văn phòng | Xếp hàng chờ bấm vân tay vào giờ cao điểm sáng mất 5–10 phút; máy bẩn hoặc nhận diện vân tay chập chờn. | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| **A — Phân loại & Định tuyến yêu cầu/sự cố (Triage & Routing)** | Candidate #1 (Liêm), #4 (Trí), #5 (Trí), #6 (Trí), #9 (Cường) | Gom thông tin văn bản/hình ảnh phản ánh từ người dùng (ngôn ngữ tự nhiên, không cấu trúc), đọc hiểu nội dung, phân loại mức độ khẩn cấp và định tuyến chính xác đến đúng bộ phận chuyên trách để xử lý. |
| **B — Giao thông, Định vị & Thị giác máy tính (Mobility & Vision)** | Candidate #3 (Liêm), #7 (Cường), #11 (Vũ) | Thu thập và xử lý tín hiệu không gian/hình ảnh thực tế (camera, bản đồ, trạng thái trụ sạc) để cảnh báo sai lệch hoặc tối ưu di chuyển. |
| **C — Thủ tục hành chính & Vận hành nội bộ (Operations & Admin)** | Candidate #2 (Liêm), #8 (Cường), #10 (Vũ), #12 (Vũ) | Đối soát dữ liệu bảng tính, lịch trình, đối chiếu quy định thủ tục giấy tờ và quy trình vận hành giữa các bộ phận. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian phản hồi và tỷ lệ chuyển sai bộ phận khi xử lý phản ánh của cư dân Vinhomes
├── Opportunity A: Cư dân mô tả bằng câu chữ tự do, không theo cấu trúc, thiếu thông tin số phòng/vị trí cụ thể
├── Opportunity B: Danh mục phân loại phòng ban nội bộ bị chồng chéo (Kỹ thuật điện/nước vs Bảo trì tòa nhà)
└── Opportunity C: Điều phối viên đọc thủ công từng ticket, mở ảnh đối chiếu và chuyển tiếp bằng tay tạo điểm nghẽn
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- ✗ *"Chatbot AI tự động trả lời cư dân"* $\rightarrow$ Đây là Solution (công cụ AI), không phải nhu cầu hay nỗi đau của người dùng.
- ✗ *"Bắt buộc cư dân tự chọn phòng ban qua cây thư mục (dropdown) trên App"* $\rightarrow$ Đây là Solution (sửa giao diện app), thậm chí còn làm tăng gánh nặng cho cư dân vì họ không nắm rõ cơ cấu tổ chức phòng ban của ban quản lý.
- ✗ *"Hệ thống tự động giao việc trực tiếp cho kỹ thuật viên mà không cần người duyệt"* $\rightarrow$ Đây là Solution (tính năng tự động hóa), vi phạm ranh giới an toàn vận hành (Human-in-the-loop).

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

**Xử lý bất đồng (nếu có):**  
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

*Ảnh chụp minh chứng đánh giá thực tế của cư dân từ Google Play Store và Apple App Store (đã gộp):*
![Đánh giá thực tế của cư dân trên Google Play và App Store](../assets/cp4-review-snapshot-1.png)

**Nhóm đã sửa problem thế nào sau kiểm chứng:**  
1. **Mở rộng phạm vi phân loại (Category Scope):** Ban đầu nhóm chỉ dự định phân loại các sự cố hỏng hóc kỹ thuật (điện, nước, điều hòa). Sau khi đọc review thực tế, nhóm nhận thấy nhu cầu phản ánh của cư dân phân bổ rất nhiều vào mảng **Dịch vụ cư dân & Tiện ích số (thẻ xe, thẻ ra vào, intercom, rác thải)**. Do đó, nhóm bổ sung danh mục định tuyến bao gồm cả 4 mảng nghiệp vụ cốt lõi của ban quản lý.  
2. **Xác lập Ranh giới (Boundary) & Kênh khẩn cấp:** Từ phản hồi của nhà phát triển về việc gọi Hotline 1900 2323 89 (nhánh 4), nhóm xác định rõ: **Hệ thống AI chỉ đóng vai trò phân loại và định tuyến các phản ánh phi khẩn cấp trên App**. Nếu phát hiện sự cố khẩn cấp hoặc lỗi hệ thống nghiêm trọng, giao diện sẽ kích hoạt nút gọi ngay đến Hotline tổng đài thay vì để ticket rơi vào hàng đợi xử lý.

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
