# BẢN ĐỒ NGUỒN PHẬT HỌC — v3.1 LEAN

**Phiên bản:** 3.1  
**Bản chỉnh:** 3.1b  
**Dấu hiệu:** `PHAT-HOC-3.1-MAP`  
**Vai trò:** Bản đồ định tuyến corpus, ngôn ngữ, hạ tầng và tuyến học giới.  
**Địa vị:** Công cụ tìm đường; không phải nguồn học thuật và không phải whitelist.

---

# 1. CÁCH DÙNG

Chỉ mở những vùng thật sự liên quan đến câu hỏi.

Source Map giúp trả lời:
- nên tìm ở corpus nào;
- ngôn ngữ/truyền bản nào có thể quan trọng;
- hạ tầng nào hữu ích để định vị;
- lỗi định tuyến nào cần tránh.

Nó **không**:
- quyết định kết luận;
- thay `02_NGUON_VA_CHUNG_CU.md`;
- phá phạm vi đóng;
- biến website thành chứng cứ;
- chọn sẵn học giả “đúng”.

Nguyên tắc:

> **MAP LÀ MỨC SÀN BAO PHỦ, KHÔNG PHẢI TRẦN TÌM KIẾM.**

Nếu đề tài nằm ngoài Map, dùng lõi phương pháp để tự dựng phạm vi; không ép vào vùng gần nhất.

---

# 2. THỨ TỰ TRA CỨU ƯU TIÊN

Khi câu hỏi cần tra cứu, mặc định đi theo ba tuyến sau, nhưng chỉ dùng những tuyến thật sự phù hợp:

**Tuyến 1 — Hạ tầng corpus/chuyên ngành.** Bắt đầu ở các cơ sở chuyên cho loại văn bản hoặc truyền thống đang nghiên cứu. Đây thường là nơi tốt nhất để xác định đúng văn bản, edition, parallel, catalog hoặc manuscript.

**Tuyến 2 — Hạ tầng học thuật.** Tìm bài báo, sách, chương sách, luận án, bibliographic record và repository học thuật, đặc biệt khi cần lịch sử nghiên cứu, tác quyền, niên đại hoặc tranh luận chuyên ngành.

**Tuyến 3 — Web rộng.** Dùng để khám phá thêm từ khóa, lần bibliography, tìm bản toàn văn hoặc nguồn chưa có trong các hạ tầng trên. Web rộng không tự động là nguồn chứng minh; sau khi phát hiện một nguồn quan trọng, quay về quy tắc truy nguồn trong `02_NGUON_VA_CHUNG_CU.md`.

Các hạ tầng ưu tiên theo chức năng:

| Nhu cầu | Hạ tầng nên thử trước |
|---|---|
| Nikāya/Āgama, Pāli, parallel sớm | SuttaCentral, Pali Text Society |
| Hán tạng và Đại Chính tân tu Đại tạng kinh | CBETA, SAT |
| Sanskrit/Pāli/Prakrit e-text | GRETIL; DSBC khi phù hợp |
| Tây Tạng, Kangyur/Tengyur, scan/catalog | BDRC/BUDA; 84000 cho bản dịch và định vị |
| Gāndhārī/Kharoṣṭhī/Gandhāra | Gandhari.org |
| Dunhuang/Trung Á | International Dunhuang Programme và catalog chuyên ngành |
| Nghiên cứu Nhật/Đông Á | INBUDS, CiNii, J-STAGE, DLMBS |
| Nghiên cứu học thuật rộng | JSTOR, Project MUSE, repository đại học, nhà xuất bản học thuật và cơ sở thư mục chuyên ngành |

Đây là **thứ tự ưu tiên tìm kiếm**, không phải thứ tự uy tín tuyệt đối và không phải danh sách đóng. Một nguồn ngoài danh sách vẫn được dùng nếu phù hợp và qua thẩm định.

**Uy tín của platform không thay thế việc đánh giá item.** CBETA có thể rất tốt để truy văn bản Hán nhưng không tự nó chứng minh một niên đại lịch sử; CiNii có thể giúp tìm bài Nhật nhưng bibliographic record không đồng nghĩa đã đọc bài; 84000 hữu ích cho bản dịch Tạng nhưng không thay critical edition khi câu hỏi phụ thuộc ngữ văn.

