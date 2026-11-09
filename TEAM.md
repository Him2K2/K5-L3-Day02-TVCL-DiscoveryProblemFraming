# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: TVCL
- Candidate problem nhóm chọn (1 câu): Phân loại và định tuyến thông minh phản ánh của cư dân đến đúng bộ phận chuyên trách trên ứng dụng Vinhomes Resident.
- Quyết định cuối (Go / Not Yet / No-Go): Not Yet.

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Hoàng Ngọc Minh Trí | 2A202603379 | điều phối, phụ trách quy trình CP5 | GaGionCay |
| 2 | Nguyễn Thanh Liêm | 2A202603358 | Phụ trách chính Kiểm chứng CP4, phản biện lựa chọn đề tài | liemt0165 |
| 3 | Nguyễn Thế Cường | 2A202603355 | Phản biện kỹ thuật & dữ liệu, Hỗ trợ kiểm chứng | nthungmta207 |
| 4 | Hồ Xuân Vũ | 2A202603406 | Nhóm trưởng, Pitch Problem Card chính, , Phụ trách chính Hội tụ nhóm CP3 | Him2K2 |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Hồ Xuân Vũ | Nguyễn Thanh Liêm, Hoàng Ngọc Minh Trí, Nguyễn Thế Cường | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Nguyễn Thanh Liêm | Hồ Xuân Vũ, Nguyễn Thế Cường, Hoàng Ngọc Minh Trí | Assumption map, snapshot hoặc survey |
| CP4 — Research | Nguyễn Thanh Liêm | Hoàng Ngọc Minh Trí | Bảng research có link |
| CP5 — Quy trình trước/sau | Hoàng Ngọc Minh Trí | Nguyễn Thanh Liêm | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | Hoàng Ngọc Minh Trí | Hồ Xuân Vũ, Nguyễn Thế Cường | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Nguyễn Thanh Liêm | Hoàng Ngọc Minh Trí | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | Hồ Xuân Vũ | Nguyễn Thanh Liêm | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### NguyenThanhLiem-2A202603358

**Phần việc phụ trách:**

