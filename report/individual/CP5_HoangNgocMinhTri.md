1. Quy trình hiện tại
[Cư dân gửi ticket thô] 
  ↓ (0.5 phút)
[1. Hệ thống ghi nhận & đẩy vào hàng đợi]
  ↓ (2.0 phút)
[2. Nhân viên mở đọc nội dung & xem ảnh đính kèm]  ← [BOTTLENECK: Mất nhiều thời gian do text không chuẩn]
  ↓ (1.0 phút)
[3. Nhân viên tra cứu danh mục phòng ban & xác định đơn vị]
  ↓ (0.5 phút)
[4. Gán nhãn & bấm chuyển giao ticket]

------
Bảng chi tiết bước (Table):

Bước 1: Tiếp nhận ticket | Actor: Hệ thống / Nhân viên | Input: Notification | Output: Ticket mới trong hàng đợi | Thời gian: 0.5 phút | Ghi chú: Giờ cao điểm bị xếp hàng.

Bước 2: Đọc nội dung & xem ảnh | Actor: Nhân viên CSKH | Input: Ticket thô | Output: Hiểu sơ bộ sự cố | Thời gian: 2.0 phút | Ghi chú: BOTTLENECK (Do mô tả dài, thiếu cấu trúc).

Bước 3: Tra cứu danh mục & chọn phòng ban | Actor: Nhân viên CSKH | Input: Nội dung đã đọc | Output: Xác định đúng/sai bộ phận | Thời gian: 1.0 phút | Ghi chú: Dễ nhầm lẫn giữa các phòng ban chồng chéo.

Bước 4: Gán nhãn & chuyển giao | Actor: Nhân viên CSKH | Input: Phân loại | Output: Ticket chuyển đến đúng đội | Thời gian: 0.5 phút | Ghi chú: Hoàn tất bước phân phối ban đầu.
------
2. Quy trình tương lai
Thiết kế luồng tương lai (Có sự kết hợp Rule, AI và Con người):

Cư dân tạo ticket qua App -> [Rule] Hệ thống bắt buộc chọn 2 trường tối thiểu (Loại sự cố + Vị trí căn hộ) kèm ảnh hiện trạng.

Hệ thống nhận dữ liệu -> [AI] Mô hình NLP + OCR tự động phân tích cú pháp, trích xuất từ khóa và gợi ý sẵn 1 nhãn phân loại tối ưu nhất kèm độ tin cậy (Confidence score).

Nhân viên điều phối kiểm tra -> [Con người / Human-in-the-loop] Nhân viên nhìn vào gợi ý của AI, chỉ mất 1 giây bấm [Xác nhận / Duyệt] hoặc đổi sang nhãn khác nếu AI đoán sai.

Chuyển giao tự động -> Hệ thống tự định tuyến đến đúng bộ phận chuyên trách.

Fallback (Phương án dự phòng nếu AI lỗi): Nếu hệ thống AI mất kết nối hoặc độ tin cậy thấp dưới 60%, giao diện tự động chuyển về dạng danh mục truyền thống để nhân viên chọn thủ công (không làm gián đoạn vận hành).

Quy định giới hạn (Boundaries): Hệ thống không được phép tự động đóng ticket hoặc tự động chuyển hướng các ca khẩn cấp (như hỏa hoạn, ngập nước nặng) mà bắt buộc phải qua xác nhận trực tiếp của con người.

3. So sánh Before / After
|Tiêu chí| |Quy trình hiện tại| |Quy trình tương lai (Dự kiến)|
|Số bước thao tác| |4 bước thủ công| |3 bước (AI Suggest)|
|Tổng thời gian xử lý| |~ 4.0 phút / ticket| |~ 1.5 phút / ticket|
|Số bước thủ công thuần túy| |4 bước| |1 bước kiểm tra/xác nhận cuối cùng|
|Điểm nghẽn (Bottleneck)| |Bước đọc hiểu mô tả thô & tra cứu danh mục thủ công| |Thời gian hệ thống AI phản hồi (dự kiến < 0.5 giây)|
|Rủi ro phát sinh mới| |Sai sót do nhân viên mệt mỏi giờ cao điểm| |Rủi ro AI gợi ý nhãn sai (cần có nhân viên duyệt lại)|

4. PROBLEM STATEMENT
Điền hoàn chỉnh 6 trường thông tin chuẩn theo khung Lean UX:

- Actor (Đối tượng chịu tác động): Nhân viên điều phối / CSKH tổng đài tại khu đô thị Vinhomes.

- Quy trình (Process): Tiếp nhận, đọc hiểu nội dung phản ánh thô và thực hiện phân loại, định tuyến ticket thủ công cho hàng trăm yêu cầu đổ về trong giờ cao điểm.

- Bottleneck (Điểm nghẽn): Bước đọc mô tả dài dòng, thiếu cấu trúc và tra cứu danh mục phân loại chồng chéo tốn trung bình 2.0 phút cho mỗi ticket (chiếm >44% thời gian xử lý ban đầu).

- Impact (Tác động nếu không giải quyết): Gây ùn tắc hàng đợi ticket giờ cao điểm, tăng tỷ lệ chuyển nhầm bộ phận (ước tính 12%), kéo dài thời gian chờ phản hồi của cư dân và làm nhân viên quá tải.

- Success Metric (Chỉ số thành công đo lường):

    + Baseline (Hiện tại): Thời gian xử lý đầu nhận ban đầu là 4.0 phút/ticket; Tỷ lệ chuyển sai bộ phận là 12%.

    + Target (Mục tiêu kỳ vọng): Giảm thời gian xử lý ban đầu xuống < 1.5 phút/ticket; Giảm tỷ lệ chuyển sai bộ phận xuống < 3%.

    + Phương pháp đo: Thống kê tự động thời gian từ lúc ticket tạo đến khi hoàn tất gán nhãn trên hệ thống log trong ca trực 8 tiếng.

- Boundary (Giới hạn hệ thống): Hệ thống AI chỉ đóng vai trò gợi ý tham khảo, tuyệt đối không được tự ý tự động chuyển giao hoặc tự đóng ticket khẩn cấp mà bắt buộc phải có sự xác nhận của nhân viên điều phối (Human-in-the-loop).