---

# 3. ĐỊNH TUYẾN NHANH

| Tín hiệu chính | Vùng ưu tiên |
|---|---|
| Nikāya, Āgama, Phật giáo sớm, lời Phật, bản song hành | 01 |
| Theravāda, Pāli, Abhidhamma Pāli, Buddhaghosa | 02 |
| Sarvāstivāda, Vaibhāṣika, Sautrāntika, Abhidharma bộ phái | 03 |
| Nāgārjuna, Madhyamaka, MMK, tính không | 04 |
| Yogācāra, vijñaptimātra, ālayavijñāna, tathāgatagarbha | 05 |
| Kinh Đại thừa: Bát-nhã, Pháp Hoa, Hoa Nghiêm, Tịnh độ… | 06 |
| Vinaya, giới, tăng đoàn, Prātimokṣa, Bồ-tát giới | 07 |
| Tantra, mật điển, mantra, sādhana, Tây Tạng | 08 |
| Trung Quốc, Triều Tiên, Nhật Bản, Việt Nam, Thiền/Tịnh độ/Thiên Thai/Hoa Nghiêm | 09 |
| Gāndhārī, Gandhāra, Khotan, Dunhuang, Trung Á, thủ bản | 10 |
| Dignāga, Dharmakīrti, pramāṇa, luận lý/nhận thức luận | 11 |
| Veda/Bà-la-môn, Jain, Ājīvika, khảo cổ, bia ký, lịch sử xã hội Ấn Độ | 12 |

Một câu hỏi có thể cần nhiều vùng. Chỉ ghép khi việc ghép đó có khả năng thay đổi kết luận.

---

# 4. VÙNG 01 — PHẬT GIÁO THỜI KỲ ĐẦU / NIKĀYA–ĀGAMA

**Dùng khi:** lời dạy sớm, “Đức Phật có nói không?”, so sánh kinh sớm, tiền bộ phái, lớp cổ, bản song hành.

**Corpus/ngôn ngữ:**
- Nikāya Pāli;
- Dīrgha/Madhyama/Saṃyukta/Ekottarika Āgama và kinh biệt dịch Hán;
- mảnh Sanskrit;
- Gāndhārī;
- Tạng khi có bản song hành liên quan;
- Vinaya cổ khi hỗ trợ so sánh.

**Hạ tầng gợi ý:** SuttaCentral, Pali Text Society, CBETA, SAT, GRETIL, Gandhari.org, BDRC/BUDA.

**Cần nhớ:**
- Pāli không mặc định là “bản gốc”;
- Āgama Hán không phải một khối đồng nhất;
- nhiều bản song hành có thể hỗ trợ một tổ tiên chung, không tự động chứng minh lời từng chữ của Đức Phật;
- câu hỏi phân tầng phải gọi `03_PHAN_TANG_VAN_BAN.md`.

---

# 5. VÙNG 02 — THERAVĀDA / PĀLI / CHÚ GIẢI

**Dùng khi:** Theravāda, Pāli Canon, Abhidhamma Pāli, Buddhaghosa, chú giải/hậu chú giải, lịch sử truyền thống Theravāda.

**Corpus/ngôn ngữ:**
- Nikāya và Vinaya Pāli;
- Abhidhamma Piṭaka;
- Aṭṭhakathā, ṭīkā;
- biên niên sử và văn học khu vực khi hỏi lịch sử truyền thống.

**Hạ tầng gợi ý:** SuttaCentral, PTS, GRETIL, thư viện số Pāli và các nhà xuất bản/tạp chí chuyên ngành.

**Cần nhớ:**
- tách Nikāya → Abhidhamma → chú giải → hậu chú giải;
- không chiếu khái niệm chú giải ngược vào kinh nếu kinh không có;
- “Theravāda” lịch sử không phải một khối đồng nhất xuyên mọi thế kỷ và khu vực.

---

# 6. VÙNG 03 — ABHIDHARMA VÀ CÁC BỘ PHÁI

