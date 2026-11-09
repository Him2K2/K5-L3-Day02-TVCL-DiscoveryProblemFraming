1. Assumption Map (Bản đồ giả định)
Lập 4–6 dòng giả định cốt lõi cần kiểm chứng cho bài toán phân loại ticket:

Giả định 1: Nhân viên CSKH mất nhiều thời gian nhất ở khâu đọc hiểu nội dung thô và tra cứu bộ phận xử lý. (Loại: Usability / Importance: 5 / Evidence: 2) -> Cần test trước

Giả định 2: Danh mục phân loại hiện tại của ban quản lý đang bị chồng chéo, khiến nhân viên dễ phân vân chọn sai phòng ban. (Loại: Value / Importance: 5 / Evidence: 2) -> Cần test trước

Giả định 3: Cư dân sẵn sàng chọn đúng nhãn phân loại từ trước trên App nếu giao diện trực quan và dễ sử dụng. (Loại: Usability / Importance: 4 / Evidence: 1)

Giả định 4: Mô hình gợi ý tự động (AI/Rule) có thể đạt độ chính xác trên 85% với dữ liệu tiếng Việt thực tế. (Loại: Feasibility / Importance: 4 / Evidence: 1)

2. Kiểm chứng thực tế (Validation - Interview/Survey)
Phương pháp: Phỏng vấn 2–3 nhân viên vận hành / CSKH hoặc khảo sát thực tế (lưu ý: không phỏng vấn thành viên trong nhóm). Ghi nhận bằng Snapshot theo đúng 6 trường bắt buộc:

Role (Vai trò): Nhân viên điều phối CSKH tòa nhà.

Memorable quote (Câu nói đáng nhớ): "Nhiều lúc cư dân chỉ chụp một cái ảnh bóng đèn tối và ghi mỗi chữ 'hỏng', mình phải gọi lại hỏi tầng mấy, khu nào, rồi mới biết chuyển cho kỹ thuật điện hay bảo trì dân dụng."

Last occurrence (Lần gần nhất xảy ra): Ca trực sáng thứ Hai tuần trước, dồn 45 ticket trong vòng 30 phút giờ cao điểm.

Current workaround (Giải pháp thay thế hiện tại): Mở lịch sử chat cũ, gọi điện thoại trực tiếp hoặc tra cứu danh bạ nội bộ trên Excel.

Time/Frequency (Thời gian/Tần suất): Mất trung bình 4–5 phút cho mỗi ticket phức tạp; lặp lại hàng chục lần mỗi ca.

Insight (Bài học rút ra): Nút thắt không nằm ở tốc độ đánh máy của nhân viên, mà nằm ở việc thông tin đầu vào từ cư dân thiếu cấu trúc và danh mục nội bộ bị phân mảnh.

Tổng kết bằng chứng:

Số lượng mẫu: 2 nhân viên CSKH được phỏng vấn.

Tín hiệu củng cố: Cả 2 đều xác nhận mất nhiều thời gian đọc và phân loại nhầm phòng ban vào giờ cao điểm.

Tín hiệu bác bỏ : Ban đầu nghĩ lỗi do hệ thống phần mềm chậm, nhưng thực tế phần lớn do thông tin mô tả của cư dân không chuẩn xác và danh mục phân loại nội bộ quá nhiều phân nhánh nhỏ.

Cập nhật/Sửa đổi bài toán: Sau kiểm chứng, nhóm điều chỉnh trọng tâm bài toán từ "AI tự động hoàn toàn" sang "Chuẩn hóa đầu vào kết hợp AI gợi ý 1-click (Human-in-the-loop)".

3. Research giải pháp đã có trên thị trường
Nghiên cứu 2–3 mô hình/công cụ thực tế (như Zendesk Support Suite, Freshdesk AI, hoặc hệ thống ticket nội bộ):

Zendesk Answer Bot / Intent Suggestion:

Bước xử lý: Tự động đọc nội dung ticket đến và gợi ý macro/nhãn phân loại.

Điểm mạnh: Xử lý nhanh, tích hợp sẵn.

Điểm yếu/Hạn chế: Chi phí cao, độ chính xác với tiếng Việt địa phương (slang/viết tắt của cư dân Việt Nam) đôi khi bị lệch.

Bài học cho nhóm: Cần có cơ chế "Human-in-the-loop" (nhân viên bấm duyệt) chứ không nên để hệ thống tự động định tuyến 100% tránh sai sót trầm trọng.

Quy trình phân loại thủ công kết hợp Form bắt buộc (Standardized Form Routing):

Bước xử lý: Bắt buộc cư dân chọn Dropdown phân nhóm trước khi gửi.

Điểm mạnh: Giải quyết triệt để 70% lỗi thiếu thông tin đầu vào mà không tốn chi phí công nghệ cao.

Điểm yếu/Hạn chế: Cư dân lười đọc, thường chọn bừa mục "Khác" nếu form quá dài.