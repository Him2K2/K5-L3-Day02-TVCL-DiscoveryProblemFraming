# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: TVCL
- Candidate problem nhóm chọn (1 câu): Phân loại và định tuyến thông minh phản ánh của cư dân đến đúng bộ phận chuyên trách trên ứng dụng Vinhomes Resident.
- Quyết định cuối (Go / Not Yet / No-Go): Go (Thực hiện pilot thử nghiệm quy mô nhỏ tại 1 phân khu trong 2 tuần).

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
- Thu thập và phân tích 4 đánh giá (reviews) thực tế của cư dân trên Google Play Store và Apple App Store cho ứng dụng Vinhomes Resident; chụp 2 ảnh snapshot đưa vào thư mục `report/assets/`.
- Phát hiện tín hiệu phản bác quan trọng: cư dân gặp bức xúc lớn ở mảng dịch vụ tiện ích số (thẻ xe, intercom) và kênh Hotline 1900 2323 89 là kênh cứu cánh khi app lỗi; từ đó giúp nhóm xác lập Boundary: AI chỉ phân loại ticket phi khẩn cấp trên app, ca khẩn cấp điều hướng gọi hotline.
- Hỗ trợ Vũ ở CP3: tham gia thảo luận gom 12 candidate thành 3 cụm (Cluster A, B, C), hoàn thiện cây OST (chỉ rõ 3 opportunity và gạch bỏ 3 solution trá hình), và chấm điểm 4 candidate theo 7 tiêu chí.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Mục 3.1 (Assumption Map) và Mục 3.2 (Kiểm chứng qua Review + Snapshot #1, #2 + Bảng tổng hợp + Nhóm đã sửa problem thế nào) trong `report/team/group_report.md`.
- File ảnh minh chứng: `report/assets/review_cu_dan.png` và `report/assets/review_cu_dan_2.png`.
- Lịch sử commit trên nhánh `ntl`: commit `5424daf` (`docs(team): update group_report with CP3 convergence and CP4 validation reviews`).

**Điều mình học được từ phần nhóm:**

- Hiểu sâu sắc giá trị của việc kiểm chứng thực tế từ người dùng (The Mom Test / Reviews thật) thay vì tự ngồi tưởng tượng giả định trong phòng. Việc phát hiện ra các vấn đề về thẻ xe kéo dài cả tuần và sự tồn tại của kênh Hotline 1900 2323 89 đã trực tiếp giúp nhóm tránh được bẫy "thần thánh hóa AI" và xác định đúng ranh giới an toàn cho hệ thống (Human-in-the-loop).
