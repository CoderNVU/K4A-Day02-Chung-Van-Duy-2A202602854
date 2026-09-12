# 02 — Group Problem Statement (Bản nộp nhóm)

> Làm chung 1 bản, mỗi thành viên copy vào repo cá nhân. Đi theo Phase 3 → 6 trong `01-worksheet.md`. Nhóm chỉ chọn **candidate problem** ở Phase 3, viết Problem Statement sau khi validate + vẽ workflow.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm |
|:---:|---|:---:|---|
| 1 | **Nguyễn Hoàng Việt** | 2A202602602 | **Workflow & Solution Lead**: Đề xuất candidate Vinmec, vẽ luồng Before/After, phân tích kiến trúc kỹ thuật và ranh giới an toàn |
| 2 | **Nguyễn Hải Hiếu** | 2A202602681 | **Evaluation & Rubric Lead**: Đề xuất candidate rà bài nộp GitHub, phản biện tiêu chí đo lường (metric), đối soát chất lượng bài làm |
| 3 | **Chung Văn Duy** | 2A202602854 | **Mobility & Smart Operations Lead**: Đề xuất candidate dự báo trạm sạc xe điện Xanh SM / VinFast, nghiên cứu công nghệ đối chuẩn (benchmark) và phân tích luồng vận hành trạm sạc |

**Candidate problem nhóm chọn (1 câu):**

Bác sĩ lâm sàng tại Vinmec mất từ 3–7 phút mỗi ca khám chỉ để tự gõ tóm tắt bệnh án vào phần mềm HIS và tra cứu mã ICD-10 thủ công, làm thời gian ca khám kéo dài lên 17 phút (vượt chuẩn 70%), gây dồn ứ dây chuyền tại sảnh chờ và gây kiệt sức nghề nghiệp (Doctor Burnout).

---

## Phase 3 — Group Convergence: từ 9-12 candidates về 1

### 3.1. Trình bày top 3 mỗi người (mỗi candidate 1-2 phút)

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---|---|---|---|---|---|
| 1 | Hoàng Việt | **Vinmec**: Bác sĩ mất 2–3h/ngày gõ bệnh án HIS & tra ICD-10 | Bác sĩ khám ngoại trú, bệnh nhân chờ | Gõ phím tự do trên HIS, tra mã bệnh thủ công | Bài toán rất nhức nhối, giá trị nhân văn cao, workflow y khoa rõ ràng. |
| 2 | Hoàng Việt | **VinFast**: Ngắt lốc lạnh cưỡng bức khi trời nắng gắt | Tài xế xe điện, kỹ sư R&D nhiệt | Firmware ngắt nhị phân On/Off khi áp gas tăng | Pain cực lớn ngoài thực tế, nhưng nghiêng về firmware nhúng, không cần AI. |
| 3 | Hoàng Việt | **Xanh SM**: Đứt gãy cung - cầu không đối xứng (Fleet Rebalancing) | Khách đặt xe, tài xế taxi điện | Dispatch thụ động, xe rỗng chạy mù quáng | Bài toán kinh điển ngành gọi xe, rất hấp dẫn nhưng scope dữ liệu quá lớn cho lab. |
| 4 | Hải Hiếu | **Lab AI20k**: Rà bài nộp đủ file và mục bắt buộc trước khi push | Học viên nộp bài, Trợ giảng chấm | Đọc lướt từng file bằng mắt tìm mục còn trống (chiếm 6–7/10–12') | Rất thực tế và gần gũi với học viên, đo đếm được ngay bằng phút và commit sửa lỗi. |
| 5 | Hải Hiếu | **Lab AI20k**: Câu hỏi lặp về cách nộp bài bị hỏi đi hỏi lại trong chat | Người hỏi (học viên vắng), 2-3 bạn hay trả lời | Mất thời gian tìm lại đoạn quy định trong tài liệu dài (3/4–5') | Pain có thật trong lớp (4–5 lần/tuần), nhưng giải quyết bằng FAQ ghim (No AI) là đã đủ 90%. |
| 6 | Hải Hiếu | **Lab AI20k**: Gom bài 3-4 thành viên thành một bản nộp nhóm thống nhất | Người ghép bài nhóm, cả nhóm chờ | Sửa định dạng và gỡ các ý trùng nhau thủ công (chiếm quá nửa 50–65') | Đau đầu vào lúc sát deadline; bước định dạng dùng template chung, bước gỡ trùng có thể dùng AI. |
| 7 | Văn Duy | **Xanh SM / VinFast**: Đề xuất trạm sạc tối ưu và dự báo hàng đợi theo thời gian thực | Tài xế Xanh SM, chủ xe VinFast khi pin < 25% | Thiếu dự báo thời gian chờ và trụ trống thực tế, tài xế di chuyển mù quáng và chờ 25–30' tại trạm | Điểm nghẽn vật lý rất rõ, ảnh hưởng trực tiếp đến thu nhập tài xế (-15–20%) và hiệu suất vận hành xe điện. |
| 8 | Văn Duy | **Vinmec**: Thu thập triệu chứng & phân loại ban đầu (Triage) qua Kiosk/App | Bệnh nhân ngoại trú, Bác sĩ khám lâm sàng | Bác sĩ mất 6–8' đầu ca hỏi lại tiền sử và gõ tay vào HIS; bệnh nhân chờ 45–60' ngoài sảnh | Cùng domain Vinmec với bài của Việt, bổ trợ tuyệt vời cho nhau (Duy: khâu tiếp đón/triage sảnh; Việt: khâu khám & ghi bệnh án phòng khám). |
| 9 | Văn Duy | **Vinhomes Resident**: Tự động phân loại và định tuyến phản ánh sự cố kỹ thuật | Cư dân khu đô thị, Ban Quản lý tòa nhà (Lễ tân/Kỹ thuật) | Đọc hiểu mô tả lộn xộn, gọi xác minh và phân loại gán task thủ công mất 4–6h/ngày | Bài toán CRM nội bộ hay nhưng scope hẹp trong tòa nhà, tác động nghiệp vụ không sâu sắc bằng y tế/giao thông. |

### 3.2. Gom trùng / cluster (gom 9-12 ý thành 3-4 cụm)

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| **A: Y tế & Trợ lý hành chính chuyên môn** | #1 (Vinmec HIS - Việt), #8 (Vinmec Triage - Duy) | Nhân sự chuyên môn cao (Bác sĩ) và bệnh nhân bị nghẽn ở khâu giao tiếp - nhập liệu hành chính (tiền sử, triệu chứng, bệnh án, ICD-10) do phần mềm HIS cứng nhắc và quy trình thủ công. | Sự hội tụ tự nhiên giữa 2 thành viên (Việt & Duy) cùng chọn hệ sinh thái Vinmec; tác động xã hội và giá trị y đức lớn nhất. |
| **B: Vận hành giao thông xanh & Đô thị thông minh** | #2 (VinFast ngắt lốc - Việt), #3 (Xanh SM điều phối xe - Việt), #7 (Xanh SM dự báo trạm sạc - Duy), #9 (Vinhomes phân loại sự cố - Duy) | Tối ưu hóa vận hành phương tiện xanh (xe điện, pin, trạm sạc) và điều phối nguồn lực đô thị thời gian thực. | Nghiêng về giải thuật điều khiển nhúng, Vận trù học (OR) và xử lý luồng dữ liệu IoT; phụ thuộc hạ tầng dữ liệu đóng của VinFast/Vingroup. |
| **C: Hỗ trợ học tập & Quy trình lớp học AI20k** | #4 (Rà bài nộp repo - Hiếu), #5 (FAQ nộp bài chat - Hiếu), #6 (Gom bài nhóm - Hiếu) | Các vấn đề lặp lại, tốn thời gian trong học tập, giao tiếp nhóm và quản trị bài nộp theo tiêu chuẩn. | Rất gần gũi với học viên; phần lớn giải quyết bằng Quy trình (Process/Template) hoặc Luật cứng (Rule-based/Linter). |

### 3.3. Shortlist (giữ 2-3 bài trả lời được 7 câu hỏi worksheet)

| Candidate | Vì sao vào shortlist (2-3 ý) | Rủi ro / điều chưa rõ |
|---|---|---|
| **1. Vinmec: Bác sĩ gõ bệnh án HIS & tra ICD-10** (Hoàng Việt pitch) | - Đối tượng chịu đau đớn rõ ràng (Bác sĩ, Bệnh nhân).<br>- Workflow khám lâm sàng 7 bước cực kỳ chuẩn hóa.<br>- Nút thắt gõ phím chiếm 30–40% thời gian ca khám, đo đếm được từng phút.<br>- Giải phóng thời gian giúp giải quyết vấn đề lớn về Doctor Burnout. | Nhận diện chính xác thuật ngữ y khoa chuyên sâu và từ ngữ địa phương trong môi trường phòng khám có tạp âm. |
| **2. Rà bài nộp repo GitHub trước khi push** (Hải Hiếu pitch) | - Workflow 5 bước rõ ràng, lặp lại đều đặn mỗi tuần cho cả lớp.<br>- Bottleneck đọc lướt tìm mục trống rất rõ, đo được bằng phút (10–12') và commit sửa lỗi.<br>- Cho phép so sánh sòng phẳng giữa Script Rule và AI kiểm tra nội dung. | 80–90% bài toán giải quyết được bằng Rule/Script linter; đất diễn cho AI khá nhỏ, checklist cứng dễ lỗi thời khi yêu cầu lab thay đổi. |
| **3. Đề xuất trạm sạc tối ưu và dự báo hàng đợi xe điện** (Văn Duy pitch) | - Nỗi đau vật lý hiện hữu của hơn 50,000 tài xế Xanh SM và chủ xe VinFast hàng ngày.<br>- Thành công đo được cụ thể bằng việc giảm thời gian chờ từ 25' xuống < 10'.<br>- Tăng trực tiếp 15% năng suất chạy xe của tài xế. | Dữ liệu trạng thái trụ sạc theo thời gian thực là dữ liệu nội bộ đóng của VinFast/V-Green, khó truy cập trong lab; nguy cơ trễ 2–3 phút gây dồn xe (thundering herd). |

### 3.4. Score để đồng thuận (chấm 1-5, ép nói rõ vì sao cho 5 / cho 3)

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **Vinmec: Bác sĩ gõ HIS** (Việt) | 5 | 5 | 5 | 5 | 5 | 5 | 4 | **34** |
| **Rà bài nộp repo GitHub** (Hiếu) | 5 | 5 | 4 | 4 | 5 | 3 | 5 | **31** |
| **Đề xuất trạm sạc xe điện** (Duy) | 4 | 4 | 5 | 5 | 3 | 4 | 4 | **29** |

**Candidate nhóm chọn (1 bài duy nhất):**

```text
Vinmec: Đứt gãy luồng vận hành & Thất thoát thời gian chuyên môn của Bác sĩ lâm sàng do nhập liệu HIS và tra cứu mã ICD-10 thủ công.
```

**Vì sao chọn (4-5 câu):**

```text
Nhóm chọn Vinmec vì đây là bài toán có nỗi đau thực tế sâu sắc và chạm đúng bản chất của việc ứng dụng AI: giải phóng con người khỏi các tác vụ nhập liệu máy móc để trả họ về đúng vai trò chuyên môn cao nhất. Luồng khám chữa bệnh ngoại trú 7 bước được chuẩn hóa rất cao tại các bệnh viện tiêu chuẩn quốc tế như Vinmec, giúp việc xác định nút thắt cổ chai và ranh giới an toàn (Safety Boundary) trở nên vô cùng rõ ràng. Giá trị tạo ra không chỉ tính bằng hàng trăm giờ làm việc tiết kiệm được mỗi ngày cho đội ngũ bác sĩ, mà còn trực tiếp nâng cao an toàn người bệnh và chỉ số hài lòng điều trị. Đồng thời, bài toán này cho phép nhóm so sánh đối chuẩn cực kỳ sắc nét giữa No AI (thư ký y khoa), Rule-based (Order Sets), Workflow và Agent AI.
```

**Vì sao KHÔNG chọn các candidate còn lại (mỗi bài 2-3 câu):**

```text
- Rà bài nộp repo GitHub (bài của Hiếu): Dù bài toán rất thực tế và gần gũi với lớp học, nhưng sau khi mổ xẻ kỹ thuật, nhóm nhận thấy 80-90% bài toán được giải quyết trọn vẹn bằng một script shell/linter kiểm tra heading và file structure (Rule-based thuần túy). Phần việc của AI chỉ là kiểm tra xem nội dung có quá sơ sài hay không, không đủ độ phức tạp về workflow, tích hợp hệ thống và ranh giới an toàn để đại diện cho đề tài nhóm.
- Đề xuất trạm sạc tối ưu xe điện (bài của Duy): Bài toán phụ thuộc sống còn vào luồng dữ liệu cảm biến IoT thời gian thực từ mạng lưới trụ sạc VinFast/V-Green, vốn là dữ liệu bảo mật nội bộ mà nhóm không có quyền truy cập API để kiểm chứng trong lab. Ngoài ra, việc can thiệp giữ chỗ (slot booking) cứng là không khả thi nếu thiếu rào chắn vật lý tại trụ sạc hoặc chính sách phạt no-show; rủi ro dữ liệu trễ 2-3 phút có thể gây hiện tượng "thundering herd" (nhiều xe cùng đổ dồn về 1 trạm vắng vừa gợi ý), tạo ra nút thắt cổ chai mới nghiêm trọng hơn.
```

**Disagreement (nếu có — ai lo gì, chốt ra sao):**

```text
Ban đầu, bạn Hải Hiếu muốn nhóm chọn bài "Rà bài nộp GitHub" vì dữ liệu có sẵn ngay trong lớp và có thể đo lường kiểm chứng ngay lập tức. Tuy nhiên, bạn Hoàng Việt và Chung Văn Duy đã challenge rằng bài của Hiếu thiên về Rule-based script (Linter), không phô diễn được toàn diện năng lực thiết kế hệ thống AI của nhóm trong Day 02 Lab. Bạn Chung Văn Duy đưa ra bài toán "Trạm sạc xe điện Xanh SM" rất hấp dẫn, nhưng cả nhóm cùng nhận thấy rào cản truy cập API nội bộ đóng của V-Green và bài toán giữ chỗ vật lý chưa khả thi trong khuôn khổ lab. Đáng chú ý, cả Duy và Việt đều cùng đề xuất bài toán trong hệ sinh thái Vinmec (Duy làm Triage sảnh tiếp đón, Việt làm Bác sĩ gõ HIS phòng khám). Nhóm nhận thấy điểm nghẽn tại khâu bác sĩ khám lâm sàng của Việt là nút thắt chí mạng nhất, mang lại giá trị nhân văn và ROI cao nhất. Bạn Hiếu lo ngại về rủi ro sai sót y khoa và tiếng ồn phòng khám. Bạn Hoàng Việt đã thuyết phục thành công cả nhóm bằng thiết kế kiến trúc Workflow với chốt chặn kiểm duyệt y đức bắt buộc (Human-in-the-loop: Bác sĩ phải bấm duyệt mới tạo hồ sơ pháp lý) và cơ chế Fallback quay về gõ tay ngay lập tức nếu AI gặp lỗi. Cả nhóm 100% đồng thuận chọn đề tài Vinmec của bạn Việt.
```

---

## Phase 4 — Quick Validation + Research

### 4.1. Quick validation (ít nhất 1 cách: interview 2-3 người hoặc survey 5-10 người)

Nhóm đã thực hiện phỏng vấn nhanh 3 Bác sĩ lâm sàng đang công tác tại các cơ sở y tế và thực hiện khảo sát nhanh qua Google Forms/Zalo với 8 nhân sự y tế.

| Nguồn | Số người / mẫu | Tín hiệu xác nhận (kèm quote nguyên văn) | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| **Phỏng vấn Bác sĩ Nội trú BV Đa khoa** | 1 | *"Nhiều lúc tôi cảm giác mình là thư ký văn phòng chứ không phải bác sĩ. Ngồi khám 1 ca mà mắt nhìn màn hình 6 phút, nhìn bệnh nhân được 2 phút. Gõ xong bệnh sử rồi lại bấm chuột mỏi tay chọn từng xét nghiệm máu, mệt nhất là nhớ mã ICD-10."* | Có những ca bệnh phức tạp, bệnh nhân kể chuyện lan man, bác sĩ vẫn phải chủ động lọc ý. | Xác định rõ AI chỉ ghi nhận các dữ liệu y khoa trọng yếu theo cấu trúc SOAP Note, không chép nguyên văn hội thoại thừa. |
| **Phỏng vấn Bác sĩ Nhi - Vinmec** | 1 | *"Khám Nhi thì áp lực vô cùng vì các cháu quấy khóc, bố mẹ sốt ruột. Vừa dỗ trẻ vừa phải xoay lưng gõ phím máy tính làm phụ huynh rất khó chịu. Nếu có công cụ tự động nghe rồi điền sẵn vào HIS thì cứu cánh cho chúng tôi."* | Bác sĩ lo ngại tiếng khóc của trẻ em hoặc tiếng bố mẹ nói xen vào làm AI nhận diện sai thông tin. | Bổ sung yêu cầu kỹ thuật về Microphone định hướng lọc tạp âm và tính năng phân tách giọng nói (Diarization). |
| **Phỏng vấn Bác sĩ Đa khoa Phòng khám** | 1 | *"Hệ thống HIS hiện tại click quá nhiều bước. Để chỉ định một bộ xét nghiệm sốt xuất huyết phải click chuột 7 lần qua 3 tầng menu. Rất ức chế vào giờ cao điểm."* | Bác sĩ quen tay với một số mã bệnh phổ biến nên gõ cũng khá nhanh (khoảng 30 giây cho mã quen). | Kết hợp giải pháp Rule-based Order Sets (gói chỉ định 1 click) vào giao diện để hỗ trợ song song với AI. |
| **Khảo sát nhanh qua Mini Poll** | 8 nhân sự y tế | - 7/8 người (87.5%) đánh giá việc nhập liệu HIS là khâu gây ức chế nhất trong ca khám.<br>- 100% khẳng định thời gian chờ đợi của bệnh nhân phần lớn do thời gian bác sĩ gõ máy tính.<br>- 8/8 người mong muốn có trợ lý giọng nói điền sẵn bệnh án. | 2 người lo lắng nếu hệ thống AI bị đơ/lag thì họ không biết làm thế nào để kịp giờ khám. | Thiết kế cơ chế Fallback mượt mà: Bác sĩ luôn có thể quay lại gõ tay truyền thống ngay lập tức mà không bị khóa phần mềm. |

**Insight sau validation (1-2 câu — pain thật nằm ở đâu):**

```text
Nỗi đau thật không nằm ở chuyên môn chẩn đoán của bác sĩ, mà nằm ở "thời gian chết hành chính": sự đứt gãy giữa ngôn ngữ giao tiếp tự nhiên trong phòng khám với giao diện nhập liệu dạng form cứng nhắc của hệ thống HIS, biến bác sĩ thành nhân viên nhập liệu bất đắc dĩ.
```

Bằng chứng đính kèm (nếu có): `02-group-problem-statement-interview-notes.md`

### 4.2. Research giải pháp đã có (ít nhất 2-3 tools/patterns + 1-2 link kiểm được)

Nhóm đã khảo cứu các giải pháp Trợ lý y khoa giọng nói (Ambient Clinical Intelligence) tiên tiến trên thế giới và hiện trạng các hệ thống HIS tại Việt Nam:

| Nguồn / tool / case | Link kiểm chứng | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Nuance DAX Copilot (Microsoft)** | [Nuance DAX Copilot](https://www.nuance.com/healthcare/ambient-clinical-intelligence.html) | Lắng nghe hội thoại phòng khám $\rightarrow$ Tự động tạo bản nháp bệnh án lâm sàng trực tiếp trên Epic EHR. | - Tích hợp sâu vào hệ thống EHR hàng đầu thế giới.<br>- Tiết kiệm trung bình 7 phút/ca khám.<br>- 70% bác sĩ giảm cảm giác kiệt sức (burnout). | - Chi phí bản quyền cực kỳ đắt đỏ.<br>- Tối ưu hóa cho tiếng Anh y khoa tại Mỹ, chưa hỗ trợ tốt tiếng Việt y tế. | Mô hình "Ambient Listening $\rightarrow$ Draft SOAP Note $\rightarrow$ Doctor Review & Sign" là mẫu hình chuẩn mực toàn cầu. |
| **Abridge AI** | [Abridge Clinical Documentation](https://www.abridge.com/) | Dùng Generative AI chuyển hội thoại lâm sàng thành tài liệu có cấu trúc, tự động link từng câu chữ về đoạn ghi âm gốc (Auditable). | - Tính minh bạch dữ liệu cực cao (Click vào câu văn xem lại đoạn ghi âm gốc).<br>- Tự động trích xuất mã thanh toán BHYT (ICD-10/CPT). | - Đòi hỏi hạ tầng Cloud bảo mật y tế nghiêm ngặt.<br>- Nguy cơ trích xuất sót các tiền sử bệnh nhân nói lướt qua. | Phải có tính năng "Click-to-source" để bác sĩ đối soát nhanh đoạn âm thanh nếu nghi ngờ AI ghi nhầm. |
| **Suki AI Assistant** | [Suki Assistant](https://www.suki.ai/) | Trợ lý ảo ra lệnh giọng nói kiêm ghi chú lâm sàng cho bác sĩ đa chuyên khoa. | - Linh hoạt giữa Ambient Mode (nghe thụ động) và Voice Command (ra lệnh chỉ định cận lâm sàng bằng miệng). | - Bác sĩ vẫn phải nhớ câu lệnh mẫu nếu dùng chế độ Command.<br>- Phụ thuộc kết nối mạng Internet. | Kết hợp giữa Ambient AI (tóm tắt bệnh án) và Rule-based Macro (gói chỉ định sẵn) giúp tối ưu tốc độ tối đa. |
| **Hệ thống HIS nội bộ (FPT.eHospital / Viettel HIS)** | [FPT.eHospital Solution](https://fpt-is.com/ehospital/) | Quản lý tổng thể bệnh viện, lưu trữ EHR, thanh toán viện phí và BHYT. | - Đáp ứng chuẩn danh mục và thông tư của Bộ Y tế Việt Nam.<br>- Ổn định, kết nối trực tiếp cổng dữ liệu BHYT quốc gia. | - Hoàn toàn không có năng lực AI/Voice.<br>- Giao diện dạng lưới (grid) nhiều click chuột, trải nghiệm người dùng lạc hậu. | Không cần đập bỏ HIS hiện có; xây dựng giải pháp AI dưới dạng Plugin/Extension tích hợp qua API/WebSocket vào HIS. |

**Research takeaway (2-3 câu — nên build gì / không build gì):**

```text
Nhóm KHÔNG tự xây dựng một hệ sinh thái quản lý bệnh viện (HIS/EHR) mới, và tuyệt đối KHÔNG xây dựng AI Agent tự chẩn đoán bệnh. Hướng đi đúng đắn nhất là xây dựng một "Lớp giải pháp Ambient AI Scribe" đóng vai trò cầu nối thông minh: thu âm hội thoại tự nhiên $\rightarrow$ mô hình AI chuyên ngành trích xuất cấu trúc SOAP Note và gợi ý mã ICD-10 $\rightarrow$ đẩy trực tiếp vào các trường dữ liệu của HIS Vinmec để bác sĩ kiểm tra và bấm duyệt trong 30 giây.
```

---

## Phase 5 — Workflow + Problem Statement

### 5.1. Current workflow bản nhóm

Dán workflow hoặc link file: `02-group-problem-statement-workflow.md`

```text
[1 Khám & Hỏi bệnh: 4' - Bác sĩ] 
→ [2 Gõ bệnh sử vào HIS: 3' - Bác sĩ] (BOTTLENECK CHÍNH)
→ [3 Tra cứu mã ICD-10: 1' - Bác sĩ] (BOTTLENECK PHỤ)
→ [4 Click chọn cận lâm sàng: 2' - Bác sĩ]
→ [5 In phiếu chỉ định & Điều dưỡng hướng dẫn: 1' - Handoff]
→ [6 Đọc kết quả CLS & Gõ chẩn đoán xác định: 3' - Bác sĩ]
→ [7 Kê đơn thuốc & Dặn dò: 3' - Bác sĩ]
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú (handoff? bottleneck?) |
|:---:|---|---|---|:---:|---|
| **1** | Bác sĩ & Bệnh nhân | Lời kể triệu chứng, thẻ khám bệnh | Thông tin bệnh sử sơ bộ, ghi nhận thực thể | 4 phút / Mỗi ca khám | Giao tiếp đối thoại trực tiếp. |
| **2** | Bác sĩ | Trí nhớ của bác sĩ về lời kể bệnh nhân | Đoạn văn bản text tóm tắt trên phần mềm HIS | **3 phút / Mỗi ca khám** | **BOTTLENECK CHÍNH**: Bác sĩ vừa nghĩ vừa gõ phím, mắt nhìn màn hình, ngừng giao tiếp với bệnh nhân. |
| **3** | Bác sĩ | Tên bệnh lý suy luận lâm sàng | Mã bệnh chuẩn ICD-10 (VD: J00, A09) | **1 phút / Mỗi ca khám** | **BOTTLENECK PHỤ**: Phải gõ từ khóa tìm kiếm trong danh mục hàng nghìn mã bệnh, dễ nhầm mã. |
| **4** | Bác sĩ | Quyết định cận lâm sàng | Danh sách xét nghiệm, X-quang được tick chọn | 2 phút / Mỗi ca khám | Thao tác chuột phân mảnh, phải mở nhiều cây thư mục xét nghiệm. |
| **5** | Bác sĩ $\rightarrow$ Điều dưỡng | Phiếu chỉ định in từ máy in | Bệnh nhân cầm phiếu di chuyển đi làm xét nghiệm | 1 phút / Mỗi ca khám | Điểm bàn giao (Handoff) giữa Bác sĩ và Điều dưỡng tiếp đón. |
| **6** | Bác sĩ | Kết quả xét nghiệm/X-quang từ hệ thống PACS/LIS | Kết luận chẩn đoán xác định gõ vào HIS | 3 phút / Sau khi có CLS | Bác sĩ tổng hợp dữ liệu cận lâm sàng và gõ giải thích bệnh. |
| **7** | Bác sĩ | Danh mục thuốc điều trị | Đơn thuốc điện tử đã ký + dặn dò bệnh nhân | 3 phút / Kết thúc ca khám | In đơn thuốc, hướng dẫn liều dùng và hẹn ngày tái khám. |

**Bottleneck chính (2-3 câu):**

```text
Điểm nghẽn nghiêm trọng nhất nằm ở Bước 2 và Bước 3 (chiếm tổng cộng 4–5 phút): Bác sĩ bị ngắt quãng tư duy chuyên môn để thực hiện việc chuyển dịch thủ công từ lời nói tự nhiên của bệnh nhân sang các ô nhập liệu của phần mềm HIS và tra cứu mã ICD-10. Đây là công việc thuần túy mang tính thủ thư/hành chính nhưng lại lấy đi hơn 30% tổng thời gian tiếp xúc quý báu giữa bác sĩ và người bệnh.
```

### 5.2. Future workflow bản nhóm

Phải nhìn ra 5 thứ: bước nào máy (Rule), bước nào AI, bước nào người, boundary ở đâu, fallback khi AI sai.

```text
[1 Khám & Hội thoại tự nhiên: 4' - Người] (Ambient Mic ngầm ghi âm)
→ [2 AI chuyển âm thanh thành SOAP Note + Gợi ý ICD-10: 0.5' - Máy/AI]
→ [3 Rule-based Order Sets tự động gắn gói cận lâm sàng: 0.2' - Máy/Rule]
→ [4 Bác sĩ rà soát bản nháp & Bấm DUYỆT (Confirm): 0.5' - BOUNDARY KIỂM SOÁT Y ĐỨC]
→ [5 In phiếu tự động & Hướng dẫn: 0.8' - Điều dưỡng]
→ [6 Đọc kết quả CLS, duyệt đơn thuốc gợi ý & Dặn dò: 4.5' - Bác sĩ & Bệnh nhân]

Fallback: Nếu Micro lỗi, mất mạng hoặc AI trích xuất sai lệch -> Bác sĩ bấm nút "Bỏ qua bản nháp", hệ thống lập tức mở lại màn hình gõ phím HIS truyền thống để bác sĩ nhập liệu tay bình thường.
```

**Before/after impact:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| **Tổng thời gian ca khám** | 17 phút | **10.5 phút** | Bấm giờ tự động từ lúc bệnh nhân vào phòng đến khi in đơn ra về trên HIS |
| **Thời gian nhập liệu hành chính** | 4 – 5 phút | **< 1 phút** | Đo thời gian tương tác bàn phím/chuột của bác sĩ trên các trường bệnh án |
| **Số thao tác click chuột / gõ phím** | ~120 ký tự + 25 clicks | **1 click xác nhận** | Log hành vi thao tác người dùng (Telemetry/Keylogger trên máy trạm HIS) |
| **Độ chính xác mã hóa ICD-10** | ~82% (hay bị xuất toán BHYT) | **> 96%** | Tỷ lệ hồ sơ bệnh án được phòng Kế hoạch tổng hợp & BHYT thẩm định hợp lệ lần đầu |
| **Tỷ lệ ca khám trễ hẹn dây chuyền** | 40% | **< 10%** | Thống kê độ lệch giữa giờ hẹn trên App Vinmec và giờ bắt đầu khám thực tế |
| **Risk mới phát sinh** | Không có rủi ro công nghệ mới | Nguy cơ AI nghe nhầm / ảo giác | Rà soát 100% bản nháp: Bác sĩ phải bấm Confirm mới sinh hồ sơ pháp lý |

### 5.3. Problem Statement v0 (mỗi field 2-3 câu)

| Field | Nội dung |
|---|---|
| **Actor** | Bác sĩ lâm sàng khám ngoại trú tại Bệnh viện Đa khoa Quốc tế Vinmec và các bệnh nhân đến khám bệnh. |
| **Workflow** | Bác sĩ đón bệnh nhân, khám thực thể, tự tay gõ tóm tắt bệnh sử vào HIS, tra cứu mã ICD-10, click chọn danh mục xét nghiệm, in phiếu chỉ định và kê đơn thuốc. |
| **Bottleneck** | Thao tác gõ phím tóm tắt bệnh sử tự do và tra cứu danh mục mã bệnh ICD-10 thủ công trên giao diện HIS rất phân mảnh và tốn thời gian. |
| **Impact** | Mỗi ca khám mất tới 17 phút, bác sĩ lãng phí 2–3 tiếng/ngày chỉ để gõ máy, phòng khám dồn ứ bệnh nhân và bác sĩ bị căng thẳng kiệt sức. |
| **Success Metric** | Giảm thời gian nhập liệu xuống dưới 1 phút/ca; rút ngắn thời gian khám từ 17 phút xuống dưới 11 phút; tăng sự hài lòng của bác sĩ và bệnh nhân. |
| **Boundary** | AI chỉ hỗ trợ ghi chép bản nháp; bác sĩ phải kiểm tra trước khi gửi; không tự ý gửi dữ liệu ra bên ngoài internet công cộng. |

**Câu hỏi AI phản biện v0 (nếu có):**
- Field nào mơ hồ: AI chỉ ra rằng: (1) `Boundary` viết quá chung chung, chưa nói rõ trách nhiệm pháp lý nếu đơn thuốc có sai sót thuộc về ai; (2) `Success Metric` chưa có tiêu chí định lượng về độ chính xác của văn bản y khoa trích xuất và cách thức đối soát lỗi; (3) Điểm can thiệp của AI (AI intervention point) chưa được định vị chính xác nằm trước hay sau bước khám thực thể.
- Tôi sửa gì: Nhóm đã tiếp thu và sửa đổi trực tiếp vào bản Problem Statement v1: Quy định rõ ranh giới pháp lý tuyệt đối thuộc về Bác sĩ; bổ sung metric về tỷ lệ chính xác mã ICD-10 (> 96%); định vị chính xác điểm can thiệp AI là lắng nghe thụ động (Ambient) trong suốt bước 1 và kết xuất bản nháp trước bước 4.

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp (suy nghĩ nhanh, không thay quyết định cuối)

- Độ mơ hồ: [ ] Thấp / [x] **Cao** — Vì sao: Ngôn ngữ hội thoại tự nhiên giữa bác sĩ và bệnh nhân vô cùng phong phú, chứa nhiều khẩu ngữ địa phương, tiếng lóng triệu chứng ("nóng trong người", "tức ngực ran ran", "ngạt mũi thở khò khè"). Không có một cấu trúc cố định nào cho cuộc đối thoại lâm sàng.
- Độ phức tạp: [ ] Thấp / [x] **Cao** — Vì sao: Quy trình đòi hỏi xử lý đa phương thức (Âm thanh $\rightarrow$ Văn bản $\rightarrow$ Cấu trúc hóa SOAP Note), đồng thời phải đối chiếu chuẩn hóa vào bảng danh mục hàng chục nghìn mã bệnh ICD-10 và kết nối dữ liệu trực tiếp với hệ sinh thái HIS/PACS/LIS của bệnh viện.

**Bài toán nhóm nằm ở ô nào:**

```text
Ô: Độ mơ hồ cao — Độ phức tạp cao (Góc trên bên phải của Ma trận phù hợp AI).
```

**Vì sao (2-3 câu):**

```text
Bài toán đòi hỏi năng lực hiểu ngôn ngữ tự nhiên sâu sắc trong ngữ cảnh hội thoại y khoa phức tạp (Độ mơ hồ cao) và cần tích hợp nhiều tầng dữ liệu chuyên ngành từ âm thanh tới mã hóa hệ thống HIS bệnh viện (Độ phức tạp cao). Tuy nhiên, vì đây là lĩnh vực y tế liên quan trực tiếp đến tính mạng con người, hệ thống không thể vận hành theo cơ chế tự chủ hoàn toàn của AI Agent, mà bắt buộc phải tổ chức dưới dạng một Workflow điều phối chặt chẽ với sự kiểm duyệt của con người (Human-in-the-loop).
```

### 6.1. So sánh Rule / Workflow / Agent (so trên cùng 1 bài)

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? (Dùng cho bước nào?) |
|---|---|---|---|:---:|
| **Rule** | Thiết lập các mẫu bệnh án sẵn (Macros/Templates) và Gói chỉ định cận lâm sàng (Order Sets: click 1 nút chọn cả bộ sốt xuất huyết/viêm họng) trên giao diện HIS. | Đủ cho các ca bệnh cực kỳ điển hình, đơn giản hoặc bước tích chọn danh mục cận lâm sàng/thuốc theo phác đồ cứng. | Không giải quyết được khâu tóm tắt bệnh sử tự do phong phú của từng cá nhân; bác sĩ vẫn phải sửa tay rất nhiều. | **CHỌN (Dùng phối hợp)**: Áp dụng Rule-based cho khâu Order Sets chỉ định cận lâm sàng chuẩn. |
| **Workflow** | **Hệ thống Ambient Clinical Voice Workflow**: Micro thu âm ngầm $\rightarrow$ AI lọc nhiễu, chuyển ngữ (STT) $\rightarrow$ LLM trích xuất SOAP Note & map mã ICD-10 $\rightarrow$ Gợi ý Order Sets $\rightarrow$ Bác sĩ rà soát 30s và bấm DUYỆT (Confirm) $\rightarrow$ Đẩy vào HIS. | Rất phù hợp vì luồng khám bệnh đi theo các bước rõ ràng; AI đóng vai trò công cụ đắc lực giải quyết phần ngôn ngữ phức tạp, còn con người giữ quyền quyết định. | Rủi ro nhận diện sai từ chuyên môn hoặc chậm trễ đường truyền. Kiểm soát được hoàn toàn nhờ bước bác sĩ rà soát và xác nhận. | **CHỌN LÀM GIẢI PHÁP CHÍNH**: Đây là điểm cân bằng hoàn hảo giữa tự động hóa và an toàn y đức. |
| **Agent** | Một Tác tử AI tự động lắng nghe, tự động suy luận chẩn đoán, tự động gửi lệnh xét nghiệm xuống phòng lab và tự phát lệnh in đơn thuốc cho bệnh nhân mà không cần bác sĩ bấm duyệt. | Chỉ có thể áp dụng trong môi trường giả định tương lai khi AI được cấp chứng chỉ hành nghề y khoa độc lập. | **CỰC KỲ NGUY HIỂM**: Ảo giác (hallucination) có thể gây ra y lệnh sai lệch làm chết người; vi phạm nghiêm trọng Luật Khám chữa bệnh và đạo đức ngành y. | **LOẠI BỎ HOÀN TOÀN**: Tuyệt đối không trao quyền tự quyết y lệnh cho AI. |

**5 câu hỏi chốt (trả lời câu đầy đủ):**
1. *Rule có giải được 70-80% case không?* $\rightarrow$ **Không.** Rule chỉ giải quyết được việc tích chọn các gói xét nghiệm mẫu, hoàn toàn bất lực trong việc lắng nghe và tóm tắt diễn biến bệnh sử phong phú của từng bệnh nhân.
2. *Các bước có đi thẳng một đường không hay phải rẽ nhánh?* $\rightarrow$ **Đi thẳng một đường có điều kiện:** Luồng thông tin đi tuần tự từ Hội thoại $\rightarrow$ Ghi nhận $\rightarrow$ Cấu trúc hóa $\rightarrow$ Bác sĩ duyệt $\rightarrow$ Lưu trữ; nhánh rẽ duy nhất là trường hợp Bác sĩ phát hiện thông tin sai và kích hoạt chế độ chỉnh sửa tay.
3. *Có thật sự cần Agent tự lập kế hoạch + gọi tool không?* $\rightarrow$ **Không cần và không được phép.** Bác sĩ là người lập kế hoạch điều trị duy nhất; AI chỉ đóng vai trò trợ lý thư ký ghi chép văn bản.
4. *Nếu AI sai, ai phát hiện đầu tiên và sửa trong bao lâu?* $\rightarrow$ **Bác sĩ phát hiện đầu tiên** ngay tại bước hiển thị bản nháp trên màn hình, và chỉ mất từ **5–15 giây** để bấm chuột chỉnh sửa hoặc gõ lại từ đúng trước khi bấm nút xác nhận.
5. *Có hạ được từ Agent → Workflow → Rule không?* $\rightarrow$ **Được.** Giải pháp của nhóm đã chủ động hạ từ Agent xuống **Workflow kết hợp Ambient AI**, và phần chỉ định danh mục được hạ tiếp xuống **Rule-based Order Sets** để đảm bảo tính tất định và an toàn tối đa.

**Mức chọn:**

```text
Workflow (Kiến trúc Hybrid: Workflow điều phối tích hợp Ambient Clinical Voice AI + Rule-based Order Sets).
```

**Vì sao chọn (3-4 câu):**

```text
Nhóm chọn Workflow vì đây là phương án tối ưu hóa trọn vẹn giá trị công nghệ mà vẫn giữ vững 100% ranh giới an toàn y đức. AI xử lý xuất sắc khâu chuyển hóa ngôn ngữ tự nhiên thành văn bản SOAP Note có cấu trúc (điểm nghẽn lớn nhất của bác sĩ), trong khi Rule-based xử lý chuẩn xác khâu gắn mã cận lâm sàng theo phác đồ. Luồng công việc tuyến tính, minh bạch, có điểm dừng cưỡng bức (Human Boundary) để bác sĩ kiểm soát chất lượng trước khi tạo ra bất kỳ chứng từ y khoa có giá trị pháp lý nào.
```

**Vì sao không chọn mức đơn giản hơn (2-3 câu):**

```text
Nếu chỉ dùng No AI hoặc Rule-based đơn thuần (như tạo form mẫu hay tuyển thư ký gõ máy), chúng ta không giải quyết được gốc rễ của vấn đề: Bác sĩ vẫn phải tự tay gõ phím điều chỉnh từng chi tiết bệnh án, hoặc bệnh viện phải tốn chi phí quỹ lương khổng lồ mà vẫn đối mặt với rủi ro rò rỉ quyền riêng tư của người bệnh. Chỉ có năng lực xử lý ngôn ngữ tự nhiên của AI mới xóa bỏ được thao tác gõ bàn phím thủ công này.
```

### 6.2. Problem Statement v1 (v0 sửa chặt hơn + 3 field cuối)

| Field | Nội dung |
|---|---|
| **Actor** | Bác sĩ lâm sàng khám ngoại trú (Nội tổng quát, Nhi, Tai Mũi Họng) tại Bệnh viện Đa khoa Quốc tế Vinmec và Bệnh nhân đến thăm khám. |
| **Workflow** | Bác sĩ khám và đối thoại với bệnh nhân $\rightarrow$ Ambient Microphone ngầm thu âm $\rightarrow$ AI tự động trích xuất SOAP Note và đề xuất mã ICD-10 + Order Sets $\rightarrow$ Bác sĩ rà soát 30 giây và bấm DUYỆT $\rightarrow$ In chỉ định cận lâm sàng $\rightarrow$ Bác sĩ đọc kết quả, duyệt đơn thuốc và dặn dò. |
| **Bottleneck** | Nút thắt tại khâu bác sĩ tự gõ phím tóm tắt bệnh sử tự do vào HIS và tra cứu mã ICD-10 thủ công (mất 4–5 phút/ca), khiến thời gian khám kéo dài lên 17 phút và phân tán sự chú ý của bác sĩ khỏi người bệnh. |
| **Impact** | Lãng phí 2–3 giờ/ngày/bác sĩ cho việc gõ máy; 40% ca khám hẹn giờ bị trễ dây chuyền; sảnh chờ quá tải; bác sĩ kiệt sức nghề nghiệp (burnout); gia tăng nguy cơ xuất toán bảo hiểm do mã hóa sai ICD-10. |
| **Success Metric** | (1) Giảm thời gian nhập liệu hành chính từ 4–5 phút xuống < 1 phút/ca khám;<br>(2) Rút ngắn tổng thời gian ca khám từ 17 phút xuống còn 10.5 phút;<br>(3) Trả lại 1.5 – 2.0 giờ/ngày cho bác sĩ tập trung chuyên môn;<br>(4) Tỷ lệ chính xác gợi ý mã ICD-10 đạt > 96%. |
| **Boundary** (làm / không làm) | **LÀM**: Tự động thu âm hội thoại, chuyển đổi giọng nói thành văn bản SOAP Note, gợi ý mã ICD-10 và đề xuất gói Order Sets lên màn hình chờ duyệt.<br>**KHÔNG LÀM**: Tuyệt đối không tự động phát lệnh cận lâm sàng, không tự động ký đơn thuốc, không tự động đưa ra kết luận chẩn đoán thay bác sĩ, không lưu trữ âm thanh thô chưa mã hóa ra ngoài mạng nội bộ. |
| **AI intervention point** | Can thiệp ngầm ngay trong lúc Bác sĩ và Bệnh nhân giao tiếp (Bước 1), kết xuất dữ liệu bản nháp hoàn tất ngay khi cuộc thăm khám thực thể kết thúc, hiển thị sẵn trên màn hình HIS trước Bước bác sĩ ra chỉ định cận lâm sàng. |
| **Mức chọn** | **Workflow** (Workflow tích hợp Ambient Clinical AI + Rule-based Order Sets): Đảm bảo tự động hóa tối đa phần ghi chép mà vẫn giữ nguyên luồng vận hành y khoa kiểm soát nghiêm ngặt. |
| **Rủi ro & người thật kiểm tra** | **Rủi ro**: AI nghe nhầm thuật ngữ y khoa đặc thù, hiểu sai triệu chứng do tiếng ồn/tiếng khóc trẻ nhỏ, hoặc sinh ảo giác (hallucination).<br>**Người thật kiểm tra**: Bác sĩ điều trị là chốt chặn pháp lý duy nhất (Human-in-the-loop); bắt buộc phải liếc mắt rà soát bản nháp và tự tay bấm nút DUYỆT (Confirm) thì hệ thống mới đẩy dữ liệu vào hồ sơ bệnh án chính thức. |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
|---|:---:|---|
| Actor + workflow rõ chưa? | **Yes** | Bác sĩ khám ngoại trú và luồng khám bệnh 7 bước chuẩn y khoa đã được phân tích chi tiết. |
| Baseline + metric đo được chưa? | **Yes** | Baseline rõ ràng: 17 phút/ca, 4–5 phút gõ phím; Metric mục tiêu: 10.5 phút/ca, < 1 phút gõ phím, đo bằng telemetry HIS. |
| Data/input đủ dùng chưa? | **Yes** | Cuộc hội thoại trực tiếp hàng ngày tại phòng khám là nguồn dữ liệu dồi dào; danh mục ICD-10 và bệnh án mẫu có sẵn trên HIS Vinmec. |
| AI sai, hậu quả chấp nhận được không? | **Yes** | Hậu quả hoàn toàn kiểm soát được vì AI chỉ đóng vai trò tạo bản nháp (Draft), Bác sĩ phải duyệt mới có hiệu lực pháp lý. |
| Có người review/owner không? | **Yes** | Bác sĩ trực tiếp khám là người review tại chỗ; Trưởng khoa lâm sàng và Giám đốc Y khoa là Owner vận hành. |
| Có cách non-AI đơn giản hơn không? | **No** | Cách non-AI (thuê thư ký gõ máy) quá tốn kém và vi phạm riêng tư; cách dùng mẫu form gõ sẵn không giải quyết được tính cá thể hóa của bệnh án. |

**Decision:**

```text
GO (Triển khai Thử nghiệm Lâm sàng có Kiểm soát - Pilot Phase).
```

**Lý do (3-4 câu dựa trên bằng chứng):**

```text
Nhóm quyết định GO vì bài toán đáp ứng trọn vẹn cả 6 tiêu chí thẩm định: Vấn đề có thật và gây nhức nhối hàng ngày cho đội ngũ y bác sĩ; giá trị mang lại đo lường được bằng số giờ cụ thể và doanh thu khám bệnh tăng thêm; công nghệ Ambient Clinical Voice AI trên thế giới đã được kiểm chứng thành công tại các hệ thống y tế lớn (như Nuance DAX tại Mỹ); và quan trọng nhất là rủi ro y tế được triệt tiêu nhờ cơ chế kiểm duyệt cưỡng bức Human-in-the-loop của Bác sĩ.
```

**Nếu Go — pilot nhỏ nhất (data nào, chạy tay ra sao, đo 3 số nào):**

```text
- Phạm vi Pilot: Thử nghiệm trong 3 tháng tại 5 phòng khám ngoại trú thuộc Khoa Nội tổng quát và Khoa Nhi tại Bệnh viện Đa khoa Quốc tế Vinmec Times City.
- Cách chạy thử: Lắp đặt micro định hướng chuyên dụng; hệ thống Ambient AI chạy song song ghi nhận và hiển thị bản nháp SOAP Note trên một cửa sổ pop-up nổi cạnh phần mềm HIS; Bác sĩ dùng thử và bấm nút copy dữ liệu vào HIS.
- Đo lường 3 chỉ số cốt lõi:
  1. Thời gian nhập liệu trung bình của bác sĩ trên mỗi ca khám (Mục tiêu: giảm từ 4.5 phút xuống < 1 phút).
  2. Tỷ lệ bản nháp SOAP Note được bác sĩ chấp thuận mà không cần chỉnh sửa quá 20% nội dung (Mục tiêu: đạt > 85%).
  3. Chỉ số giảm căng thẳng và kiệt sức nghề nghiệp của bác sĩ tham gia thử nghiệm (Đo bằng thang đo Maslach Burnout Inventory trước và sau pilot).
```

**Nếu Not Yet — cần validate gì trước:**

```text
(Không áp dụng vì nhóm quyết định GO). Tuy nhiên, trước ngày bấm nút pilot 2 tuần, cần kiểm tra đo kiểm thực địa về độ ồn decibel trong phòng khám và khả năng bắt âm khi bệnh nhân đeo khẩu trang y tế.
```

**Nếu No-Go — làm gì thay AI:**

```text
(Không áp dụng vì nhóm quyết định GO). Nếu trong tương lai phải dừng AI, giải pháp thay thế tối ưu là chuẩn hóa lại giao diện phần mềm HIS bằng việc áp dụng 100% Rule-based Order Sets và phím tắt thông minh (Smart Macros) để giảm bớt số cú click chuột.
```

**Exit / rollback (khi nào dừng AI, quay về cách cũ):**

```text
Hệ thống sẽ lập tức dừng thử nghiệm và kích hoạt cơ chế Rollback quay về quy trình cũ nếu xảy ra một trong hai điều kiện sau:
1. Tỷ lệ nhận diện sai lệch các thông tin y khoa chí mạng (như tiền sử dị ứng thuốc, liều lượng dùng thuốc) vượt quá 2% số ca khám trong tuần đầu tiên mà không được bác sĩ phát hiện kịp thời;
2. Thời gian bác sĩ phải đọc lại và sửa lỗi văn bản nháp của AI kéo dài trung bình vượt quá 2 phút/ca (khiến việc dùng AI còn chậm hơn cả tự gõ tay truyền thống) trong 2 tuần liên tiếp.
```

---

### Self-check nộp phần 02 (nhóm)
- [x] Có nhật ký hội tụ 9-12 → 1 (cluster + shortlist + score)
- [x] Có validation (quote thật) + research (link kiểm được)
- [x] Có workflow trước/sau đủ thời gian, handoff, bottleneck, boundary, fallback
- [x] Có PS v0 → v1, metric có trước/sau + cách đo, boundary có làm/không làm
- [x] Có so sánh Rule/Workflow/Agent + Decision Go/Not Yet/No-Go có lý do