**Dùng khi:** Sarvāstivāda, Vaibhāṣika, Sautrāntika, Dharmaguptaka, Mahāsāṃghika và các tranh luận bộ phái/Abhidharma.

**Corpus/ngôn ngữ:**
- Abhidharma các trường phái;
- Jñānaprasthāna, Mahāvibhāṣā và nguồn liên quan khi hỏi Sarvāstivāda/Vaibhāṣika;
- Sanskrit còn lại;
- Hán dịch quy mô lớn;
- Tạng khi bảo tồn nguồn/chú giải cần thiết;
- nguồn đối thủ, nhưng phải gắn nhãn.

**Hạ tầng gợi ý:** CBETA, SAT, GRETIL, DSBC, BDRC, INBUDS, J-STAGE, CiNii, DLMBS.

**Cần nhớ:**
- không đồng nhất Sarvāstivāda với Vaibhāṣika ở mọi giai đoạn;
- không dựng lập trường trường phái chỉ từ lời đối thủ;
- với nhiều đề tài, Hán văn là nguồn trung tâm chứ không phải “thứ cấp”.

---

# 7. VÙNG 04 — NĀGĀRJUNA / MADHYAMAKA

**Dùng khi:** Nāgārjuna, MMK, śūnyatā, duyên khởi, hai đế, lịch sử Madhyamaka.

**Corpus/ngôn ngữ:**
- Mūlamadhyamakakārikā;
- các tác phẩm gán cho Nāgārjuna với mức tác quyền nêu rõ;
- Sanskrit, Hán, Tạng;
- chú giải Ấn Độ/Hán/Tạng khi câu hỏi về lịch sử diễn giải.

**Hạ tầng gợi ý:** GRETIL, DSBC, CBETA, SAT, BDRC, 84000, INBUDS, CiNii/J-STAGE.

**Cần nhớ:**
- Nāgārjuna lịch sử ≠ toàn bộ Madhyamaka hậu kỳ;
- tác quyền phải kiểm thay vì tin toàn bộ attribution truyền thống;
- một bản dịch hiện đại không đủ cho câu hỏi phụ thuộc câu kệ/thuật ngữ.

---

# 8. VÙNG 05 — YOGĀCĀRA / TATHĀGATAGARBHA

**Dùng khi:** Asaṅga, Vasubandhu, Yogācāra, vijñaptimātra, trisvabhāva, ālayavijñāna, Như Lai tạng.

**Corpus/ngôn ngữ:**
- Yogācārabhūmi;
- Mahāyānasaṃgraha;
- Madhyāntavibhāga, Triṃśikā và các nguồn liên quan;
- Saṃdhinirmocana và các kinh Yogācāra;
- các kinh/luận tathāgatagarbha khi đúng câu hỏi;
- Sanskrit, Hán, Tạng.

**Hạ tầng gợi ý:** GRETIL, DSBC, CBETA, SAT, BDRC, 84000, DLMBS, INBUDS.

**Cần nhớ:**
- Yogācāra không nên giản lược ngay thành “duy tâm” trước khi xác định văn bản và nghĩa kỹ thuật;
- tathāgatagarbha và Yogācāra có vùng giao nhau nhưng không phải một hệ duy nhất;
- phân biệt tác phẩm Ấn Độ với tái diễn giải Đông Á/Tây Tạng.

---

# 9. VÙNG 06 — KINH ĐIỂN ĐẠI THỪA

**Dùng khi:** Bát-nhã, Pháp Hoa, Hoa Nghiêm, Vimalakīrti, Tịnh độ, Avataṃsaka, Mahāyāna sūtra nói chung.

**Corpus/ngôn ngữ:**
- Sanskrit/Buddhist Hybrid Sanskrit khi còn;
- Hán dịch nhiều lớp và nhiều dịch giả;
- Tạng;
- mảnh Trung Á/Gandhāra khi liên quan;
- catalog dịch thuật và lịch sử tiếp nhận.

**Hạ tầng gợi ý:** CBETA, SAT, GRETIL, DSBC, BDRC, 84000, BDK/Numata và các edition chuyên ngành.

