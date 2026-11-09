# Báo cáo cá nhân 

## 1. Thông tin học viên

- Họ tên: **[Nguyen The Cuong]**.
- MSSV: **[2A202603355]**.
- Tên nhóm: **[TVCL]**.
- Repo nhóm: **[https://github.com/Him2K2/K5-L3-Day02-TVCL-DiscoveryProblemFraming]**.

## 2. Scan problem (CP1)

Scan 10 vấn đề theo bốn lăng kính: lặp lại, tốn thời gian, cần đọc/tổng hợp nhiều thông tin và pain từ người khác.

> Cột “Dấu hiệu thật” là chỗ điền bằng chứng thực tế. Các ô `[cần đo]` chưa phải kết quả quan sát; không dùng số liệu mô phỏng để thay thế.

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

**AI gợi ý thêm:** các ý #3, #6, #7, #9 và #10 được AI gợi ý bổ sung; các ý #1, #2, #4, #5 và #8 chuyển từ [bài scan cũ](../assets/cp1-source-problem-scan.md). Học viên cần xác nhận ý giữ/bỏ theo trải nghiệm thật. Chưa có bằng chứng để khẳng định cả 10 vấn đề đều đã xảy ra. Bốn frame synthetic trong bài cũ chỉ minh họa phép tính, không tính là dấu hiệu thật cho #5.

## 3. Top 3 Problem Cards và quy trình nháp (CP2)

| Rank đề xuất | Problem | Vì sao | Điều chưa chắc |
|---:|---|---|---|
| 1 | Nhận diện biển/vạch đúng, kịp thời | Đúng hướng đề tài, đã có định nghĩa metric | Dữ liệu, thiết bị, baseline, người dùng |
| 2 | Đối soát phiên sạc | Quy trình ghép dữ liệu rõ | Chưa có bảng phiên/hóa đơn |
| 3 | Phân loại mô tả lỗi | Có thể đối chiếu nhãn bộ phận | Chưa có phiếu và nhãn |

### Card 1 — Nhận diện biển báo và hai vạch làn

| Trường | Nội dung |
|---|---|
| Job Story | Khi đánh giá video camera trước, tôi muốn biết kết quả biển/vạch đúng và kịp thời, để chọn hướng cải thiện |
| Actor | Kỹ sư phát triển và kiểm thử CV |
| Bối cảnh | Video ghi sẵn, đô thị ban ngày trời khô, một camera trước, nhóm biển khai báo |
| Quy trình | Nhận frame → tiền xử lý → nhận diện → hậu xử lý → đầu nhận mô phỏng |
| Bottleneck | Bước nhận diện/hậu xử lý có thể sai; khâu gây trễ chưa đo, chưa kết luận |
| Impact | Sai/thiếu/muộn thông tin đầu vào của mô phỏng; chưa đo tác động vận hành |
| Metric | Baseline thật chưa đo → precision ≥95%, recall đúng hạn mỗi loại ≥95%, đúng hai vạch ≥90%, p95 ≤100 ms; mục tiêu đề xuất |
| Không dùng AI | Gán nhãn/kiểm thủ công để tạo tham chiếu; Rule tính điểm từ dự đoán, không thay toàn bộ nhận diện |
| Giả thuyết AI | CV tạo dự đoán tại bước cố định; không cần Agent; Gemini không trực tiếp cải thiện nhận diện |
| Cảm nhận nhanh | Workflow cho CV, Rule cho đánh giá; cần dữ liệu trước khi chấp nhận |

```text
[Nhận frame/hàng đợi: chưa đo] → [Tiền xử lý: chưa đo]
→ [Nhận diện: chưa đo, nghi vấn lỗi chất lượng]
→ [Hậu xử lý: chưa đo] → [Trả kết quả: chưa đo]
Đo toàn tuyến = available_ms − capture_ms (gồm chờ).
```

### Card 2 — Đối chiếu hóa đơn sạc

| Trường | Nội dung |
|---|---|
| Job Story | Khi đối soát phiên sạc, tôi muốn tìm dòng lệch hóa đơn, để xử lý đúng ca |
| Actor | Nhân viên đối soát |
| Bối cảnh | Đối soát theo lô, chưa có quan sát thực tế |
| Quy trình | Nhận bảng → chuẩn hóa mã → ghép → kiểm lệch → chuyển ca |
| Bottleneck | Ghép và kiểm lệch, chưa đo phút/lô |
| Impact | Có thể bỏ sót lệch hoặc chậm xử lý, chưa kiểm chứng |
| Metric | Baseline chưa đo → giảm ≥25% phút/lô và phát hiện ≥95% dòng lệch trên mẫu có nhãn, mục tiêu từ bài cũ |
| Không dùng AI | Rule ghép khóa phiên và kiểm ngưỡng, nhân viên xử lý không khớp |
| Giả thuyết AI | Chưa cần AI khi dữ liệu/logic ghép rõ |
| Cảm nhận nhanh | Rule |

```text
[Nhận bảng: ? phút] → [Chuẩn hóa: ? phút] → [Ghép: ? phút]
→ [Kiểm lệch: ? phút, nghi vấn nghẽn] → [Chuyển ca: ? phút]
? = chưa đo, cần ghi thời gian thật.
```

### Card 3 — Phân loại mô tả lỗi xe

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận mô tả lỗi xe, tôi muốn xác định nhóm kỹ thuật phù hợp, để chuyển phiếu đúng nơi |
| Actor | Nhân viên hỗ trợ kỹ thuật |
| Bối cảnh | Phiếu mô tả tự do, chưa có dữ liệu thật |
| Quy trình | Nhận phản ánh → đọc → gán nhóm → xác nhận → chuyển |
| Bottleneck | Đọc và phân loại triệu chứng; chưa đo giây/phiếu |
| Impact | Có thể chuyển sai hoặc chậm, cần kiểm chứng |
| Metric | Baseline chưa đo → ≥90% gợi ý trùng nhãn và giảm ≥25% giây/phiếu, mục tiêu đề xuất |
| Không dùng AI | Checklist triệu chứng, bảng phân tuyến, nhân viên gán nhóm |
| Giả thuyết AI | Phân loại gợi ý từ nội dung; nhân viên duyệt; so với checklist trước |
| Cảm nhận nhanh | Workflow nếu lợi ích hơn Rule được chứng minh |

```text
[Nhận: ? giây] → [Đọc: ? giây, nghi vấn nghẽn]
→ [Gán nhóm: ? giây] → [Xác nhận: ? giây] → [Chuyển: ? giây]
? = chưa đo. Có thể đổi sang phút khi ghi báo cáo chính thức.
```

### Card đề xuất pitch

- Card 1, đúng ý tưởng người học lựa chọn.
- Câu hỏi chuẩn bị: Chưa có log thật thì bằng chứng nào cho rằng suy luận là khâu gây trễ, thay vì hàng đợi hoặc hậu xử lý?
- Chưa xác nhận học viên đã pitch câu hỏi này.

### Phản biện AI trong lần chuyển thể

| Điểm yếu trợ lý nêu | Đề xuất sửa trong bản nháp | Học viên xác nhận |
|---|---|---|
| Số synthetic dễ bị hiểu thành baseline | Tách synthetic và chưa đo thật | Chưa xác nhận |
| Đồng nhất nhận diện với báo cáo Gemini | Đặt CV ở nhánh nhận diện, LLM chỉ offline tùy chọn | Chưa xác nhận |
| Khẳng định nghẽn inference khi chưa profile | Chỉ ghi giả thuyết, đo từng khâu | Chưa xác nhận |
| Đặt metric mà thiếu số mẫu và quyền dữ liệu | Bổ sung điều kiện cần chốt trước pilot | Chưa xác nhận |

## 4. Tôi đã tham gia phần nào (CP3-CP6)

**Học viên tự ghi sự kiện thật**, không nhận nội dung trợ lý soạn thành đóng góp họp nhóm đã thực hiện.

| Hoạt động | Tôi đã làm gì? | Kết quả/bằng chứng |
|---|---|---|
| Pitch | [CẦN ĐIỀN] | |
| Phản biện bạn khác | Câu hỏi thật: [CẦN ĐIỀN] | |
| Nhận phản biện | Ai hỏi/câu hỏi thật: [CẦN ĐIỀN] | Thay đổi thực tế: |
| Cluster/OST/chọn candidate | [CẦN ĐIỀN] | |
| Kiểm chứng/research | [CẦN ĐIỀN] | |
| Quy trình/Problem Statement | [CẦN ĐIỀN] | |
| Mức can thiệp/quyết định | [CẦN ĐIỀN] | |

## 5. Dùng AI

| Phạm vi hỗ trợ lần này | AI đã làm | Giới hạn cần học viên kiểm tra |
|---|---|---|
| CP1–2 | Chuyển bài nguồn thành Job Story/card, bổ sung 5 candidate #6–#10 theo cách trình bày bài mẫu và nêu điểm yếu | Chưa có bằng chứng pain thật cho các gợi ý; cần tự xác nhận, ghi ý giữ/bỏ và sửa theo trải nghiệm |
| CP3 | Lập khung và phân tích tài liệu | Không thay pitch/challenge hoặc điểm do nhóm chấm |
| CP4 | Mở 3 nguồn chính thức, soạn kế hoạch hỏi | Chưa phỏng vấn; thành viên phải tự đọc nguồn |
| CP5–6 | Soạn dự thảo quy trình, statement, metric và quyết định từ bài cũ | Nhóm cần tự rà soát/chốt; chưa đo hay kiểm lại code/log cũ |
| CP7 | Để câu hỏi tự ghi | Không có reflection được viết thay |

Học viên bổ sung nhật ký AI trước đó, chỗ AI sai/hời hợt thực tế và cách mình đã sửa. Không tự nhận các đề xuất ở trên là trải nghiệm đã xảy ra.

## 6. Reflection (CP7) — học viên tự viết

Mục 6.1–6.6 tối thiểu 200 từ tổng cộng, không tính 6.7. Hiện chưa có nội dung trả lời.

**6.1.** Tôi học được gì từ top 3 problems của các bạn khác?

**6.2.** Nhóm có lúc nào nghĩ giải pháp trước khi hiểu vấn đề? Đã xử lý ra sao?

**6.3.** Một lần tôi đổi ý sau phản biện: ai hỏi, hỏi gì, tôi sửa gì?

**6.4.** Kiểm chứng/research có điều gì làm tôi bất ngờ?

**6.5.** Điều khó nhất khi viết Problem Statement là gì?

**6.6.** Làm lại tôi sẽ đổi gì và phản biện mạnh hơn ở đâu?

**6.7.** Tự giải thích 5–8 câu, không nhìn tài liệu: problem → quy trình → metric → boundary → mức can thiệp → quyết định.

## 7. Tài liệu tham khảo

- [Scan nguồn](../assets/cp1-source-problem-scan.md), [deep-dive nguồn](../assets/cp5-source-deep-dive.md).
- [Báo cáo nhóm dự thảo](../team/group_report.md), gồm nguồn research và quy tắc metric.
