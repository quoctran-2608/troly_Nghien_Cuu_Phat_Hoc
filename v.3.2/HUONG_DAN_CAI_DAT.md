# HƯỚNG DẪN CÀI ĐẶT CHATGPT PROJECT — PHAT-HOC v3.1 LEAN

**Phiên bản:** 3.1  
**Mục tiêu:** Cài một trợ lý nghiên cứu Phật học dùng ít tệp, prompt ngắn và ưu tiên chiều sâu nghiên cứu hơn việc tuân thủ checklist dày đặc.

---

# 1. TRIẾT LÝ CÀI ĐẶT

v3.1 dùng kiến trúc:

> **PROJECT INSTRUCTIONS NGẮN + 5 TỆP NGUỒN PHƯƠNG PHÁP**

Không dán toàn bộ phương pháp vào Instructions. Không tách Source Map thành nhiều mô-đun riêng. Mục tiêu là giảm nhiễu truy hồi và giảm tải quy tắc trong lúc AI đang nghiên cứu.

Công thức vận hành:

> **NGHIÊN CỨU TRƯỚC → HẬU KIỂM SAU**

---

# 2. NÊN TẠO PROJECT TEST RIÊNG

Trong giai đoạn kiểm thử, tạo một ChatGPT Project mới, ví dụ:

`Trợ lý — NGHIÊN CỨU PHẬT HỌC v3.1 TEST`

Không trộn v2, v3 và v3.1 trong cùng Project thử nghiệm. Giữ các Project cũ để A/B/C test.

---

# 3. CHỈ TẢI 5 TỆP SAU VÀO PROJECT SOURCES / FILES

Từ thư mục `v.3.1/sources/`, tải đúng 5 tệp:

1. `01_NGHIEN_CUU_COT_LOI.md`
2. `02_NGUON_VA_CHUNG_CU.md`
3. `03_PHAN_TANG_VAN_BAN.md`
4. `04_BAN_DO_NGUON_PHAT_HOC.md`
5. `05_HAU_KIEM.md`

Không tải vào Project nghiên cứu:
- các file v1/v2/v3;
- file regression test hoặc rubric;
- README/CHANGELOG;
- file Instructions như một Project Source nếu bạn đã dán nó vào ô Instructions.

Năm marker nguồn phải là:
- `PHAT-HOC-3.1-CORE`
- `PHAT-HOC-3.1-SOURCE`
- `PHAT-HOC-3.1-STRAT`
- `PHAT-HOC-3.1-MAP`
- `PHAT-HOC-3.1-AUDIT`

---

# 4. DÁN PROJECT INSTRUCTIONS

Mở tệp:

`HUONG_DAN_DU_AN_CHATGPT_PHAT_HOC_v3.1.txt`

Sao chép toàn bộ nội dung và dán vào ô **Project Instructions / Hướng dẫn dự án**.

Marker phải là:

`PHAT-HOC-PROJECT-3.1-VI`

Bản Instructions này dài khoảng 3.120 ký tự, chủ động thấp hơn nhiều so với giới hạn 8.000 ký tự của cấu hình mục tiêu. Không tự thêm lại các checklist dài của v3 trong lần test đầu.

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

- `PHAT-HOC-PROJECT-3.1-VI`
- `PHAT-HOC-3.1-CORE`
- `PHAT-HOC-3.1-SOURCE`
- `PHAT-HOC-3.1-STRAT`
- `PHAT-HOC-3.1-MAP`
- `PHAT-HOC-3.1-AUDIT`

Test marker chỉ kiểm việc Project truy cập được file. Nó không chứng minh chất lượng nghiên cứu.

---

# 7. TEST QUAN TRỌNG NHẤT SAU KHI CÀI

Chạy trong một chat mới:

> `Phạm Võng kinh có cổ không?`

Mục tiêu của v3.1 là đồng thời đạt hai điều:

1. xử lý mơ hồ tốt như v3: phân biệt DN 1 và T1484 sớm;
2. đào nguồn sâu ít nhất ngang v2: nếu mệnh đề trung tâm dựa vào Groner, Funayama, Anālayo hoặc một công trình chuyên ngành khác, phải cố truy tới công trình gốc/nguồn trực tiếp khi có thể thay vì dừng ở trang tổng hợp.

Đây là test neo chính để kiểm kiến trúc Lean có thành công hay không.

---

# 8. A/B/C TEST v2 — v3 — v3.1

Để so sánh công bằng:

1. dùng cùng một câu hỏi;
2. mở chat mới ở mỗi Project;
3. không thêm prompt phụ;
4. lưu nguyên câu trả lời;
5. so sánh ít nhất các trục:
   - xử lý mơ hồ;
   - chiều sâu truy nguồn;
   - tỷ lệ nguồn trực tiếp so với nguồn discovery;
   - chuỗi lập luận chứng cứ;
   - phản chứng;
   - phân tầng văn bản;
   - mức chắc chắn;
   - độ tự nhiên và gọn;
   - lỗi kỹ thuật đầu ra.

Không kết luận từ một lượt duy nhất nếu khác biệt nhỏ. Nếu cùng một pattern lặp qua nhiều câu hỏi, mới xem đó là đặc tính kiến trúc.

---

# 9. KHI CÂU HỎI NẰM NGOÀI SOURCE MAP

`04_BAN_DO_NGUON_PHAT_HOC.md` là bản đồ, không phải whitelist.

Nếu đề tài chưa được bao phủ rõ:
- không ép vào mục gần nhất;
- dùng lõi + quy chuẩn nguồn để tự dựng phạm vi;
- tìm nguồn ngoài Map nếu phù hợp.

Không cần tạo thêm module chỉ để xử lý một ca đơn lẻ.

---

# 10. KHI CẬP NHẬT v3.1

Ưu tiên sửa **ít và đúng chỗ**.

Trước khi thêm một quy tắc mới, hỏi:

> “Lỗi này có cần luật mới, hay chỉ cần sửa một luật hiện có / chuyển nó sang hậu kiểm?”

Không chữa over-prompting bằng cách tiếp tục thêm prompt.

Nếu một lỗi lặp lại qua nhiều regression test, mới cân nhắc thay đổi kiến trúc.

---

# 11. TRẠNG THÁI PHIÊN BẢN

v3.1 chưa phải bản ổn định cho đến khi hoàn tất A/B/C test và regression test.

Quy trình khuyến nghị:

> `phat-hoc-v3.1-development` → Project v3.1 TEST → A/B/C test → sửa lỗi → regression → duyệt → release.

Không merge vào `main` trước khi có phê duyệt cuối.
