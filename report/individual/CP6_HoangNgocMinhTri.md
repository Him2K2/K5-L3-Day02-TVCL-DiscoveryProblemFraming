Mục 6: Mức can thiệp AI

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

Mục 7: Problem Statement v1 + Tiêu chí đánh giá
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

Mục 8: Quyết định
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