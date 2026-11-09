# Báo cáo cá nhân — Nguyễn Thế Cường (2A202603355)

## 1. Thông tin học viên

- Họ tên: Nguyễn Thế Cường.
- MSSV: 2A202603355.
- Tên nhóm: TVCL.
- Repo nhóm: [Repo nhóm TVCL](https://github.com/Him2K2/K5-L3-Day02-TVCL-DiscoveryProblemFraming).
- Đề tài nhóm: Phân loại và định tuyến phản ánh cư dân đến đúng bộ phận chuyên trách trên ứng dụng Vinhomes Resident.
- Phần việc phụ trách: CP5 — Quy trình trước/sau, bảng before/after và Problem Statement v0.
- Trạng thái quyết định: CP6 trong báo cáo nhóm chưa được hoàn thiện; chưa có quyết định Go / Not Yet / No-Go cuối cùng.

## 2. Scan problem (CP1)

Tôi liệt kê 10 vấn đề theo bốn góc nhìn: việc lặp lại, việc tốn thời gian, việc cần đọc/tổng hợp nhiều thông tin và khó khăn của người khác.

> Tôi chưa có số đo hoặc bằng chứng trực tiếp cho các dòng dưới đây. Các ô “cần đo” ghi thông tin cần thu thập, chưa phải kết quả quan sát.

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi đối soát một lô phiên sạc, tôi muốn tìm các phiên không khớp hóa đơn, để xử lý đúng giao dịch bị lệch | Nhân viên đối soát, bộ phận thanh toán | [Cần đo] … phút/lô; … phiên lệch trong … phiên kiểm tra |
| 2 | Lặp lại | Khi tiếp nhận phản ánh cư dân, tôi muốn biết bộ phận nào chịu trách nhiệm, để chuyển phản ánh đúng nơi ngay lần đầu | Nhân viên vận hành, cư dân, bộ phận tiếp nhận | [Cần đo] … phản ánh/ngày; … lần chuyển lại do sai bộ phận |
| 3 | Lặp lại | Khi nhận một lô video mới, tôi muốn biết frame nào thiếu hoặc sai nhãn biển báo và vạch làn, để sửa trước khi chạy đánh giá | Người gán nhãn, kỹ sư kiểm thử | [Cần đo] … phút kiểm tra/lô; … frame thiếu hoặc sai nhãn |
| 4 | Pain từ người khác | Khi tài xế thấy ghi chú điểm đón khác vị trí trên bản đồ, họ muốn xác định đúng nơi khách chờ, để tránh đi vòng và gọi lại nhiều lần | Tài xế, khách đặt xe | [Cần xác nhận với tài xế] … lần/tuần; … phút xác nhận lại/lần |
| 5 | Tốn thời gian | Khi kiểm thử nhận diện biển báo và vạch làn trên video, tôi muốn biết kết quả nào sai hoặc đến muộn, để chọn đúng lỗi cần cải thiện | Kỹ sư CV, kỹ sư kiểm thử | [Cần đo trên video thật] … lỗi/… frame; … phút kiểm tra/clip; p95 … ms |
| 6 | Tốn thời gian | Khi kết quả nhận diện trả về chậm, tôi muốn biết khâu nào mất nhiều thời gian nhất, để không thử tối ưu từng khâu một cách mò mẫm | Kỹ sư phát triển pipeline, kỹ sư kiểm thử | [Cần đo] … phút tìm nguyên nhân/lần; khâu chậm nhất … ms/frame |
| 7 | Cần đọc, tổng hợp nhiều thông tin | Khi so sánh các cấu hình nhận diện, tôi muốn xem chất lượng và độ trễ trong cùng một bảng, để chọn cấu hình phù hợp với mục tiêu kiểm thử | Kỹ sư CV, người review thử nghiệm | [Cần đo] … cấu hình/lần so sánh; … phút tổng hợp từ các log |
| 8 | Cần đọc, tổng hợp nhiều thông tin | Khi đọc một phiếu mô tả lỗi xe, tôi muốn xác định triệu chứng và bộ phận tiếp nhận, để tránh chuyển phiếu sai nhóm kỹ thuật | Nhân viên hỗ trợ, kỹ thuật viên tiếp nhận | [Cần đo] … giây/phiếu; …/… phiếu phải chuyển lại |
| 9 | Cần đọc, tổng hợp nhiều thông tin | Khi điểm đánh giá chung tốt nhưng vẫn có cảnh nhận sai, tôi muốn biết lỗi tập trung ở loại biển và điều kiện ảnh nào, để ưu tiên bổ sung đúng dữ liệu còn thiếu | Kỹ sư dữ liệu, kỹ sư CV | [Cần đo] … phút phân tích/đợt; … lỗi theo từng loại biển hoặc điều kiện ảnh |
| 10 | Pain từ người khác | Khi kỹ sư phát triển nhận báo cáo lỗi từ người kiểm thử, họ muốn tìm đúng video và cấu hình đã chạy, để tái hiện lỗi trước khi sửa | Kỹ sư phát triển, người kiểm thử bàn giao lỗi | [Cần xác nhận từ ticket] … phút tái hiện/lỗi; …/… ca thiếu video hoặc cấu hình |

**AI gợi ý thêm:** các ý #3, #6, #7, #9 và #10 được AI gợi ý bổ sung; các ý #1, #2, #4, #5 và #8 được lấy từ bài Lab2 Assignment ở lecture. Tôi giữ các gợi ý này để xem xét thêm, nhưng vẫn cần đối chiếu với trải nghiệm và bằng chứng thực tế. Hiện chưa đủ cơ sở xác nhận cả 10 vấn đề. Bốn frame synthetic trong bài cũ chỉ minh họa phép tính, không tính là dấu hiệu thật cho #5.

## 3. Top 3 Problem Cards (CP2)

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Nhận diện biển/vạch đúng, kịp thời | Phù hợp hướng quan tâm cá nhân ban đầu, có thể xác định cách đo | Dữ liệu, thiết bị, baseline, người dùng |
| 2 | Đối soát phiên sạc | Quy trình ghép dữ liệu rõ | Chưa có bảng phiên/hóa đơn |
| 3 | Phân loại mô tả lỗi | Có thể đối chiếu nhãn bộ phận | Chưa có phiếu và nhãn |

### Problem Card #1 — Nhận diện biển báo và hai vạch làn

| Trường | Nội dung |
|---|---|
| Job Story | Khi đánh giá video camera trước, tôi muốn biết kết quả biển/vạch đúng và kịp thời, để chọn hướng cải thiện |
| Actor | Kỹ sư phát triển và kiểm thử CV |
| Thời điểm / bối cảnh | Video ghi sẵn, đô thị ban ngày trời khô, một camera trước, nhóm biển khai báo |
| Quy trình hiện tại | Nhận frame → tiền xử lý → nhận diện → hậu xử lý → bộ phận nhận kết quả mô phỏng |
| Bottleneck | Bước nhận diện/hậu xử lý có thể sai; khâu gây trễ chưa đo, chưa kết luận |
| Impact | Sai/thiếu/muộn thông tin đầu vào của mô phỏng; chưa đo tác động vận hành |
| Success metric | Baseline thật chưa đo → precision ≥95%, recall đúng hạn mỗi loại ≥95%, đúng hai vạch ≥90%, p95 ≤100 ms; mục tiêu đề xuất |
| Phương án không dùng AI | Gán nhãn/kiểm thủ công để tạo tham chiếu; Rule tính điểm từ dự đoán, không thay toàn bộ nhận diện |
| Giả thuyết về AI | CV tạo dự đoán tại bước cố định; không cần Agent; Gemini không trực tiếp cải thiện nhận diện |
| Cảm nhận nhanh | Workflow cho CV, Rule cho đánh giá; cần dữ liệu trước khi chấp nhận |

```text
HIỆN TẠI — chưa có baseline độ trễ thực tế (đơn vị đo: ms/frame)

[1 Nhận frame và chờ hàng đợi: chưa đo] → [2 Tiền xử lý ảnh: chưa đo]
→ [3 Nhận diện biển báo và hai vạch làn: chưa đo] ← BOTTLENECK (giả định về chất lượng)
→ [4 Lọc và chuẩn hóa dự đoán: chưa đo] → [5 Trả kết quả mô phỏng: chưa đo]
```

Để có baseline, tôi cần ghi timestamp đầu/cuối từng khâu trên cùng thiết bị và cấu hình, gắn với mã frame; đo toàn tuyến bằng `available_ms − capture_ms`, gồm thời gian chờ. Báo số frame, precision/recall, tỷ lệ đúng hai vạch và p95 độ trễ; đối chiếu dự đoán với nhãn tham chiếu. Khâu gây trễ chưa xác định; không cộng trùng thời gian các nhánh song song. Hiện tôi chưa có video và log để điền thời gian từng bước.

### Problem Card #2 — Đối chiếu hóa đơn sạc

| Trường | Nội dung |
|---|---|
| Job Story | Khi đối soát phiên sạc, tôi muốn tìm dòng lệch hóa đơn, để xử lý đúng ca |
| Actor | Nhân viên đối soát |
| Thời điểm / bối cảnh | Đối soát theo lô, chưa có quan sát thực tế |
| Quy trình hiện tại | Nhận bảng → chuẩn hóa mã → ghép → kiểm lệch → chuyển ca |
| Bottleneck | Ghép và kiểm lệch, chưa đo phút/lô |
| Impact | Có thể bỏ sót lệch hoặc chậm xử lý, chưa kiểm chứng |
| Success metric | Baseline chưa đo → giảm ≥25% phút/lô và phát hiện ≥95% dòng lệch trên mẫu có nhãn, mục tiêu từ bài cũ |
| Phương án không dùng AI | Rule ghép khóa phiên và kiểm ngưỡng, nhân viên xử lý không khớp |
| Giả thuyết về AI | Chưa cần AI khi dữ liệu/logic ghép rõ |
| Cảm nhận nhanh | Rule |

```text
HIỆN TẠI — chưa có baseline thời gian thực tế (đơn vị đo: phút/lô)

[1 Nhận bảng phiên sạc và hóa đơn: chưa đo] → [2 Chuẩn hóa mã phiên: chưa đo]
→ [3 Ghép phiên với hóa đơn: chưa đo] → [4 Kiểm tra dòng lệch: chưa đo] ← BOTTLENECK (giả định)
→ [5 Chuyển ca chưa khớp: chưa đo]
```

Để có baseline, tôi cần bấm giờ từng bước trên một lô có số lượng phiên được ghi rõ; cộng thời gian thao tác để tính phút/lô và đối chiếu với nhãn giao dịch lệch do người phụ trách xác nhận. So sánh bước ghép phiên và bước kiểm lệch để xác định bottleneck. Hiện tôi chưa có bảng dữ liệu để đo; mức giảm 25% mới là mục tiêu đề xuất.

### Problem Card #3 — Phân loại mô tả lỗi xe

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận mô tả lỗi xe, tôi muốn xác định nhóm kỹ thuật phù hợp, để chuyển phiếu đúng nơi |
| Actor | Nhân viên hỗ trợ kỹ thuật |
| Thời điểm / bối cảnh | Phiếu mô tả tự do, chưa có dữ liệu thật |
| Quy trình hiện tại | Nhận phản ánh → đọc → gán nhóm → xác nhận → chuyển |
| Bottleneck | Đọc và phân loại triệu chứng; chưa đo giây/phiếu |
| Impact | Có thể chuyển sai hoặc chậm, cần kiểm chứng |
| Success metric | Baseline chưa đo → ≥90% gợi ý trùng nhãn và giảm ≥25% giây/phiếu, mục tiêu đề xuất |
| Phương án không dùng AI | Checklist triệu chứng, bảng phân tuyến, nhân viên gán nhóm |
| Giả thuyết về AI | Phân loại gợi ý từ nội dung; nhân viên duyệt; so với checklist trước |
| Cảm nhận nhanh | Workflow nếu lợi ích hơn Rule được chứng minh |

```text
HIỆN TẠI — chưa có baseline thời gian thực tế (đơn vị đo: phút/phiếu)

[1 Nhận phiếu: chưa đo] → [2 Đọc và xác định triệu chứng: chưa đo] ← BOTTLENECK (giả định)
→ [3 Gán nhóm kỹ thuật: chưa đo] → [4 Xác nhận phân loại: chưa đo]
→ [5 Chuyển phiếu: chưa đo]
```

Để có baseline, tôi cần ghi thời gian từng bước trên tập phiếu có nhãn bộ phận do người phụ trách xác nhận; tính giây/phiếu và tỷ lệ chuyển sai, bao gồm công kiểm tra/sửa. Ghi riêng phiếu thiếu thông tin hoặc có nhiều nhóm phù hợp. Hiện tôi chưa có phiếu thật để đo thời gian. Nếu báo bằng phút thì chia số giây cho 60.

### Card muốn pitch nhất

- **Card số:** 1 — Nhận diện biển báo và hai vạch biên làn.
- **Vì sao:** phù hợp hướng tôi quan tâm ban đầu và đã có quy trình để phân tích. Tôi vẫn cần dữ liệu thật để đánh giá; đây không phải đề tài cuối cùng nhóm chọn.
- **Câu hỏi muốn nhóm phản biện:** Chưa có log thật thì bằng chứng nào cho rằng suy luận là khâu gây trễ, thay vì hàng đợi hoặc hậu xử lý?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Bốn frame synthetic không chứng minh hiệu năng trên video thật | Đồng ý với nhận xét | Ghi baseline thật chưa đo; giữ dữ liệu mô phỏng ở phần minh họa |
| Chưa có log để quy lỗi độ trễ cho suy luận | Đồng ý với nhận xét | Đánh dấu bottleneck là giả định, giữ các bước riêng để đo |
| Gemini tạo báo cáo không trực tiếp cải thiện nhận diện ảnh | Đồng ý với nhận xét | Tách CV nhận diện và Rule tính điểm; nêu rõ giới hạn vai trò Gemini |
| Chưa có căn cứ cần Agent tự quyết các bước | Đồng ý với nhận xét | Giữ Workflow cho CV và Rule cho đánh giá trong card |

---
## 4. Tôi đã tham gia phần nào

Tôi phụ trách CP5 và đã đưa phần quy trình trước/sau, bảng so sánh và Problem Statement v0 vào mục 4–5 của [báo cáo nhóm](../team/group_report.md). Ba Problem Card ở mục 3 là các candidate cá nhân; phần CP5 thực hiện theo đề tài phản ánh cư dân của Trí mà nhóm đã chọn. Tôi đối chiếu nhật ký dưới đây với mục 2.1 của báo cáo nhóm và diễn đạt lại câu hỏi cho dễ đọc.

| Hoạt động | Tôi đã làm gì? | Kết quả |
|---|---|---|
| Pitch Problem Card | Trình bày ba candidate: kiểm thử nhận diện biển báo/vạch làn, đối soát phiên sạc và phân loại mô tả lỗi xe; ưu tiên bài nhận diện biển/vạch vì phù hợp chuyên môn | Theo báo cáo nhóm, bài nhận diện biển/vạch khó tiếp cận dữ liệu và kiểm chứng trong thời gian lab; tôi đồng thuận chọn bài phản ánh cư dân và phụ trách CP5 |
| Phản biện bài bạn khác | Hỏi Vũ về phương thức triển khai bài Google Maps; với bài thủ tục hành chính, hỏi tính khả thi khi tệp người dùng và tần suất sử dụng thấp | Mục 2.1 báo cáo nhóm ghi nhận hai câu hỏi của tôi; mục 2.4 nêu lý do không chọn bài thủ tục hành chính liên quan đến tần suất và quy trình ký duyệt. Báo cáo chưa ghi Vũ đã sửa card thế nào sau từng câu hỏi |
| Nhận phản biện — Card 1 | Liêm hỏi camera nhận dạng ban đêm có tốt không và AI có thực sự phát hiện, phản hồi nhanh hơn mắt thường không | Card hiện giới hạn video ban ngày trời khô, chưa tuyên bố hiệu năng ban đêm hay nhanh hơn con người; baseline chất lượng/độ trễ vẫn cần đo. Theo mục 2.4, tôi đồng thuận không chọn đề tài này do khó kiểm chứng trong thời gian lab |
| Nhận phản biện — Card 2 | Liêm hỏi triển khai đối soát phiên sạc có thực sự tạo thêm doanh thu không | Giữ mục tiêu đề xuất về thời gian đối soát và phát hiện dòng lệch; chưa khẳng định tăng doanh thu. Lợi ích tài chính cần dữ liệu về công xử lý và giao dịch lệch để đánh giá |
| Nhận phản biện — Card 3 | Liêm hỏi khi một triệu chứng có thể đến từ nhiều lỗi thì dựa vào tiêu chí nào để ưu tiên nơi chuyển phiếu | Card giữ checklist, bảng phân tuyến và nhân viên duyệt; chưa có quy tắc ưu tiên được xác nhận. Trường hợp nhiều nhóm phù hợp cần người phụ trách xác nhận, không để AI tự quyết |
| Cluster/OST/chọn candidate | Đối chiếu ba card cá nhân với các cluster trong báo cáo nhóm và đồng thuận chọn đề tài phản ánh cư dân | Card mô tả lỗi xe thuộc cluster Phân loại & Định tuyến; biển/vạch thuộc Giao thông & Thị giác máy tính; đối soát phiên sạc thuộc Vận hành nội bộ. CP5 được triển khai theo outcome giảm thời gian phản hồi và tỷ lệ chuyển sai |
| Kiểm chứng/research | Đối chiếu số liệu bài Trí với bản CP5 và đọc kết quả rà soát review được ghi trong báo cáo nhóm | Làm rõ baseline 4.5 phút/ticket cần xác minh, 12% chuyển sai là ước tính; ghi nhận phản ánh còn liên quan đến thẻ và tiện ích số. Tôi chưa có ghi chép về việc trực tiếp phỏng vấn hoặc thu thập review |
| Quy trình hiện tại (CP5) | Tổng hợp 5 bước tiếp nhận, đọc mô tả/ảnh, tra đơn vị, gán thông tin và lưu/chuyển; ghi actor, input, output và thời gian theo bài Trí | Mục 4.1 báo cáo nhóm; đánh dấu bước đọc mô tả/ảnh là bottleneck theo nguồn, chưa coi là kết quả đo mới |
| Quy trình tương lai (CP5) | Đề xuất 4 bước, phân biệt Rule, AI nếu cần thử và nhân viên duyệt; nêu boundary, nhánh ngoại lệ và cách quay về thủ công | Mục 4.2 báo cáo nhóm; 1.4 phút/ticket là ngân sách mục tiêu chưa thử nghiệm |
| Before/after (CP5) | So sánh số bước, thời gian, thao tác thủ công, bottleneck và rủi ro mới | Mục 4.3 báo cáo nhóm; phân biệt hiện trạng cần xác minh với kết quả kỳ vọng |
| Problem Statement v0 (CP5) | Tổng hợp 6 trường, baseline → target và cách đo; ghi các câu hỏi phản biện về dữ liệu, nguyên nhân gốc, ngoại lệ và sự cần thiết của AI | Mục 5 báo cáo nhóm; thời gian 4.5 phút/ticket và ước tính chuyển sai 12% vẫn cần xác minh. Mục 5.2 ghi nhóm đồng ý các phản biện; riêng sự cần thiết của AI là đồng ý với việc cần kiểm tra |
| Trình bày báo cáo CP5 | Tổng hợp quy trình, before/after, v0, cách đo và phản biện vào báo cáo chung | Mục 4.1–4.3 và mục 5; bản nhóm hiện có thêm mục 5.1 về cách đo và 5.2 về phản biện |
| Mức can thiệp/quyết định | Trong CP5, giữ biểu mẫu/danh mục/Rule làm đối chứng và AI là phương án chỉ thử nếu cần; tôi không phụ trách CP6 và chưa có kết quả cuối để ghi nhận | Mục 6–8 báo cáo nhóm còn trống; chưa có mức can thiệp, v1, đánh giá bốn rủi ro hoặc quyết định cuối được chốt |

## 5. Dùng AI

| Checkpoint | Dùng AI để làm gì? | Hữu ích ở đâu? | Sai/hời hợt ở đâu? | Tôi sửa gì |
|---|---|---|---|---|
| CP1 Scan | Bổ sung ý #3, #6, #7, #9, #10 và chỉnh Job Story | Gợi ý actor và cách đo cho từng vấn đề | Gợi ý chưa có bằng chứng từ trải nghiệm thật | Giữ #3, #6, #7, #9, #10 trong danh sách candidate để xem xét vì có actor và cách đo cụ thể; chưa coi là vấn đề đã kiểm chứng. Chỉ chọn ba card để phân tích sâu; các ý còn lại không được chọn, không có nghĩa đã chứng minh chúng không có giá trị. |
| CP2 Card | Phản biện và chuẩn hóa ba card, quy trình | Nêu thiếu baseline và nguy cơ nhầm synthetic với dữ liệu thật | Bản trước chưa thống nhất bảng và cách trình bày quy trình với bài mẫu | Đã tách số liệu mô phỏng, ghi bottleneck giả định; cần tự xác nhận nội dung cuối |
| CP4 Research | Hỗ trợ tìm tài liệu và lập khung kiểm chứng trong bản riêng | Có nguồn và câu hỏi để rà soát | Chưa thay thế việc tự mở nguồn và hỏi người thật | Đối chiếu kết quả review được ghi trong mục 3.2 báo cáo nhóm; không nhận là tôi trực tiếp phỏng vấn hoặc thu thập review. Review về chậm xử lý chưa chứng minh phân loại sai; chưa ghi công cụ hay hiệu quả AI là đã được xác minh. |
| CP5 Quy trình và before/after | Hỗ trợ chuyển bản CP5 được cung cấp vào mục 4 báo cáo nhóm, chuẩn hóa sơ đồ và bảng | Làm rõ actor/input/output, bước duyệt của con người, boundary và phương án quay về; phân biệt thời gian thao tác với thời gian chờ | Lần tổng hợp đầu thêm bảng và tiểu mục ngoài format yêu cầu; thời gian tương lai chưa có kết quả thử | Yêu cầu sửa lại đúng template; giữ 4.5 phút là số liệu nguồn cần xác minh và 1.4 phút là ngân sách mục tiêu |
| CP5 Problem Statement v0 | Hỗ trợ tổng hợp bản v0 có sẵn vào mục 5 và giữ lại câu hỏi phản biện | Làm rõ baseline → target, cách tính tỷ lệ chuyển sai và yêu cầu tính cả công duyệt/sửa | AI chưa xác minh phiếu quan sát và chưa chứng minh Rule không đủ | Giữ nhãn ước tính cho tỷ lệ 12%, mục tiêu dưới 3%; cập nhật rằng mục 5.2 báo cáo nhóm đã ghi ý kiến đồng ý, nhưng việc đồng ý phản biện không xác nhận baseline hoặc hiệu quả đã đạt |
| Ghi nhận đóng góp | Hỗ trợ cập nhật TEAM.md và báo cáo cá nhân từ bản CP5 đã cung cấp | Liên kết phần việc CP5 với sản phẩm ở mục 4–5 báo cáo nhóm | Không có căn cứ để điền thay hoạt động họp, phỏng vấn hoặc trải nghiệm cá nhân | Chỉ ghi sản phẩm đã có; để các sự kiện chưa xác nhận và reflection cho tôi tự bổ sung |
| CP6 Mức can thiệp/quyết định | Hỗ trợ so sánh phương án trong bản riêng | Làm rõ điều kiện thử Rule trước | Chưa có kết quả pilot hoặc đồng thuận nhóm | Phạm vi tôi phụ trách là CP5; phần so sánh chỉ là hỗ trợ bản nháp. Chưa xác nhận mức can thiệp hoặc quyết định cuối thay nhóm vì CP6 trong báo cáo chung chưa hoàn thiện. |
| Đồng bộ báo cáo cá nhân | Đối chiếu bản nhóm sau khi cập nhật main | Phát hiện nhật ký người hỏi và trạng thái phản biện CP5 đã thay đổi | Các câu hỏi do AI đề xuất trước đó không khớp bảng pitch thực tế | Thay bằng câu hỏi của Liêm và câu hỏi tôi đặt cho Vũ được ghi trong mục 2.1; giữ rõ CP6 chưa chốt |
| CP7 Reflection | Hỗ trợ soạn câu trả lời 6.1–6.7 và chỉnh giọng văn tự nhiên hơn | Tổng hợp bài cá nhân, phản biện của Liêm, phần CP5 và review trong báo cáo nhóm | Không biết cảm nhận cá nhân hoặc các sự kiện ngoài tài liệu; bản trước suy ra quan hệ trước/sau giữa phản biện và giới hạn ban ngày chưa có căn cứ | Đã yêu cầu đối chiếu báo cáo nhóm; bản sửa nêu giới hạn hiện có và bỏ suy diễn về thời điểm thay đổi. Việc tự xác nhận cảm nhận và viết lại bằng lời của tôi vẫn cần thực hiện |

---
## 6. Reflection (CP7)

Mục 6.1–6.6 tối thiểu 200 từ tổng cộng, không tính 6.7. Phần reflection có AI hỗ trợ soạn và chỉnh giọng văn từ nội dung bài; tôi cần tự xác nhận cảm nhận và sự kiện trước khi nộp.

**6.1. Tôi học được gì từ top 3 problems của các bạn khác?**

Đọc bài các bạn, tôi thấy mình ban đầu hơi tập trung vào chuyên môn CV nên ưu tiên bài nhận diện biển báo và vạch làn. Trong khi đó, bài Liêm và Trí cho thấy những việc quen thuộc như đọc tin nhắn, phân loại phản ánh hay tìm người phụ trách cũng có nhiều chỗ cần cải thiện. Bài Vũ khiến tôi chú ý hơn đến câu hỏi giải pháp sẽ triển khai thế nào và có được dùng thường xuyên không. Tôi nhận ra đề tài phù hợp còn cần dữ liệu, người dùng và cách kiểm chứng trong thời gian lab.

**6.2. Nhóm có lúc nào nghĩ giải pháp trước khi hiểu vấn đề? Đã xử lý ra sao?**

Có những lúc các đề xuất đã nhắc đến chatbot hoặc AI phân loại khá sớm. Khi làm CP5, tôi mới thấy việc đọc ticket lâu chưa chắc là do mô tả khó hiểu; có thể nhân viên đang phân vân vì trách nhiệm giữa các phòng ban chưa rõ. Tôi tách bước đọc nội dung và bước tra đơn vị để nhìn rõ hơn. Trong quy trình đề xuất, tôi cũng giữ hướng chuẩn hóa danh mục và thử Rule trước, thay vì mặc định phải dùng AI.

**6.3. Một lần tôi đổi ý sau phản biện: ai hỏi, hỏi gì, tôi sửa gì?**

Liêm hỏi bài nhận diện biển/vạch của tôi có hoạt động tốt vào ban đêm không, và AI có thực sự phản hồi nhanh hơn con người không. Tôi thấy mình chưa có dữ liệu để trả lời chắc chắn. Câu hỏi đó cho thấy phạm vi video ban ngày, trời khô trong card chưa đủ để kết luận về ban đêm hay so sánh tốc độ với con người; các chỉ số vẫn là mục tiêu cần đo. Sau khi nhóm trao đổi thêm về việc khó lấy dữ liệu và kiểm chứng trong buổi lab, tôi đồng ý chuyển sang bài phản ánh cư dân của Trí và nhận làm CP5.

**6.4. Kiểm chứng/research có điều gì làm tôi bất ngờ?**

Tôi chú ý đến việc các review trong báo cáo nhóm không chỉ nói về sự cố điện, nước mà còn nhắc đến thẻ xe, thẻ ra vào và tiện ích số. Nếu chỉ nhìn bài toán ban đầu, tôi dễ nghĩ danh mục phân loại chủ yếu dành cho hỏng hóc kỹ thuật. Tuy vậy, review về xử lý chậm cũng chưa cho biết chính xác chậm ở bước nào. Tôi thấy cần xem thêm dữ liệu vận hành trước khi kết luận rằng phân loại bằng AI sẽ giải quyết được vấn đề.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khó nhất với tôi là viết cho rõ mà không nói chắc hơn những gì mình biết. Chẳng hạn, 4.5 phút/ticket là số liệu lấy từ bài nguồn, còn 1.4 phút là thời gian đề xuất cho quy trình mới. Nếu trình bày không kỹ thì rất dễ khiến người đọc hiểu rằng nhóm đã đo và đạt kết quả đó. Tôi cũng phải chú ý tính cả thời gian nhân viên kiểm tra, sửa gợi ý và xử lý các ca khó, chứ không chỉ tính lúc công cụ chạy.

**6.6. Làm lại tôi sẽ đổi gì và phản biện mạnh hơn ở đâu?**

Nếu làm lại, tôi sẽ hỏi về nguồn số liệu sớm hơn: đo trên bao nhiêu ticket, có mấy người xử lý và có tính thời gian chờ không. Tôi cũng muốn làm rõ danh mục phòng ban trước khi vẽ quy trình tương lai. Khi trao đổi, tôi sẽ hỏi kỹ hơn liệu form hoặc Rule đã đủ chưa, và nếu thêm AI thì lợi ích có lớn hơn công kiểm tra, sửa lỗi hay không. Làm rõ những điểm đó từ đầu sẽ giúp phần CP5 bớt phải sửa lại.

**6.7. Tự giải thích 5–8 câu, không nhìn tài liệu: problem → quy trình → metric → boundary → mức can thiệp → quyết định.**

Nhóm tôi chọn bài phân loại và chuyển phản ánh cư dân đến đúng bộ phận trên ứng dụng Vinhomes Resident. Hiện nhân viên phải tiếp nhận, đọc mô tả và ảnh, tra đơn vị, gán thông tin rồi chuyển ticket. Bài nguồn ghi tổng thời gian là 4.5 phút/ticket, trong đó đọc nội dung mất 2 phút, nhưng nhóm vẫn cần xác minh cách đo và nguyên nhân gây chậm. Mục tiêu CP5 là dưới 1.5 phút/ticket và chuyển sai dưới 3%, có tính cả công duyệt, sửa và ghi riêng thời gian chờ. Nhân viên vẫn phải xác nhận trước khi chuyển; AI không được tự thêm thông tin, đổi ưu tiên hay đóng ticket. Hướng đề xuất là thử chuẩn hóa danh mục và Rule trước, chỉ cân nhắc AI khi cách đơn giản chưa đủ. CP6 trong báo cáo hiện chưa hoàn thiện nên nhóm chưa có quyết định cuối cùng về mức can thiệp và Go, Not Yet hay No-Go.

## 7. Tài liệu tham khảo

- [Báo cáo nhóm — Quy trình trước/sau (CP5)](../team/group_report.md#4-quy-trình-trướcsau-cp5): mục 4.1–4.3.
- [Báo cáo nhóm — Problem Statement v0 (CP5)](../team/group_report.md#5-problem-statement-v0-cp5): bảng v0 và phản biện.
- [TEAM.md — phần đóng góp cá nhân](../../TEAM.md#nguyenthecuong-2a202603355).
- [Báo cáo nhóm — Pitch và phản biện](../team/group_report.md#21-pitch): nguồn đối chiếu người hỏi và nội dung câu hỏi.
- [Báo cáo nhóm — Kiểm chứng](../team/group_report.md#32-kiểm-chứng): kết quả nhóm rà soát review công khai; không phải phỏng vấn do tôi thực hiện.
- [Worksheet](../../docs/01-worksheet.md): hướng dẫn cấu trúc Problem Card, CP5 và reflection.

**Nguồn nội dung gốc được dẫn lại:**

- *Lab2 Assignment* trong tài liệu lecture: nguồn các ý #1, #2, #4, #5 và #8 theo ghi chú CP1 và các mục tiêu ban đầu trong card. Chưa có bản tài liệu, thông tin tác giả hoặc URL được cung cấp trong repo; chưa thể tạo liên kết nguồn. Các số mô phỏng trong tài liệu không được dùng làm baseline thực tế.
- Hoàng Ngọc Minh Trí, *Báo cáo cá nhân — 2A202603379_HoangNgocMinhTri*, Card 1 về phân loại phản ánh cư dân và phần phản biện AI. Bản Markdown đã được cung cấp trong phiên làm việc dưới tên `2A202603379_HoangNgocMinhTri (1).md`, hiện chưa có trong repo. Đây là nguồn được CP5 kế thừa cho quy trình, 4.5 phút/ticket, 2 phút đọc mô tả/ảnh, khoảng 12% chuyển sai và 120 ticket/ca; chưa có phiếu quan sát gốc để xác minh độc lập.
- Nguyễn Thanh Liêm, *Báo cáo cá nhân — 2A202603358_NguyenThanhLiem*, và Hồ Xuân Vũ, *Báo cáo cá nhân — 03406_HoXuanVu*: tài liệu đối chiếu các candidate trong reflection. Các file cùng tên đã có trong thư mục cá nhân của repo: [bài Liêm](2A202603358_NguyenThanhLiem.md), [bài Vũ](03406_HoXuanVu.md).

Các đường dẫn báo cáo nhóm và TEAM.md ở trên là minh chứng sản phẩm/đóng góp; không thay thế nguồn dữ liệu gốc. Nhóm vẫn cần bổ sung bản nguồn hoặc đường dẫn của tài liệu lecture và bài Trí trước khi nộp.