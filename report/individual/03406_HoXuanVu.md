# Bài làm của Vũ

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | tốn thời gian | Tôi tham gia khóa học trên mạng và việc kiếm tài liệu rất khó khăn | Người dùng web | Phải tìm đến khóa học, lướt tìm ngày học và kiếm đến phần chia sẻ mới tìm ra file pdf |
| 2 | tốn thời gian | Tôi sử dụng Google Maps nhưng dạo gần đây đường Hà Nội có những nơi đang xây dựng, có những nơi vừa xây xong đã thông luồng, việc Google Maps update chậm thông tin khiến nó chỉ đường sai cho tôi | Người dùng Google Maps | Tôi bị chỉ đường sai và phải quay lại, gây nguy hiểm |
| 3 | lặp lại | Khi đi làm tôi thấy nhân viên tính lương phải tính lương cho mọi người để gửi bảng lương, việc này lặp đi lặp lại mà việc tính lương dựa trên các số liệu có sẵn đã tổng hợp, và phải gửi mail cho từng người | Kế toán | Sai sót của bảng lương, gửi nhầm bảng lương |
| 4 | tốn thời gian | Chấm công thủ công bằng tay, gây mất thời gian và mất vệ sinh khi cùng nhấn vào một nút chấm công, có thể lây cho nhau bệnh truyền nhiễm như Covid, có những ngày nhân viên gặp vấn đề về bản thân mà mong người khác thấu hiểu | Nhân viên | Cả công ty cùng bị một bệnh truyền nhiễm như Covid, khó chịu khi làm việc |
| 5 | tốn thời gian | Sếp quản lý nhân viên về hiệu suất làm việc để có những nhắc nhở cho ai có dấu hiệu làm việc không tập trung, ra ngoài nhiều | Sếp | Phải nhắc nhở nhân viên gây mất thời gian và ảnh hưởng về mặt tình cảm nhưng vẫn phải đảm bảo hiệu suất công việc |
| 6 | lặp lại | Những người bị những bệnh ngoài da dễ chẩn đoán nhưng vẫn phải cần bác sĩ xem bệnh và lập bệnh án thủ công | Bác sĩ | Gây quá tải, áp lực công việc cho bác sĩ |
| 7 | bất tiện | Tôi đi siêu thị mua sắm và khi thanh toán phải xếp hàng dài ở quầy thu ngân vì chỉ có vài quầy mở, trong khi tôi chỉ mua vài món đồ nhanh | Khách hàng | Khách hàng bỏ giỏ hàng đi về không mua nữa hoặc cảm thấy bực bội vì mất thời gian chờ đợi |
| 8 | tốn thời gian | Tôi là sinh viên đi làm thủ tục hành chính tại trường đại học, mỗi lần cần xin giấy xác nhận sinh viên phải đến tận phòng ban xếp hàng, điền giấy tờ bằng tay và chờ đợi nhiều ngày | Sinh viên | Sinh viên phải nghỉ học để đến trường làm thủ tục, tốn nhiều thời gian di chuyển và chờ đợi, web trường đã khác chức năng mới khó tìm kiếm đến mục mình cần tìm thông tin mờ mịt sau khi ra trường đã lâu |
| 9 | lặp lại | Tôi làm công việc chăm sóc khách hàng, mỗi ngày phải trả lời những câu hỏi giống hệt nhau về chính sách đổi trả hàng cho hàng chục khách hàng nhắn tin tới fanpage | Nhân viên CSKH | Nhân viên bị quá tải, mệt mỏi vì gõ lại nội dung giống nhau liên tục, dễ trả lời chậm hoặc thiếu sót |

---

# Top 3 Problem Cards (CP2)

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Google Maps sai (#2) | Tốn thời gian, gây nguy hiểm tính mạng | Có thực sự nhiều người bị sai như mình, và cần làm gì để giải quyết vấn đề (sản phẩm như thế nào?) |
| 2 | Chấm công bằng vân tay (#4) | Thuận tiện, cải thiện sức khỏe & tinh thần | AI có thực sự hiểu được cảm xúc của con người qua khuôn mặt để ra cảnh báo cho sếp để có biện pháp với người đang có vấn đề hay không? |
| 3 | Thủ tục cho sinh viên cũ lâu (#8) | Nhiều người đau, impact rộng | Tệp khách hàng ít |

---

# Card #1: Google Maps sai chưa update kịp tốc độ sửa đường Hà Nội

```text
HIỆN TẠI — 20 phút

[1 Phát hiện chỉ đường sai: 2'] → [2 Tấp lề dừng xe tìm đường thay thế: 5']
→ [3 So sánh các lộ trình thay thế trên app: 5'] → [4 Hỏi người dân / định hướng thực tế: 5'] ← BOTTLENECK
→ [5 Quay đầu / di chuyển tiếp: 3']
```
# Card #3: Thủ tục hành chính cho sinh viên/cựu sinh viên mất nhiều thời gian

HIỆN TẠI — 3 ngày (tính cả thời gian di chuyển & chờ xử lý)

[1 Tìm kiếm form mẫu / mục dịch vụ trên web cũ: 30'] → [2 Chuẩn bị giấy tờ & di chuyển đến trường: 60']
→ [3 Xếp hàng & nộp hồ sơ giấy tại phòng một cửa: 45'] → [4 Cán bộ tra cứu hồ sơ/bảng điểm lưu trữ thủ công: 2 ngày] ← BOTTLENECK
→ [5 Nhận kết quả (đến lấy trực tiếp hoặc chờ gửi bưu điện): 1 ngày]




### AI phản biện Card #1 (Google Maps sai đường):

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Người dùng cá nhân không thể trực tiếp sửa đổi cơ sở dữ liệu bản đồ cốt lõi | Đồng ý | Thu hẹp giải pháp sang cơ chế **"Cộng đồng report nhanh điểm rào chắn / thông luồng mới"** kết hợp thuật toán ưu tiên xác thực nhanh |
| Sai lệch chỉ đường có thể do mất tín hiệu GPS (vùng khuất cao ốc) chứ không hẳn do Maps update chậm | Đồng ý một phần | Bổ sung tiêu chí phân biệt lỗi do thiết bị/GPS vs lỗi do dữ liệu bản đồ vào danh sách giả định cần kiểm chứng ở CP4 |
| Gợi ý xây dựng tính năng AI tự động bẻ lái / đổi tuyến đột ngột | Không đồng ý | Giữ nguyên boundary: **"Cảnh báo nguy hiểm / Gợi ý lựa chọn, quyền quyết định cuối cùng thuộc về người lái"** để đảm bảo an toàn giao thông |

### AI phản biện Card #3 (Thủ tục cho sinh viên cũ lâu):

### AI phản biện Card #3 (Thủ tục cho sinh viên cũ lâu):

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì | 
| ----- | ----- | ----- | 
| Tệp cựu sinh viên có nhu cầu phát sinh không thường xuyên (tệp nhỏ, tần suất thấp) | Đồng ý | Mở rộng scope giải pháp: Xây dựng hệ thống Portal Dịch vụ 1 cửa online dùng chung cho **cả sinh viên hiện tại lẫn cựu sinh viên** để tối ưu chi phí vận hành | 
| Việc xác thực danh tính cựu sinh viên ra trường lâu dễ bị giả mạo thông tin | Đồng ý một phần | Đưa giả định về "xác thực danh tính qua VNeID / Căn cước công dân chip" vào danh sách điều cần kiểm chứng ở CP4 | 
| Gợi ý xây dựng chatbot tự động duyệt và ký số duyệt giấy xác nhận cho sinh viên | Không đồng ý | Giữ nguyên boundary: **"AI/Hệ thống hỗ trợ tra cứu và điền form tự động, cán bộ nhà trường kiểm tra và ấn nút duyệt cuối cùng"** để bảo đảm tính pháp lý | 


==> vì card 1 chưa tìm ra cách giải quyết củ thể, card 2 tốn thêm cơ sở vật chất nhiều và chỉnh sửa nhiều quy trình, card 3 gây mất thời gian nhất 

==> chọn card 3 xây dụng agent chat bot hỗ trợ cựu sinh viên làm thủ tục