- **Phụ trách chính:** CP4 — Kiểm chứng + research giải pháp đã có (với sự hỗ trợ của Vũ, Cường, Trí).
- **Hỗ trợ:** CP3 — Hội tụ nhóm (Vũ làm chính, Liêm hỗ trợ thảo luận cluster, OST và chấm điểm candidate).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Xây dựng Assumption Map gồm 5 giả định theo 4 khía cạnh (Value, Usability, Feasibility, Viability), xác định 2 giả định #1 và #4 cần kiểm chứng trước.
- Thu thập và phân tích 4 đánh giá (reviews) thực tế của cư dân trên Google Play Store và Apple App Store cho ứng dụng Vinhomes Resident; tạo file tài liệu tổng hợp `report/assets/cp4-review-snapshot-1.md` và ảnh minh chứng gộp `report/assets/cp4-review-snapshot-1.png`.
- Phát hiện tín hiệu phản bác quan trọng: cư dân gặp bức xúc lớn ở mảng dịch vụ tiện ích số (thẻ xe, intercom) và kênh Hotline 1900 2323 89 là kênh cứu cánh khi app lỗi; từ đó giúp nhóm xác lập Boundary: AI chỉ phân loại ticket phi khẩn cấp trên app, ca khẩn cấp điều hướng gọi hotline.
- Hỗ trợ Vũ ở CP3: tham gia thảo luận gom 12 candidate thành 3 cụm (Cluster A, B, C), hoàn thiện cây OST (chỉ rõ 3 opportunity và gạch bỏ 3 solution trá hình), và chấm điểm 4 candidate theo 7 tiêu chí.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Trong `report/team/group_report.md`: Mục 3.1 (Assumption Map) và Mục 3.2 (Kiểm chứng qua Review + Snapshot #1, #2 + Bảng tổng hợp + Nhóm đã sửa problem thế nào sau kiểm chứng).
- Trong `report/assets/`:
  - `report/assets/cp4-review-snapshot-1.md` (file tài liệu tổng hợp 2 Review Snapshot chi tiết).
  - `report/assets/cp4-review-snapshot-1.png` (ảnh minh chứng đánh giá thực tế của cư dân từ Google Play và App Store đã gộp).
  - `report/assets/cp2-workflow-card-1.png` (ảnh sơ đồ quy trình nháp cho Problem Card #1).
  - `report/assets/cp5-workflow-future.png` (ảnh sơ đồ quy trình tương lai kết hợp Rule, AI và HITL).
- Lịch sử commit trên nhánh `ntl`: commit `5424daf`, `bbd1240`, `8215a0a`, `5c733a9`.

**Điều mình học được từ phần nhóm:**

- Hiểu sâu sắc giá trị của việc kiểm chứng thực tế từ người dùng (The Mom Test / Reviews thật) thay vì tự ngồi tưởng tượng giả định trong phòng. Việc phát hiện ra các vấn đề về thẻ xe kéo dài cả tuần và sự tồn tại của kênh Hotline 1900 2323 89 đã trực tiếp giúp nhóm tránh được bẫy "thần thánh hóa AI" và xác định đúng ranh giới an toàn cho hệ thống (Human-in-the-loop).


### NguyenTheCuong-2A202603355

**Phần việc phụ trách:**

- **Vai trò:** Phản biện kỹ thuật và dữ liệu; rà tính khả thi, cách đo và giới hạn của phương án đề xuất.
- **Hỗ trợ CP3 — Hội tụ nhóm:** Pitch ba Problem Card, đặt câu hỏi phản biện và trao đổi để chọn đề tài cùng nhóm do Vũ phụ trách chính.
- **Hỗ trợ CP4 — Kiểm chứng:** Rà số liệu và đối chiếu kết quả review do Liêm tổng hợp; không nhận phần trực tiếp phỏng vấn hoặc thu thập review.
- **Hỗ trợ CP5 — Problem Statement v0:** Hỗ trợ Trí tổng hợp v0, đồng thời đóng góp nội dung quy trình trước/sau và bảng before/after.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Chuẩn bị và pitch ba vấn đề: kiểm thử nhận diện biển báo/vạch làn, đối soát phiên sạc và phân loại mô tả lỗi xe. Sau trao đổi về dữ liệu và phạm vi lab, đồng thuận chọn bài phản ánh cư dân của Trí.
- Đặt câu hỏi cho Vũ về cách triển khai bài Google Maps và tính khả thi của bài thủ tục hành chính khi tần suất sử dụng thấp; tiếp nhận phản biện của Liêm về điều kiện nhận diện ban đêm, lợi ích của đối soát và tiêu chí ưu tiên khi phân loại lỗi xe.
- Rà baseline và cách tính thời gian: phân biệt số liệu 4.5 phút/ticket kế thừa từ bài nguồn, tỷ lệ chuyển sai khoảng 12% còn là ước tính và ngân sách 1.4 phút/ticket chưa được thử nghiệm. Nêu điểm cần làm rõ khi 120 ticket nhân 4.5 phút vượt thời lượng một ca 8 giờ nếu chỉ có một người thao tác tuần tự.
- Tổng hợp quy trình hiện tại 5 bước và phương án tương lai 4 bước; làm rõ actor, input, output, bước nhân viên duyệt và cách quay về thủ công khi gợi ý sai hoặc công cụ lỗi.
- Đóng góp bảng before/after và Problem Statement v0 đủ 6 trường; giữ mục tiêu dưới 1.5 phút/ticket, chuyển sai dưới 3% ở trạng thái đề xuất, tính cả công duyệt/sửa và báo riêng thời gian chờ, ca ngoại lệ.
- Rà boundary: AI chỉ gợi ý trong danh mục đã duyệt, không tự thêm dữ kiện, đổi ưu tiên hoặc đóng ticket; giữ biểu mẫu/danh mục/Rule làm phương án đối chứng trước khi cân nhắc AI.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Mục 2.1 và 2.4 của `report/team/group_report.md`: pitch, câu hỏi phản biện và lý do đồng thuận chọn đề tài.
- Mục 4.1–4.3 và 5 của `report/team/group_report.md`: phần quy trình, before/after, v0, cách đo và phản biện tôi đóng góp tổng hợp.
- [Báo cáo cá nhân](report/individual/2A202603355_NguyenTheCuong.md), mục 4–6: nhật ký đóng góp, dùng AI và reflection.
- Commit `d054289` trên nhánh `NguyenTheCuong-2A202603355` (`Feat: Complete individual assignment by Nguyen The Cuong`): cập nhật báo cáo cá nhân ghi nhận phần việc. Đây là minh chứng báo cáo cá nhân, không thay thế kết quả đo hoặc commit báo cáo nhóm.

**Điều mình học được từ phần nhóm:**

- Ban đầu tôi ưu tiên bài nhận diện biển/vạch vì đúng hướng mình quan tâm. Khi trao đổi cùng nhóm, tôi thấy khả năng lấy dữ liệu và kiểm chứng trong thời gian lab cũng quan trọng như ý tưởng kỹ thuật. Làm CP5 giúp tôi chú ý hơn đến việc tách số liệu hiện tại khỏi mục tiêu dự kiến, tính cả thời gian người duyệt sửa gợi ý và hỏi xem Rule đã đủ chưa trước khi chọn AI. Có ít bước hơn chưa chắc đã nhanh hơn, nên phần before/after vẫn cần được đo thử thực tế.


### HoangNgocMinhTri-2A202603379

**Phần việc phụ trách:**

- **Phụ trách chính:** CP5 — Quy trình trước/sau và Problem Statement v0.
- **Hỗ trợ:** CP3 — Pitch Problem Card và thảo luận hội tụ; CP4 — research/kiểm chứng; CP6 — phân tích mức can thiệp và rủi ro.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đề xuất và pitch bài toán phân loại, định tuyến phản ánh của cư dân Vinhomes; nêu câu hỏi phản biện về việc chuẩn hóa biểu mẫu/danh mục trước khi cân nhắc AI.
- Mô tả quy trình tiếp nhận ticket hiện tại và xác định các bước đọc nội dung, phân loại và chuyển giao cần được đo lường.
- Đóng góp vào quy trình tương lai và Problem Statement, trong đó AI chỉ gợi ý nhãn/phòng ban để nhân viên xem xét; các trường hợp nhạy cảm hoặc cần xử lý khẩn cấp không được tự động định tuyến.
- Tham gia thảo luận về phương án không dùng AI, cách đo thời gian xử lý và tỷ lệ chuyển sai, cùng điều kiện dữ liệu cần có trước khi thử nghiệm.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Báo cáo cá nhân: `report/individual/2A202603379_HoangNgocMinhTri.md`, mục 3–5.
- Báo cáo nhóm: `report/team/group_report.md`, các mục về CP3, CP5 và CP6.

**Điều mình học được từ phần nhóm:**

- Qua việc mô tả quy trình và nhận phản biện, mình nhận ra cần phân biệt số liệu đo được với ước tính, kiểm tra phương án không dùng AI trước, và xác định rõ vai trò duyệt của nhân viên cùng các giới hạn an toàn trước khi đề xuất tự động hóa.
### HoXuanVu-2A202603406

**Phần việc được phân công:**

- **Vai trò:** Nhóm trưởng, Pitch Problem Card chính.
- **Phụ trách chính CP3 — Hội tụ nhóm:** Cluster, cây OST, bảng chấm điểm.
- **Đóng góp khi hội tụ nhóm:** Đặt câu hỏi phản biện cho các ý tưởng của mọi người, tổng hợp ý kiến và cùng nhóm chốt phương án cuối cùng.
- **Hỗ trợ CP4 — Kiểm chứng:** Assumption map, snapshot hoặc survey.
- **Hỗ trợ CP5 — Problem Statement v0:** Problem Statement v0.
- **Phụ trách chính CP6 — Quyết định:** 4 rủi ro + Go/Not Yet/No-Go.
