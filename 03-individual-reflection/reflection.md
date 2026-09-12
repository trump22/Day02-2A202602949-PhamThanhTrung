# 03 — Individual Reflection



## Thông tin cá nhân

- **Họ và tên:** Phạm Thành Trung
- **Mã học viên:** 2A202602949
- **Nhóm:** DDGPT
- **Candidate problem nhóm chọn:** Bác sĩ lâm sàng Vinmec mất 30-40% thời gian làm việc để tự gõ hồ sơ bệnh án (EMR) sau mỗi lượt khám.

---

## 1. Tôi đã tham gia vào phần nào?

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Quét 25 problem bằng 4 lăng kính, lọc ra các bài toán tốn thời gian như gõ EMR, tra trạm sạc, phân loại ticket. | Tạo ra danh sách ban đầu rất sát thực tế hệ sinh thái Vingroup. |
| Pitch Problem Card | Trình bày bài "Bác sĩ Vinmec tự gõ EMR", đưa ra con số ước tính 30-40% thời gian lãng phí. | Thuyết phục được nhóm đây là bài có pain thật, thu hút sự ủng hộ của Dũng. |
| Challenge bài của bạn khác | Đặt câu hỏi về tính khả thi của bài "Phân bổ Kubernetes" của Phi (liệu có xin được data thật không?). | Giúp nhóm nhận diện rủi ro data access và loại các bài quá ngách. |
| Gom trùng / cluster | Nhận ra bài của mình và Dũng cùng nói về y tế/EMR. | Gom thành cụm Healthcare Documentation để làm mũi nhọn. |
| Chọn candidate problem | Bảo vệ bài EMR Vinmec bằng cách chỉ ra boundary pháp lý rất rõ (bác sĩ ký số). | Nhóm đồng thuận tuyệt đối chọn bài EMR làm đề tài chính. |
| Validation / research | Đi tìm 4 nghiên cứu (Arndt, Sinsky, AMA) và sản phẩm thực tế (Nuance DAX, PhoBERT) để chứng minh. | Bổ sung evidence vững chắc cho báo cáo, chứng minh bài toán đã có tiền lệ giải quyết. |
| Workflow nhóm | Vẽ chi tiết 8 bước khám bệnh hiện tại, chỉ ra đúng bottleneck ở bước 4-5-6 (gõ narrative và tra mã ICD). | Luồng công việc rõ ràng, nhóm biết chính xác AI cần can thiệp ở đâu. |
| Problem Statement | Định nghĩa phần Impact và Success Metric cụ thể (giảm từ 8-12 phút xuống ≤2 phút). | PS v1 chặt chẽ, đo lường được chứ không nói chung chung. |
| Rule / Workflow / Agent | Phân tích sâu lý do không chọn Agent (pháp lý y tế chặn) và Rule (không xử lý được text tự do). | Chốt định hướng giải pháp ở mức Workflow. |
| Decision | Đề xuất hướng "Not Yet — Go for Pilot" với quy mô nhỏ (3 bác sĩ) để đo baseline. | Quyết định thực tế, khiêm tốn, không over-promise về kết quả. |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Phần Research và Workflow trước/sau là nơi tôi đóng góp nhiều nhất, đặc biệt là việc tìm ra 4 nghiên cứu peer-reviewed và chỉ đích danh 3 bước bottleneck trong chu trình khám bệnh.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Brainstorm thêm các góc nhìn từ dataset 25 problems. | Gợi ý nhiều angle và keywords chuyên ngành y tế/vận hành. | Tự bịa ra các con số tiết kiệm không có căn cứ (kiểu "tiết kiệm 90%"). | Xóa toàn bộ số ảo, chỉ giữ lại insight về quy trình và logic. |
| Problem Card | Prompt AI tạo bảng so sánh ngắn gọn. | Định dạng bảng nhanh, câu chữ mượt. | Viết pain point chung chung kiểu "giúp bác sĩ nhàn hơn". | Ép lại vào công thức định lượng rõ ràng: tốn 8-12 phút/lượt. |
| Workflow | Dùng AI vẽ luồng khám bệnh v0. | Lên khung các bước giao tiếp bác sĩ - bệnh nhân rất nhanh. | AI hoàn toàn mù mờ về quy định ký số bắt buộc tại Việt Nam. | Tự thêm bước "Ký số & submit HIS" làm human boundary bắt buộc. |
| Research | Dùng web search/Perplexity tìm case study (Nuance DAX, Suki AI). | Gom link nhanh, tóm tắt cốt lõi bài báo khoa học mượt mà. | Hay chém gió số liệu báo cáo hoặc nhầm lẫn giữa quảng cáo và nghiên cứu thực tế. | Tự click link verify, chia rõ đâu là số của vendor (Nuance) và đâu là số peer-reviewed (AMA). |
| Problem Statement | Dùng AI gọt giũa câu từ cho súc tích. | Làm ngắn các đoạn mô tả dài dòng. | Field Impact bị bay bổng, viết như văn mẫu. | Viết lại Impact bám sát thực tế mệt mỏi/burnout và pajama time. |
| Rule / Workflow / Agent | Nhờ AI lập bảng so sánh 3 mức tự động hóa. | Phân định Rule và Workflow khá rành mạch, dễ hiểu. | Gợi ý dùng Agent để tự động chẩn đoán bệnh (quá ảo và vi phạm đạo đức y khoa). | Phủ quyết Agent hoàn toàn, nhấn mạnh rào cản pháp lý y tế. |
| Decision | Không dùng | N/A | N/A | Quyết định chốt Go/No-go cần dựa trên tình hình thực tế nhóm (thiếu data, thiếu champion), tự viết sẽ chân thực và sát sườn hơn. |

---

## 3. Reflection câu hỏi mở

**Reflection:**

```text
Thành thật mà nói, lúc đầu tôi cứ nghĩ bài của mình (EMR Vinmec) là "dễ ăn" và ngon nghẻ nhất rồi, nhưng khi nghe top 3 của các bạn khác, đặc biệt là bài VinFast RAG tra cứu tài liệu của Giang, tôi nhận ra mình hơi bị thiên kiến. Bài của Giang có impact về chi phí nằm xưởng rất rõ ràng và dễ làm prototype (RAG) hơn nhiều so với việc loay hoay với data y tế nhạy cảm. 

Trong quá trình làm, nhóm cũng có một giai đoạn hơi bị "solution-first", kiểu ai cũng muốn nhét cái chữ Agent vào cho ngầu, vẽ ra viễn cảnh AI tự chẩn đoán, tự đặt lịch tái khám luôn. Nhưng sau khi bị tôi và Dũng challenge gắt về rào cản của Thông tư 46 bắt buộc bác sĩ phải là người chịu trách nhiệm và ký số, cả nhóm mới "tỉnh mộng" và chịu lùi về mức Workflow. 

Cái khó nhất lúc tôi phụ trách viết Problem Statement chính là phần Boundary. Định nghĩa metric (giảm bao nhiêu phút) thì dễ vì có benchmark quốc tế, nhưng việc vạch ra lằn ranh rõ ràng là "AI chỉ gợi ý draft SOAP, tuyệt đối không tự quyết chẩn đoán cuối cùng" đòi hỏi mình phải thực sự đặt mình vào vị trí chịu rủi ro y tế. Đóng góp mà tôi ưng ý nhất trong bài nhóm chính là phần Workflow và Evidence. Nếu được làm lại, tôi sẽ challenge nhóm mạnh hơn ở khâu đo baseline, bắt mọi người phải nghĩ cách đi phỏng vấn bác sĩ thật sớm hơn thay vì xài proxy data của Mỹ.
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
