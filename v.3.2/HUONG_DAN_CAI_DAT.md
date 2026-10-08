# HƯỚNG DẪN CÀI ĐẶT CHATGPT PROJECT — PHAT-HOC v3.2 LEAN

**Phiên bản:** 3.2  
**Mục tiêu:** Cài một trợ lý nghiên cứu Phật học dùng ít tệp, mặc định nghiên cứu học thuật sâu, truy nguồn trực tiếp khi cần, không lấy một hệ kinh điển hay một ngôn ngữ học thuật làm chuẩn mặc định.

---

# 1. TRIẾT LÝ CÀI ĐẶT

v3.2 dùng kiến trúc:

> **PROJECT INSTRUCTIONS NGẮN + 5 TỆP NGUỒN PHƯƠNG PHÁP**

Không dán toàn bộ phương pháp vào Instructions. Không tách Source Map thành nhiều mô-đun riêng. Mục tiêu là giảm nhiễu truy hồi và giảm tải quy tắc trong lúc AI đang nghiên cứu.

Công thức vận hành:

> **NGHIÊN CỨU TRƯỚC → HẬU KIỂM SAU**

v3.2 kế thừa nền v3.1 đã qua nhiều stress test, đồng thời tăng cường nguyên tắc:

> **KHÔNG CÓ KINH ĐIỂN, TRUYỀN THỐNG HAY NGÔN NGỮ HỌC THUẬT MẶC ĐỊNH.**

Nghĩa là không lấy Pāli/Theravāda làm đại diện mặc định cho toàn bộ Phật giáo, và cũng không coi scholarship tiếng Anh là đại diện mặc định cho toàn bộ học giới quốc tế.

---

# 2. NÊN TẠO PROJECT TEST RIÊNG

Trong giai đoạn kiểm thử, tạo một ChatGPT Project mới, ví dụ:

`Trợ lý — NGHIÊN CỨU PHẬT HỌC v3.2 TEST`

Không trộn v3.1 và v3.2 trong cùng Project thử nghiệm. Giữ Project v3.1 làm benchmark để A/B test khi cần.

---

# 3. CHỈ TẢI 5 TỆP SAU VÀO PROJECT SOURCES / FILES

Từ thư mục `v.3.2/sources/`, tải đúng 5 tệp:

1. `01_NGHIEN_CUU_COT_LOI.md`
2. `02_NGUON_VA_CHUNG_CU.md`
3. `03_PHAN_TANG_VAN_BAN.md`
4. `04_BAN_DO_NGUON_PHAT_HOC.md`
5. `05_HAU_KIEM.md`

Không tải vào Project nghiên cứu:
- các file v1/v2/v3/v3.1;
- file regression test hoặc rubric;
- README/CHANGELOG nếu có;
- file Instructions như một Project Source nếu bạn đã dán nó vào ô Instructions.

Năm marker nguồn phải là:
- `PHAT-HOC-3.2-CORE`
- `PHAT-HOC-3.2-SOURCE`
- `PHAT-HOC-3.2-STRAT`
- `PHAT-HOC-3.2-MAP`
- `PHAT-HOC-3.2-AUDIT`

---

# 4. DÁN PROJECT INSTRUCTIONS

Mở tệp:

`HUONG_DAN_DU_AN_CHATGPT_PHAT_HOC_v3.2.txt`

Sao chép toàn bộ nội dung và dán vào ô **Project Instructions / Hướng dẫn dự án**.

Marker phải là:

`PHAT-HOC-PROJECT-3.2-VI`

Không tự thêm lại các checklist dài của v3 hoặc ghép Instructions của v3.1 vào cùng Project, vì điều đó làm sai phép test và có thể tăng compliance tax.

---

# 5. CÁCH DÙNG HẰNG NGÀY

Sau khi cài, người dùng chỉ cần hỏi tự nhiên, ví dụ:

- `anattā?`
- `Phạm Võng kinh có cổ không?`
- `T1484 do Kumārajīva dịch thật không?`
- `Nāgārjuna có phủ nhận nhân quả không?`
- `Yogācāra có phải duy tâm không?`
- `Đoạn này có phải thêm sau không?`

Không cần thêm:
- “hãy áp dụng skill”;
- “hãy chạy Stage…”;
- “hãy dùng Source Map”;
- “hãy tự kiểm toán”.

Nếu muốn khóa phạm vi, nói trực tiếp điều muốn khóa, ví dụ:

`Chỉ dùng năm Nikāya Pāli; không dùng chú giải hay học giả hiện đại làm chứng cứ.`

---

# 6. KIỂM TRA CÀI ĐẶT

Sau khi tải 5 file và dán Instructions, mở một chat mới trong Project TEST rồi hỏi:

> `Bạn đang áp dụng hệ phương pháp Phật học nào? Hãy nêu marker của Project Instructions và 5 tệp nguồn.`

Kết quả mong đợi:

- `PHAT-HOC-PROJECT-3.2-VI`
- `PHAT-HOC-3.2-CORE`
- `PHAT-HOC-3.2-SOURCE`
- `PHAT-HOC-3.2-STRAT`
- `PHAT-HOC-3.2-MAP`
- `PHAT-HOC-3.2-AUDIT`

Test marker chỉ kiểm việc Project truy cập được file. Nó không chứng minh chất lượng nghiên cứu.

---

# 7. TEST NEO SAU KHI CÀI

Có thể bắt đầu bằng các prompt đã dùng để kiểm v3.1:

> `DN 1 có phải toàn bộ đều là kinh rất sớm không? Hãy phân tầng niên đại nếu có thể.`

> `Duy thức có thật sự nói “chỉ có tâm tồn tại, thế giới bên ngoài không tồn tại” không?`

Mục tiêu là bảo đảm v3.2 giữ được các ưu điểm của v3.1:
- mặc định nghiên cứu sâu;
- truy nguồn trực tiếp khi claim quyết định;
- phân tầng văn bản chặt;
- không phá phạm vi đóng;
- không lấy Pāli làm chuẩn chung;
- không để nguồn trung gian gánh nhiều nhánh quyết định.

Sau đó test riêng năng lực mới của v3.2 bằng các prompt đòi hỏi scholarship đa ngôn ngữ/đa truyền thống nghiên cứu, ví dụ:

> `Khi so sánh anattā với ātman của Bṛhadāraṇyaka và Chāndogya Upaniṣad, các chuyên gia Veda/Upaniṣad — không chỉ Buddhist Studies — hiểu ātman trong các văn bản đó như thế nào?`

> `Hãy nghiên cứu T1484 và chủ động kiểm scholarship Nhật Bản và Trung Quốc/Đài Loan, không chỉ công trình tiếng Anh.`

---

# 8. A/B TEST v3.1 — v3.2

Để so sánh công bằng:

1. dùng cùng một câu hỏi;
2. mở chat mới ở mỗi Project;
3. dùng cùng model/settings nếu có thể;
4. không thêm prompt phụ ngoài câu test;
5. lưu nguyên câu trả lời;
6. so sánh ít nhất các trục:
   - xử lý mơ hồ;
   - chiều sâu truy nguồn;
   - tỷ lệ nguồn trực tiếp so với nguồn discovery;
   - chuỗi lập luận chứng cứ;
   - phản chứng;
   - phân tầng văn bản;
   - mức chắc chắn;
   - độ bao phủ corpus;
   - độ bao phủ học giới/ngôn ngữ;
   - khả năng mở sang ngành chuyên môn ngoài Buddhist Studies khi cần;
   - độ tự nhiên và sạch đầu ra.

Không kết luận từ một lượt duy nhất nếu khác biệt nhỏ. Nếu cùng một pattern lặp qua nhiều câu hỏi, mới xem đó là đặc tính kiến trúc.

---

# 9. KHI CÂU HỎI NẰM NGOÀI SOURCE MAP

`04_BAN_DO_NGUON_PHAT_HOC.md` là bản đồ, không phải whitelist.

Nếu đề tài chưa được bao phủ rõ:
- không ép vào mục gần nhất;
- dùng lõi + quy chuẩn nguồn để tự dựng phạm vi;
- tìm nguồn ngoài Map nếu phù hợp;
- mở sang ngành chuyên môn liên quan nếu chính câu hỏi đòi hỏi.

Không cần tạo thêm module chỉ để xử lý một ca đơn lẻ.

---

# 10. KHI CẬP NHẬT v3.2

Ưu tiên sửa **ít và đúng chỗ**.

Trước khi thêm một quy tắc mới, hỏi:

> “Lỗi này có cần luật mới, hay chỉ cần sửa một luật hiện có / chuyển nó sang hậu kiểm?”

Không chữa over-prompting bằng cách tiếp tục thêm prompt.

Nếu một lỗi lặp lại qua nhiều regression test, mới cân nhắc thay đổi kiến trúc.

---

# 11. TRẠNG THÁI PHIÊN BẢN

v3.2 chưa phải bản ổn định cho đến khi hoàn tất test riêng của nhánh 3.2.

Quy trình khuyến nghị:

> `phat-hoc-v3.2-development` → Project v3.2 TEST → A/B với v3.1 → stress test đa học giới/ngôn ngữ → sửa lỗi nếu cần → regression → duyệt → release.

Không merge vào `main` trước khi có phê duyệt cuối.
