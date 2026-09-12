# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Chung Văn Duy
- Mã học viên: 2A202602854
- Nhóm: Nhóm 3 thành viên (Nguyễn Hoàng Việt, Nguyễn Hải Hiếu, Chung Văn Duy)
- Candidate problem nhóm chọn: Vinmec: Đứt gãy luồng vận hành & Thất thoát thời gian chuyên môn của Bác sĩ lâm sàng do nhập liệu HIS và tra cứu mã ICD-10 thủ công.

---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| **Scan cá nhân** | Scan 10 bài toán thực tế bám sát hệ sinh thái Vingroup (VinFast, Xanh SM, VinBus, Vinhomes, Vinmec) với đầy đủ số liệu đo lường bằng phút, tần suất và tỷ lệ lỗi. | Đóng góp 3 bài toán vào pool chung của nhóm (#7 Trạm sạc Xanh SM, #8 Triage Vinmec, #9 Sự cố Vinhomes); mở đường cho việc hội tụ cụm y tế Vinmec với bạn Hoàng Việt. |
| **Pitch Problem Card** | Trình bày Problem Card #1 (Dự báo trạm sạc xe điện Xanh SM) với số liệu 50.000 tài xế, lãng phí 25–30 phút/ca, giảm 15–20% thu nhập; chỉ rõ nút thắt thiếu thông tin hàng đợi. | Giúp nhóm thấy rõ cấu trúc chuẩn của một Problem Card có số liệu và workflow Before/After; tạo tiền đề thảo luận về rào cản dữ liệu đóng IoT. |
| **Challenge bài của bạn khác** | - Challenge bài "Rà bài nộp repo GitHub" của bạn Hải Hiếu: Phân tích rằng 80–90% bài này chỉ cần viết Shell script/Linter (Rule-based), không cần đến AI, scope bài hẹp.<br>- Challenge bài "Vinmec gõ HIS" của bạn Hoàng Việt: Đặt câu hỏi về tiếng ồn phòng khám, nguy cơ ảo giác (hallucination) y khoa và trách nhiệm pháp lý nếu AI ghi sai đơn thuốc. | - Thuyết phục bạn Hiếu đồng thuận không chọn bài GitHub.<br>- Buộc bạn Việt phải thiết kế chốt chặn kiểm soát y đức bắt buộc (Human-in-the-loop: Bác sĩ bấm Confirm mới tạo hồ sơ pháp lý) và cơ chế Fallback quay lại gõ tay ngay lập tức. |
| **Gom trùng / cluster** | Cùng nhóm phân tích và gom 9 candidates thành 3 cụm (Cluster A: Y tế & Trợ lý hành chính chuyên môn; Cluster B: Vận hành giao thông xanh & Đô thị; Cluster C: Hỗ trợ học tập AI20k). | Nhận diện sự hội tụ tự nhiên ở Cluster A giữa bài Vinmec của bạn Việt (#1) và bài Vinmec của tôi (#8). |
| **Chọn candidate problem** | Tự phản biện lại bài trạm sạc xe điện của chính mình (nhận thấy nguy cơ Overengineering, thiếu quyền truy cập API trạm sạc VinFast/V-Green và nguy cơ "thundering herd"); chủ động đồng thuận dồn lực cho bài Vinmec của bạn Việt. | Giúp nhóm tránh sa vào bài toán vĩ mô không pilot được trong lab; đạt được 100% đồng thuận chọn đề tài Vinmec. |
| **Validation / research** | Tìm kiếm, khảo cứu và phân tích sâu các giải pháp Ambient Clinical AI trên thế giới (Abridge AI, Suki AI) và mô hình HIS tại Việt Nam (FPT.eHospital); đối chuẩn tính năng trích xuất SOAP Note và "Click-to-source". | Cung cấp bằng chứng công nghệ kiểm chứng được (auditable) cho mục 4.2 của nhóm, giúp nhóm định hình rõ "nên build gì / không build gì". |
| **Workflow nhóm** | Bóc tách chi tiết thời gian từng bước trong Current Workflow (bước 2 gõ HIS 3', bước 3 tra ICD-10 1'); đề xuất tích hợp Rule-based Order Sets vào Future Workflow để tối ưu thời gian. | Hoàn thiện sơ đồ Before (17') và After (10.5') với điểm nghẽn, handoff và fallback rõ ràng. |
| **Problem Statement** | Tham gia hoàn thiện 3 trường then chốt của PS v1: Bổ sung Success Metric định lượng (độ chính xác mã ICD-10 > 96%), siết chặt Boundary (những gì hệ thống KHÔNG ĐƯỢC LÀM) và định vị chính xác AI intervention point. | Giúp PS v1 đạt chuẩn chặt chẽ, khắc phục triệt để các điểm mơ hồ mà AI đã chỉ ra ở bản v0. |
| **Rule / Workflow / Agent** | Trả lời câu hỏi chốt số 1 và số 3; kiên quyết bác bỏ phương án Agent vì nguy cơ vi phạm y đức; bảo vệ phương án kiến trúc lai (Hybrid Workflow: Ambient AI + Rule-based Order Sets). | Nhóm thống nhất chọn mức Workflow, có lập luận so sánh sắc bén giữa No AI / Rule / Workflow / Agent. |
| **Decision** | Thiết kế kịch bản Pilot nhỏ nhất tại 5 phòng khám Khoa Nội và Khoa Nhi tại Vinmec Times City; xây dựng tiêu chí Exit/Rollback (dừng ngay nếu tỷ lệ sai thông tin y khoa chí mạng > 2%). | Đưa ra quyết định GO có cơ sở thực tế vững chắc, an toàn và thuyết phục. |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Dấu tay rõ nhất của tôi là việc kiên quyết kéo nhóm thoát khỏi bẫy "Agent tự động hóa viễn tưởng" để chốt chặn ranh giới kiểm soát y đức bắt buộc (Human-in-the-loop: Bác sĩ phải bấm duyệt mới tạo hồ sơ pháp lý), đồng thời đóng góp phần nghiên cứu đối chuẩn các giải pháp Ambient AI Scribe (Abridge, Suki AI) để chứng minh tính khả thi cho quyết định GO của nhóm.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| **Scan** | Mở rộng góc nhìn tìm kiếm bài toán quanh hệ sinh thái Vingroup. | Gợi ý các mảng hoạt động đa dạng (xe điện, bệnh viện, khu đô thị). | Đưa ra ý tưởng chung chung "xây chatbot tổng đài chăm sóc khách hàng toàn năng cho Vingroup", không có actor cụ thể, không chỉ ra được điểm nghẽn quy trình. | Bỏ hoàn toàn ý tưởng chatbot viển vông, tự đi sâu vào nỗi đau cụ thể của tài xế Xanh SM và bác sĩ Vinmec với số liệu đo lường bằng phút. |
| **Problem Card** | Đóng vai Skeptical PM phản biện Problem Card #1. | Chỉ ra rủi ro bài toán trạm sạc phụ thuộc vào dữ liệu nội bộ V-Green và hiện tượng "thundering herd". | AI gợi ý giải quyết bằng "Agent tự động đặt chỗ sạc" (vi phạm thực tế vì trụ sạc không có rào chắn cơ học). | Nhận diện đây là bẫy Overengineering; chuyển hướng tư duy sang Rule tính toán vật lý hoặc bài toán xử lý văn bản y tế có tính khả thi cao hơn. |
| **Workflow** | Gợi ý cú pháp Mermaid và sơ đồ hóa các bước khám bệnh Before/After. | Định dạng luồng Before/After trực quan, phân tách rõ các mốc thời gian và điểm nghẽn. | AI tự động hóa luôn cả bước kê đơn thuốc và gửi chỉ định xét nghiệm mà không có bước bác sĩ rà soát. | Thêm bước Human Boundary bắt buộc (Bác sĩ rà soát 30s và bấm Confirm) và cơ chế Fallback quay lại gõ tay khi AI lỗi. |
| **Research** | Tìm kiếm các case study và công cụ Ambient Clinical Intelligence trên thế giới. | Giới thiệu các sản phẩm hàng đầu như Nuance DAX Copilot, Abridge, Suki AI. | Cung cấp một số số liệu thống kê không kèm link kiểm chứng hoặc link dẫn đến trang 404. | Tự tay search Google, tìm trang chủ chính thức của Nuance DAX, Abridge và FPT.eHospital để lấy link kiểm chứng được và tóm tắt đúng điểm mạnh/khoảng trống. |
| **Problem Statement** | Phản biện bản Problem Statement v0 xem còn field nào mơ hồ. | Chỉ ra rất chuẩn xác rằng field `Boundary` của nhóm quá lỏng lẻo và `Success Metric` thiếu tiêu chí định lượng về độ chính xác y khoa. | AI tự viết lại một bản PS mới nhưng lại đưa thêm các tính năng chẩn đoán bệnh (Diagnosis AI) mà nhóm đã cấm. | Không copy bản AI viết, tự tay nhóm sửa lại v1 bằng cách siết chặt ranh giới "KHÔNG ĐƯỢC LÀM" (không tự kê đơn, không chẩn đoán thay bác sĩ). |
| **Rule / Workflow / Agent** | So sánh ưu nhược điểm của 3 mức độ công nghệ trên bài toán y tế. | Phân tích rõ sự khác biệt giữa Rule (Macros) và Generative AI (Ambient SOAP Note). | AI thiên vị việc dùng Autonomous Agent để "thể hiện công nghệ cao". | Cùng nhóm kiên quyết bác bỏ Agent, chốt chọn Workflow kết hợp Rule-based Order Sets vì lý do an toàn tính mạng người bệnh. |
| **Decision** | Gợi ý các tiêu chí đo lường cho giai đoạn Pilot. | Gợi ý chỉ số đo mức độ kiệt sức nghề nghiệp (Maslach Burnout Inventory). | Đề xuất pilot trên toàn bộ hệ thống bệnh viện Vinmec ngay lập tức (quá rủi ro). | Thu hẹp phạm vi pilot xuống quy mô tối thiểu an toàn: chỉ chạy tại 5 phòng khám Khoa Nội và Khoa Nhi tại Vinmec Times City trong 3 tháng. |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

**Reflection:**

```text
Trải nghiệm lớn nhất của tôi qua buổi lab Day 02 là bài học sâu sắc về việc chống lại cám dỗ "solution-first" và "cuồng Agent". Ban đầu, khi pitch bài toán trạm sạc xe điện Xanh SM, tôi từng nghĩ đây là một bài toán rất thời thượng, nhưng chính quá trình tự phản biện về chi phí hạ tầng và dữ liệu API đóng đã giúp tôi nhận ra nguy cơ overengineering nghiêm trọng nếu cố tình đưa AI vào một vấn đề vốn thuộc về giới hạn vật lý. Nhóm tôi cũng có lúc bị cuốn vào ý tưởng xây dựng một Agent y tế tự động ra y lệnh cho "ngầu", nhưng chúng tôi đã kịp thời phanh lại khi nhận thức được rủi ro chết người từ ảo giác AI (hallucination) trong môi trường bệnh viện. Khi chuyển sang đào sâu đề tài Vinmec cùng bạn Hoàng Việt, tôi học được rằng một giải pháp công nghệ xuất sắc không nằm ở việc dùng mô hình phức tạp nhất, mà nằm ở việc xác định ranh giới can thiệp (Boundary) chuẩn xác nhất. Dấu tay rõ nhất của tôi trong bản nộp nhóm là việc thiết kế chốt chặn kiểm soát y đức (Human-in-the-loop: Bác sĩ bấm duyệt) và khảo cứu các mô hình đối chuẩn Abridge/Suki để chứng minh tính khả thi của Ambient AI. Điều thách thức nhất đối với tôi khi viết Problem Statement không phải là metric thời gian, mà chính là ranh giới "KHÔNG LÀM" để bảo vệ tính mạng người bệnh trước sai số của máy móc. Tôi đã thay đổi hoàn toàn quan điểm từ việc tìm kiếm một bài toán "đao to búa lớn" sang việc tập trung giải phóng 3–5 phút gõ phím vô nghĩa cho bác sĩ, trả họ về đúng sứ mệnh lắng nghe bệnh nhân. Nếu được làm lại từ đầu, tôi sẽ challenge nhóm sớm hơn nữa ở khâu khảo sát thực địa để có thêm dữ liệu đo kiểm tiếng ồn âm học thực tế tại phòng khám. Sau buổi lab, tôi tự tin rằng mình đã nắm vững mạch tư duy đi từ nỗi đau có thật, qua phân tích luồng công việc, đến việc lựa chọn công nghệ phù hợp nhất thay vì chạy theo trào lưu.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI
