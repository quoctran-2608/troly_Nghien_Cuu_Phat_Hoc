# BUDDHIST SOURCE MAP v3 — BỘ ĐỊNH TUYẾN NGUỒN PHẬT HỌC

**Phiên bản:** 3.0  
**Dấu hiệu:** `PHAT-HOC-3.0-SOURCE-MAP`  
**Vai trò:** Giúp ChatGPT Project xác định nhanh những hệ văn bản, truyền bản, ngôn ngữ, hạ tầng và tuyến học giới nào cần được khảo sát cho từng câu hỏi Phật học.

---

# 1. ĐỊA VỊ CỦA SOURCE MAP

Source Map là **lớp định tuyến**, không phải nguồn học thuật và không phải danh sách trắng.

Nó trả lời:
- câu hỏi này nên mở những nhánh nguồn nào;
- tầng văn bản nào phải tách;
- ngôn ngữ/truyền bản nào có thể thay đổi kết luận;
- hạ tầng nào hữu ích để định vị;
- tuyến học giới nào có khả năng quan trọng;
- lỗi định tuyến nào thường làm sai nghiên cứu.

Nó không được:
- quyết định kết luận;
- thay `QUY_CHUAN_NGUON_VA_CHUNG_CU.md` thẩm định nguồn thật;
- phá phạm vi đóng do người dùng đặt;
- biến tên website thành chứng cứ;
- chọn sẵn học giả “đúng”;
- ngăn phát hiện nguồn mới phù hợp ngoài Map.

Nguyên tắc:

> **MAP LÀ MỨC SÀN BAO PHỦ, KHÔNG PHẢI TRẦN TÌM KIẾM.**

---

# 2. CÁCH DÙNG TRONG CHATGPT PROJECT

Không nạp toàn bộ 12 mô-đun cho mọi câu hỏi.

Quy trình nội bộ:
1. đọc câu hỏi;
2. xác định đối tượng, thời kỳ, loại văn bản và phạm vi;
3. chọn **ít nhất một mô-đun lõi**, tối đa chỉ các mô-đun thật sự có khả năng thay đổi kết luận;
4. nếu câu hỏi đi qua nhiều truyền thống, kết hợp các mô-đun;
5. nếu câu hỏi nằm ngoài Map, không ép vào mô-đun gần nhất; dùng lõi phương pháp chung và ghi nhận khoảng trống Map;
6. mọi nguồn được tìm thấy vẫn phải qua quy chuẩn nguồn/chứng cứ.

Mục tiêu là **truy hồi ít nhưng đúng**, tránh phình ngữ cảnh của ChatGPT Project.

---

# 3. BẢNG ĐỊNH TUYẾN NHANH

| Tín hiệu câu hỏi | Mô-đun ưu tiên |
|---|---|
| Nikāya, Āgama, Phật giáo thời kỳ đầu, lời Phật, bản song hành sớm | 01 |
| Theravāda, Pāli, Abhidhamma, Buddhaghosa, chú giải Theravāda | 02 |
| Sarvāstivāda, Vaibhāṣika, Sautrāntika, Abhidharma, bộ phái | 03 |
| Nāgārjuna, Trung quán, tính không, MMK, Madhyamaka | 04 |
| Yogācāra, Vijñaptimātra, ālayavijñāna, Như Lai tạng | 05 |
| Bát-nhã, Pháp Hoa, Hoa Nghiêm, Tịnh độ, kinh Đại thừa | 06 |
| Luật, giới, Tăng đoàn, Prātimokṣa, Vinaya, Bồ-tát giới | 07 |
| Tantra, mật điển, mantra, sādhana, Tây Tạng, Kangyur/Tengyur | 08 |
| Trung Quốc, Triều Tiên, Nhật Bản, Việt Nam; Thiền, Thiên Thai, Hoa Nghiêm, Tịnh Độ | 09 |
| Gāndhārī, Gandhāra, Khotan, Trung Á, thủ bản, Con đường Tơ lụa | 10 |
| Dignāga, Dharmakīrti, pramāṇa, luận lý, nhận thức luận | 11 |
| Veda/Bà-la-môn, Jain, Ājīvika, khảo cổ, bia ký, lịch sử xã hội Ấn Độ | 12 |

Một câu hỏi có thể kích hoạt nhiều mô-đun. Ví dụ:
- “Nāgārjuna có tiếp nối duyên khởi trong kinh sớm không?” → 01 + 04.
- “Bồ-tát giới Phạm Võng hình thành khi nào?” → 06 + 07 + 09.
- “Yogācāra ở Tây Tạng hiểu ālayavijñāna ra sao?” → 05 + 08.

---

# 4. NGUYÊN TẮC CHỌN MÔ-ĐUN

## 4.1. Chọn theo câu hỏi, không theo từ khóa máy móc

Tên một truyền thống xuất hiện trong câu không tự động buộc mở toàn bộ mô-đun nếu nó chỉ là bối cảnh phụ.

## 4.2. Không mở đa ngôn ngữ để làm đẹp

Chỉ mở ngôn ngữ/truyền bản nếu:
- nguồn quyết định được bảo tồn ở đó;
- khác biệt ngôn ngữ có thể thay đổi kết luận;
- học giới chuyên ngành ở ngôn ngữ đó có đóng góp trực tiếp.

## 4.3. Phạm vi người dùng cao hơn Map

Nếu người dùng nói “chỉ dùng năm Nikāya Pāli”, Map không được tự đưa Āgama, Abhidhamma hay học giả hiện đại vào làm chứng cứ.

## 4.4. Đề tài ngoài Map

Nếu câu hỏi chưa có mô-đun phù hợp:
- không bịa mô-đun;
- dùng `PHUONG_PHAP_NGHIEN_CUU_COT_LOI.md` + `QUY_CHUAN_NGUON_VA_CHUNG_CU.md`;
- tự lập phạm vi mở có kiểm soát;
- ghi nhận `CANDIDATE MAP UPDATE` nội bộ nếu loại câu hỏi có giá trị lặp lại.

---

# 5. SCHEMA BẮT BUỘC CỦA MỖI MÔ-ĐUN

Mỗi mô-đun gồm:

**A. Tín hiệu kích hoạt** — loại câu hỏi nên gọi mô-đun.  
**B. Ranh giới khái niệm** — những phạm trù dễ bị trộn.  
**C. Tầng nguồn cần cân nhắc** — các lớp nguồn có thể quan trọng.  
**D. Ngôn ngữ và truyền bản** — các nhánh có thể thay đổi kết luận.  
**E. Hạ tầng truy cập/định vị** — nơi ưu tiên tìm nguồn; không phải chứng cứ tự thân.  
**F. Tuyến học giới cần thăm dò** — chuyên ngành/ngôn ngữ học thuật đáng chú ý.  
**G. Vùng tranh luận định tuyến** — vấn đề phải mở đủ để nghiên cứu, không tự quyết.  
**H. Lỗi định tuyến thường gặp** — shortcut cần tránh.  
**I. Giới hạn** — điều mô-đun không được dùng để kết luận.  
**J. CANDIDATE MAP UPDATE** — tiêu chí mở rộng mô-đun sau này.

---

# 6. QUY TẮC VỀ HẠ TẦNG

Tên các nền tảng trong mô-đun chỉ là **điểm ưu tiên để định vị/truy cập**.

Phải truy ngược về:
- văn bản/edition cụ thể;
- bản dịch cụ thể;
- thủ bản/facsimile cụ thể;
- bài báo/sách cụ thể.

Không viết kiểu “CBETA cho rằng…”, “BDRC nói…”, “SuttaCentral chứng minh…”.

Nếu nền tảng thay đổi, URL chết hoặc item không rõ nguồn gốc, tìm hạ tầng khác; Map không được biến thành whitelist cứng.

---

# 7. QUY TẮC VỀ HỌC GIỚI ĐA NGÔN NGỮ

Không coi tiếng Anh là toàn bộ học giới.

Tùy đề tài, phải cân nhắc:
- Nhật;
- Hoa/Đài Loan;
- Pháp;
- Đức;
- Nga;
- Ba Lan;
- Hàn;
- Nam Á và các tuyến khác.

Không đặt quota quốc gia. Chỉ mở nhánh khi có khả năng ảnh hưởng trực tiếp đến câu hỏi.

Nếu không truy cập được một nhánh có khả năng quan trọng, áp dụng `GIỚI HẠN BAO PHỦ` theo quy chuẩn nguồn.

---

# 8. CÁC MÔ-ĐUN v3.0

1. `01_PHAT_GIAO_THOI_KY_DAU_NIKAYA_AGAMA.md`
2. `02_THERAVADA.md`
3. `03_ABHIDHARMA_VA_CAC_BO_PHAI.md`
4. `04_MADHYAMAKA.md`
5. `05_YOGACARA_TATHAGATAGARBHA.md`
6. `06_KINH_DIEN_DAI_THUA.md`
7. `07_VINAYA.md`
8. `08_VAJRAYANA_TIBET.md`
9. `09_PHAT_GIAO_DONG_A.md`
10. `10_GANDHARA_TRUNG_A.md`
11. `11_LUAN_LY_NHAN_THUC_LUAN.md`
12. `12_BOI_CANH_AN_DO_KHAO_CO_LIEN_TON_GIAO.md`

---

# 9. QUY TẮC BẢO TRÌ MAP

Chỉ thêm nguồn, hạ tầng hoặc nhánh nghiên cứu khi nó có **giá trị định tuyến lặp lại**, không phải chỉ giúp một ca nghiên cứu đơn lẻ.

Không thêm:
- kết luận của một tranh luận;
- danh sách học giả “nên tin”;
- prompt mẫu dài;
- dữ kiện quá chuyên biệt;
- website phổ thông chỉ vì dễ tìm.

Khi Map lớn lên, ưu tiên tăng độ chính xác của router thay vì tiếp tục nạp toàn bộ mô-đun vào mọi lượt.

---

# 10. CÔNG THỨC VẬN HÀNH

> **CÂU HỎI → XÁC ĐỊNH PHẠM VI → CHỌN MÔ-ĐUN TỐI THIỂU CẦN THIẾT → MỞ HỆ NGUỒN PHÙ HỢP → THẨM ĐỊNH NGUỒN THẬT → NGHIÊN CỨU → PHẢN CHỨNG → KIỂM TOÁN → TRẢ LỜI.**

Source Map chỉ giúp ChatGPT **đi đúng đường**; chứng cứ thật mới quyết định câu trả lời.