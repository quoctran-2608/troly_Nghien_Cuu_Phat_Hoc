# HƯỚNG DẪN CÀI ĐẶT CHATGPT PROJECT — TRỢ LÝ NGHIÊN CỨU PHẬT HỌC v3.0

**Phiên bản:** 3.0  
**Mục tiêu:** Cài PHAT-HOC 3.0 vào một ChatGPT Project sao cho người dùng chỉ cần hỏi tự nhiên, còn trợ lý tự xác định phạm vi, định tuyến nguồn, nghiên cứu, phản chứng và kiểm toán.

---

# 1. KIẾN TRÚC CÀI ĐẶT

PHAT-HOC 3.0 được tách thành hai lớp:

## Lớp A — Project Instructions

Dùng tệp:

`HUONG_DAN_DU_AN_CHATGPT_PHAT_HOC_v3.0.txt`

Sao chép toàn bộ nội dung tệp này vào ô **Instructions / Hướng dẫn dự án**.

Bản này được thiết kế chủ động dưới 8.000 ký tự. Không dán các tệp phương pháp dài vào ô Instructions.

## Lớp B — Project Sources / Files

Tải các tệp phương pháp và Source Map vào nguồn của Project.

Các tệp này chứa chi tiết mà Instructions chỉ định tuyến tới.

---

# 2. KHÔNG TRỘN v2 VÀ v3 TRONG CÙNG PROJECT THỬ NGHIỆM

Khi thử v3, khuyến nghị dùng một Project mới hoặc bảo đảm các tệp phương pháp v2 không còn hoạt động cùng lúc.

Không nên để đồng thời:

- `BO_QUY_TAC_NGHIEN_CUU_PHAT_HOC_TOAN_DIEN_v2.0.md`;
- `HUONG_DAN_DU_AN_CHATGPT_PHAT_HOC_v2.1.txt`;

với bộ v3 trong cùng một Project, vì hai bộ có kiến trúc và tên tệp khác nhau và có thể làm truy hồi lẫn lộn.

v2 vẫn được giữ nguyên trong GitHub để tham khảo và phục hồi khi cần.

---

# 3. CÁC TỆP BẮT BUỘC PHẢI TẢI VÀO PROJECT

## Nhóm 1 — Lõi phương pháp: bắt buộc

1. `PHUONG_PHAP_NGHIEN_CUU_COT_LOI.md`
2. `QUY_CHUAN_NGUON_VA_CHUNG_CU.md`
3. `QUY_TRINH_PHAN_TANG_VAN_BAN.md`
4. `KIEM_TOAN_VA_HAU_KIEM.md`

Bốn tệp này tạo thành lõi nghiên cứu và kiểm toán.

## Nhóm 2 — Bộ định tuyến Source Map: bắt buộc

5. `00_BUDDHIST_SOURCE_MAP_DINH_TUYEN.md`

Đây là tệp router trung tâm. Trong GitHub hiện vẫn có `source-map/README.md` với nội dung tương đương để duyệt repo; **không cần tải README.md vào ChatGPT Project**. Dùng tệp `00_...` vì tên duy nhất và dễ được Instructions gọi chính xác.

## Nhóm 3 — Mô-đun Source Map: nên tải đầy đủ

6. `01_PHAT_GIAO_THOI_KY_DAU_NIKAYA_AGAMA.md`
7. `02_THERAVADA.md`
8. `03_ABHIDHARMA_VA_CAC_BO_PHAI.md`
9. `04_MADHYAMAKA.md`
10. `05_YOGACARA_TATHAGATAGARBHA.md`
11. `06_KINH_DIEN_DAI_THUA.md`
12. `07_VINAYA.md`
13. `08_VAJRAYANA_TIBET.md`
14. `09_PHAT_GIAO_DONG_A.md`
15. `10_GANDHARA_TRUNG_A.md`
16. `11_LUAN_LY_NHAN_THUC_LUAN.md`
17. `12_BOI_CANH_AN_DO_KHAO_CO_LIEN_TON_GIAO.md`

Các thư mục trong GitHub chỉ dùng để tổ chức repo. Khi tải vào ChatGPT Project, điều quan trọng là **tên tệp duy nhất** và nội dung/marker của tệp; không cần tái tạo cấu trúc thư mục.

---

# 4. CÁCH CÀI ĐẶT

## Bước 1 — Tạo Project thử nghiệm v3

Khuyến nghị tạo một Project riêng trong giai đoạn kiểm thử, ví dụ:

> `Trợ lý — NGHIÊN CỨU PHẬT HỌC v3 TEST`

Mục đích là tránh ảnh hưởng Project v2 đang dùng.

Nếu bạn đang sử dụng chế độ bộ nhớ chỉ dành cho Project và muốn giữ dự án nghiên cứu tách biệt, có thể tiếp tục dùng cách đó.

## Bước 2 — Tải 17 tệp nguồn

Tải 4 tệp trong `core/`, tệp router `00_...` và 12 mô-đun Source Map vào phần Sources / Files của Project.

Không tải:
- file v1/v2;
- tài liệu test;
- README repo;
- prompt Instructions như một nguồn thay cho việc dán nó vào Instructions.

## Bước 3 — Dán Project Instructions

Mở:

`HUONG_DAN_DU_AN_CHATGPT_PHAT_HOC_v3.0.txt`

Sao chép **toàn bộ** nội dung vào Project Instructions và lưu.

Không tự rút gọn thêm trong lần thử đầu tiên.

## Bước 4 — Mở cuộc trò chuyện mới

Sau khi thay nguồn hoặc Instructions, nên chạy bài thử trong một chat mới của chính Project để giảm ảnh hưởng của lịch sử thử nghiệm cũ.

---

# 5. PROJECT INSTRUCTIONS ĐƯỢC THIẾT KẾ NHƯ THẾ NÀO?

Instructions không cố chứa toàn bộ phương pháp.

Nó chỉ giữ các luật có mức ưu tiên cao nhất:

1. mọi câu hỏi Phật học tự kích hoạt v3;
2. người dùng không cần câu lệnh dài;
3. lõi phương pháp luôn áp dụng;
4. router chọn Source Map liên quan;
5. câu hỏi thực chứng phải kiểm nguồn;
6. lịch sử văn bản tự kích hoạt protocol phân tầng;
7. vấn đề tranh luận phải tìm phản chứng;
8. trước khi gửi phải kiểm toán;
9. đầu ra là tiếng Việt tự nhiên;
10. các tệp phương pháp không được dùng làm chứng cứ.

Thiết kế này nhằm giảm xung đột giữa một prompt dài và cơ chế truy hồi tệp của ChatGPT Project.

---

# 6. CƠ CHẾ ĐỊNH TUYẾN MONG ĐỢI

Ví dụ:

### Người dùng hỏi

> `anattā?`

Trợ lý phải tự nhận diện đây là thuật ngữ Phật học. Tùy cách trả lời và phạm vi, có thể gọi mô-đun 01; nếu mở sang Theravāda hậu kỳ mới gọi thêm 02. Không được bắt người dùng viết “hãy nghiên cứu theo skill”.

### Người dùng hỏi

> `Phạm Võng kinh có cổ không?`

Trợ lý phải phát hiện tên này mơ hồ giữa các văn bản khác nhau và không âm thầm chọn một nghĩa.

### Người dùng hỏi

> `Phạm Võng DN 1 có phần thêm sau không?`

Phải tự động dùng:
- lõi phương pháp;
- quy chuẩn nguồn;
- mô-đun 01;
- protocol phân tầng;
- hậu kiểm.

### Người dùng hỏi

> `Nāgārjuna có phủ nhận nhân quả không?`

Router ưu tiên mô-đun 04; nếu câu hỏi cần đối chiếu Abhidharma hoặc kinh sớm thì mới mở thêm 03 hoặc 01.

### Người dùng hỏi

> `Chỉ dùng năm Nikāya Pāli: anattā được trình bày thế nào?`

Đây là **phạm vi đóng**. Source Map không được lén đưa Āgama, Abhidhamma hoặc nguồn ngoài phạm vi vào làm chứng cứ.

---

# 7. BÀI KIỂM TRA CÀI ĐẶT NHANH

Sau khi cài, mở một chat mới và chạy lần lượt.

## Test A — Nhận diện phiên bản và tệp

Hỏi:

> `Bạn đang áp dụng hệ phương pháp Phật học nào? Hãy nêu marker của Project Instructions, lõi, quy chuẩn nguồn, phân tầng, kiểm toán và Source Map.`

Kết quả mong đợi phải nhận ra:
- `PHAT-HOC-PROJECT-3.0-VI`
- `PHAT-HOC-3.0-CORE`
- `PHAT-HOC-3.0-SOURCE-GOV`
- `PHAT-HOC-3.0-STRATIFICATION`
- `PHAT-HOC-3.0-AUDIT`
- `PHAT-HOC-3.0-SOURCE-MAP`

## Test B — Tự động kích hoạt từ câu ngắn

Hỏi đúng:

> `Phạm Võng kinh có cổ không?`

Đạt khi:
- phát hiện tên mơ hồ;
- không yêu cầu bạn phải nói “hãy nghiên cứu”;
- tự kiểm nguồn nếu đưa ra kết luận lịch sử.

## Test C — Phân tầng

Hỏi:

> `Phạm Võng kinh trong Trường Bộ có phải bài kinh rất sớm không?`

Đạt khi:
- không coi toàn bộ DN 1 là một khối đồng niên;
- tìm truyền bản liên quan;
- phân biệt lõi sớm với nguyên văn lời Đức Phật;
- không dùng vắng mặt ở một bản làm chứng cứ đủ.

## Test D — Phạm vi đóng

Hỏi:

> `Chỉ dùng năm Nikāya Pāli. Giải thích anattā trong phạm vi đó; không dùng Āgama hay Abhidhamma làm chứng cứ.`

Đạt khi không phá phạm vi.

## Test E — Nguồn và mức truy cập

Hỏi:

> `Khi bạn chỉ tìm được abstract của một bài nghiên cứu, bạn có được viết “tác giả đã chứng minh rằng...” không?`

Đạt khi trả lời **không**, và phân biệt metadata/abstract với việc đã đọc phần lập luận trực tiếp.

Các test regression đầy đủ sẽ nằm trong bước kiểm thử riêng; các test trên chỉ kiểm tra cài đặt.

---

# 8. CÁCH DÙNG HẰNG NGÀY

Sau khi cài đúng, **không cần prompt nghiên cứu mẫu**.

Chỉ hỏi tự nhiên, ví dụ:

> `Niết-bàn là gì?`

> `Đức Phật có nói câu này không?`

> `Kinh này có lớp muộn không?`

> `Yogācāra có phải duy tâm không?`

> `Nāgārjuna hiểu duyên khởi thế nào?`

> `Phạm Võng T1484 do Kumārajīva dịch thật không?`

Trợ lý tự quyết định độ sâu và hệ nguồn.

Nếu muốn giới hạn nghiên cứu, chỉ cần nói giới hạn thực sự, ví dụ:

> `Chỉ dùng Hán tạng.`

> `Chủ yếu xét các truyền bản sớm; có thể dùng nghiên cứu hiện đại để phân tích.`

> `Không bàn truyền thống chú giải hậu kỳ.`

---

# 9. KHI PROJECT KHÔNG TÌM THẤY TỆP

Nếu trợ lý nói không truy cập được một file:
1. kiểm tra file đã được tải vào đúng Project chưa;
2. kiểm tra tên file;
3. mở chat mới;
4. hỏi lại marker của file.

Không sửa Instructions để bảo trợ lý “hãy giả định nội dung file”. Quy tắc v3 cấm giả vờ đã đọc nguồn Project không truy cập được.

---

# 10. KHI CẬP NHẬT SOURCE MAP

Có thể bổ sung hoặc sửa mô-đun sau này mà không cần viết lại toàn bộ Instructions, miễn:
- marker hệ v3 không đổi hoặc được nâng có chủ ý;
- tên router và mô-đun được cập nhật nhất quán;
- regression tests được chạy lại.

Đây là lợi ích chính của kiến trúc mô-đun.

---

# 11. NGUYÊN TẮC AN TOÀN KHI NÂNG PHIÊN BẢN

Không chỉnh trực tiếp Project đang dùng ổn định trước khi test bản mới.

Quy trình khuyến nghị:

> GitHub development branch → Project TEST → regression tests → sửa lỗi → duyệt → đưa vào bản ổn định → thay Project chính.

Không xóa v2 khỏi GitHub. v2 là bản mốc để so sánh hồi quy.

---

# 12. TÌNH TRẠNG CỦA BẢN v3.0

Ở giai đoạn này đã có:
- 4 tệp core;
- Source Map router;
- 12 mô-đun Source Map;
- Project Instructions v3;
- hướng dẫn cài đặt này.

Chưa coi là bản phát hành ổn định cho đến khi hoàn tất **bộ kiểm thử hồi quy** và rà soát cuối.

Dấu hiệu Project Instructions:

`PHAT-HOC-PROJECT-3.0-VI`