**Cần nhớ:**
- “Đại thừa” không phải một corpus đồng thời;
- niên đại bản dịch không tự động bằng niên đại sáng tác;
- không dùng Pāli làm chuẩn cuối để phán tính hợp lệ của kinh Đại thừa;
- câu hỏi hình thành văn bản phải so recension và lịch sử dịch.

---

# 10. VÙNG 07 — VINAYA / GIỚI / TĂNG ĐOÀN

**Dùng khi:** giới luật, Prātimokṣa, lịch sử tăng đoàn, truyền giới, Bồ-tát giới, luật các bộ phái.

**Corpus/ngôn ngữ:**
- Pāli Vinaya;
- Dharmaguptaka, Mahīśāsaka, Mahāsāṃghika, Sarvāstivāda, Mūlasarvāstivāda Vinaya;
- Prātimokṣa và mảnh Sanskrit/Tạng/Hán;
- văn bản Bồ-tát giới khi câu hỏi thuộc Đại thừa/Đông Á.

**Hạ tầng gợi ý:** SuttaCentral, CBETA, SAT, GRETIL, BDRC, 84000.

**Cần nhớ:**
- không lấy một Vinaya làm “bản chuẩn” cho toàn tăng đoàn Phật giáo;
- truyện duyên khởi điều luật và chính điều luật có lịch sử truyền thừa khác nhau;
- Bồ-tát giới Đông Á cần kết hợp vùng 06 và 09 khi phù hợp.

---

# 11. VÙNG 08 — VAJRAYĀNA / TANTRA / TÂY TẠNG

**Dùng khi:** tantra, mantra, sādhana, maṇḍala, Guhyasamāja, Hevajra, Cakrasaṃvara, Kālacakra, Kangyur/Tengyur, lịch sử Phật giáo Tây Tạng.

**Corpus/ngôn ngữ:**
- Sanskrit tantric texts khi còn;
- Kangyur/Tengyur;
- chú giải Ấn Độ/Tạng;
- Dunhuang và tư liệu thủ bản khi liên quan;
- tiểu sử và lịch sử dòng truyền với phê bình nguồn.

**Hạ tầng gợi ý:** BDRC/BUDA, 84000, GRETIL, DSBC và catalog chuyên ngành.

**Cần nhớ:**
- Phật giáo Tây Tạng không đồng nhất với Vajrayāna; nhiều nguồn kinh/luận không phải tantra;
- tantra có nhiều lớp và hệ phân loại hậu kỳ khác nhau;
- truyền thống dòng truyền không tự động là biên niên sử phê bình;
- khi câu hỏi là cách một truyền thống Tây Tạng hiểu giáo lý, trước tác/chú giải Tây Tạng có thể là nguồn trực tiếp cho lịch sử diễn giải và không nên bị thay bằng tóm tắt của học giả phương Tây.

---

# 12. VÙNG 09 — PHẬT GIÁO ĐÔNG Á

**Dùng khi:** Trung Quốc, Triều Tiên, Nhật Bản, Việt Nam; Thiền/Chan/Zen, Thiên Thai, Hoa Nghiêm, Tịnh độ, Tam luận, Pháp tướng, Bồ-tát giới Đông Á.

**Corpus/ngôn ngữ:**
- Hán tạng;
- catalog kinh điển;
- chú sớ và trước tác bản địa;
- văn bia, ngữ lục, thanh quy, sử truyện;
- Hàn/Nhật/Việt khi câu hỏi thuộc lịch sử khu vực.

**Hạ tầng gợi ý:** CBETA, SAT, DDB, INBUDS, CiNii, J-STAGE, DLMBS và các bộ sưu tập số khu vực.

**Cần nhớ:**
- attribution “dịch từ Sanskrit” cần kiểm catalog và nghiên cứu văn bản;
- “kinh ngụy” là phân loại lịch sử/thư mục, không phải phán xét giá trị;
- không đồng nhất tiếp nhận Đông Á với nghĩa gốc Ấn Độ của văn bản;
- scholarship Trung Quốc/Đài Loan và Nhật Bản có thể là nghiên cứu văn bản–lịch sử trung tâm của đề tài, không chỉ là “tiếp nhận khu vực”.

---

# 13. VÙNG 10 — GANDHĀRA / TRUNG Á / THỦ BẢN

**Dùng khi:** Gāndhārī, Kharoṣṭhī, Gandhāra, Bamiyan, Gilgit, Khotan, Dunhuang, Tocharian/Sogdian/Khotanese, mảnh thủ bản, Con đường Tơ lụa.

**Corpus/ngôn ngữ:**
- Gāndhārī manuscripts;
- Sanskrit Buddhist manuscripts;
- Khotanese, Tocharian, Sogdian khi liên quan;
- Hán/Tạng trong lịch sử truyền bá;
- dữ liệu cổ tự học và lịch sử vật mang.

**Hạ tầng gợi ý:** Gandhari.org, International Dunhuang Programme, BDRC, GRETIL/DSBC và các catalog thủ bản chuyên ngành.

**Cần nhớ:**
- niên đại vật mang ≠ niên đại sáng tác nội dung;
- provenance và hoàn cảnh khai quật/mua bán ảnh hưởng giá trị lịch sử;
- fragment ngắn không cho phép khái quát toàn văn nếu không có cơ sở.

---

# 14. VÙNG 11 — LUẬN LÝ VÀ NHẬN THỨC LUẬN

**Dùng khi:** Dignāga, Dharmakīrti, pramāṇa, pratyakṣa, anumāna, apoha, hetu, tranh luận luận lý/nhận thức luận.

**Corpus/ngôn ngữ:**
- Pramāṇasamuccaya và truyền thống chú giải;
- Pramāṇavārttika và các tác phẩm Dharmakīrti;
- mảnh/edition Sanskrit;
- Tạng và Hán khi bảo tồn cần thiết;
- nguồn Nyāya, Mīmāṃsā, Jain khi là đối thoại trực tiếp.

**Hạ tầng gợi ý:** GRETIL, DSBC, BDRC và các critical edition/repository chuyên ngành.

**Cần nhớ:**
- thuật ngữ luận lý cần đọc đúng hệ thống và ngữ cảnh;
- không đồng nhất thuật ngữ cùng hình thức giữa các trường phái;
- nguồn đối thủ phải tách khỏi tự thuật Phật giáo.

---

# 15. VÙNG 12 — BỐI CẢNH ẤN ĐỘ / LIÊN TÔN / KHẢO CỔ

**Dùng khi:** Veda/Brahmanism, Upaniṣad, Jain, Ājīvika, śramaṇa, Aśoka, bia ký, khảo cổ, lịch sử xã hội, thương mại, tự viện, bảo trợ.

**Corpus/ngôn ngữ:**
- Vedic/Classical Sanskrit;
- Pāli/Prakrit;
- Jain Prakrit;
- Aśokan Prakrit, Greek/Aramaic khi liên quan;
- bia ký, coins, reliquaries, stūpa, monastery archaeology;
- sử liệu du hành và nguồn ngoài Phật giáo.

**Hạ tầng gợi ý:** GRETIL, corpus/edition bia ký chuyên ngành, Gandhari.org khi vùng Tây Bắc liên quan, CBETA/SAT cho sử liệu Hán, các ấn phẩm khảo cổ học, repository và nhà xuất bản chuyên về Indology/Vedic Studies khi phù hợp.

**Cần nhớ:**
- tương đồng khái niệm ≠ tự động là vay mượn;
- “Upaniṣad” không phải một khối đồng thời;
- văn bản, bia ký và khảo cổ là các loại chứng cứ khác nhau;
- không dùng văn bản hậu kỳ như cửa sổ trực tiếp vào thế kỷ V TCN nếu chưa biện minh;
- nếu claim thực chất nói về nghĩa, niên đại, lớp văn bản hoặc lịch sử tư tưởng của Veda/Upaniṣad/Brahmanism, phải kiểm scholarship chuyên ngành Vedic Studies/Upaniṣadic Studies/Indology hoặc lịch sử tôn giáo Ấn Độ; một Buddhist Studies work tóm tắt các văn bản ấy không tự động thay thế được chuyên môn này.

---

# 16. HỌC GIỚI ĐA NGÔN NGỮ VÀ ĐA TRUYỀN THỐNG NGHIÊN CỨU

Nguyên tắc trung tâm:

> **KHÔNG COI SCHOLARSHIP TIẾNG ANH LÀ ĐẠI DIỆN MẶC ĐỊNH CHO TOÀN BỘ HỌC GIỚI QUỐC TẾ.**

Khi đề tài phụ thuộc trực tiếp vào một corpus, ngôn ngữ, vùng truyền thừa hoặc lịch sử nghiên cứu, phải chủ động kiểm các tuyến học giới có năng lực và đóng góp đáng kể cho chính đề tài đó nếu chúng có khả năng làm đổi, bổ sung hoặc giới hạn kết luận.

Tùy đề tài, có thể cần các truyền thống/tuyến nghiên cứu Nhật, Hoa/Đài Loan, Hàn, Pháp/Bỉ, Anh/Đức, Nga/Ba Lan, Nam Á, Tây Tạng hoặc các tuyến khác. Đây không phải danh sách đóng và không có học giới quốc gia nào mặc định “cao hơn” học giới khác.

Đặc biệt:
- với Phật giáo Đông Á, nghiên cứu Trung Quốc/Đài Loan và Nhật Bản có thể là scholarship văn bản–lịch sử hàng đầu, không chỉ là tài liệu về “tiếp nhận khu vực”;
- với Phật giáo Tây Tạng, cần phân biệt nguồn scholastic Tạng trực tiếp với scholarship hiện đại về Tây Tạng; không để bản tóm tắt phương Tây thay thế nguồn Tạng khi chính cách hiểu của truyền thống là đối tượng nghiên cứu;
- với Abhidharma, Madhyamaka, Yogācāra, logic, lịch sử kinh điển hoặc manuscript studies, các truyền thống nghiên cứu Pháp/Bỉ, Anh/Đức, Nga/Ba Lan, Nhật hoặc Hoa có thể chứa những công trình nền tảng mà literature tiếng Anh đương đại chỉ dẫn lại;
- với Veda/Upaniṣad/Brahmanism hoặc lĩnh vực ngoài Buddhist Studies, phải mở sang học giới chuyên ngành tương ứng thay vì chỉ dùng Buddhist scholars mô tả lĩnh vực đó.

Một bài tiếng Anh tóm tắt nghiên cứu Nhật/Hoa/Nga/Pháp không đồng nghĩa đã khảo sát chính học giới đó. Nếu công trình gốc có thể truy hợp lý và claim quan trọng, áp dụng `02_NGUON_VA_CHUNG_CU.md` để truy tiếp. Nếu không truy được, nêu rõ giới hạn thay vì mô tả như đã kiểm trực tiếp.

Không có quota quốc gia hay quota ngôn ngữ. Chỉ mở nhánh khi nó có khả năng hợp lý thay đổi câu trả lời, làm rõ lịch sử tranh luận hoặc ngăn thiên lệch do chỉ nhìn một hệ học thuật.

---

# 17. CÁCH DÙNG HẠ TẦNG

Tên platform ở đây chỉ là nơi **định vị**.

Sau khi tìm được item:
- xác định text/edition thực;
- xác định dịch giả/biên tập viên;
- kiểm provenance nếu là manuscript;
- kiểm bài/sách cụ thể nếu là scholarship.

Không biến Source Map thành danh sách website “được phép tin”.

---

# 18. CÔNG THỨC MAP v3.1

> **XÁC ĐỊNH ĐỀ TÀI → CHỌN 1–3 VÙNG THẬT SỰ LIÊN QUAN → ƯU TIÊN HẠ TẦNG CHUYÊN NGÀNH → MỞ CORPUS/NGÔN NGỮ/HỌC GIỚI/NGÀNH CHUYÊN MÔN CẦN THIẾT → TÌM ITEM → TRUY NGUỒN GỐC KHI MỆNH ĐỀ QUAN TRỌNG → THẨM ĐỊNH ITEM BẰNG `02_NGUON_VA_CHUNG_CU.md`.**

Bản đồ chỉ giúp đi đúng hướng. Chứng cứ thật mới quyết định kết luận.