# BỘ KIỂM THỬ HỒI QUY — PHAT-HOC 3.0

**Phiên bản:** 3.0  
**Dấu hiệu:** `PHAT-HOC-3.0-REGRESSION`  
**Mục tiêu:** Kiểm tra hành vi thực tế của Trợ lý Nghiên cứu Phật học v3 trong ChatGPT Project sau khi đã cài Project Instructions và 17 tệp nguồn.

---

# 0. NGUYÊN TẮC CHẠY TEST

1. Mỗi test phải chạy trong **chat mới** của Project TEST, trừ khi test ghi rõ là nhiều lượt.
2. Không thêm câu như “hãy áp dụng skill”, “hãy nghiên cứu sâu”, “hãy tìm nguồn” nếu đề bài test không có. Mục tiêu là kiểm khả năng **tự kích hoạt**.
3. Khi test là câu hỏi thực chứng/lịch sử, đánh giá cả **cách dùng nguồn**, không chỉ nội dung kết luận.
4. Không xem câu trả lời dài hoặc có nhiều citation là tự động tốt.
5. Chấm theo `TIEU_CHI_CHAM_TEST.md`.
6. Nếu một test thất bại, phải xác định lỗi thuộc lớp nào trước khi sửa: Instructions, core, Source Map, module, protocol phân tầng, quy chuẩn nguồn hay hậu kiểm.
7. Không sửa Source Map chỉ để vượt một ca đơn lẻ nếu thay đổi không có giá trị lặp lại.
8. Nếu công cụ tra cứu không khả dụng trong lượt test, hành vi đúng là **nêu giới hạn**, không giả vờ đã kiểm nguồn.

---

# NHÓM A — TỰ KÍCH HOẠT, ĐỘ SÂU VÀ ĐỊNH TUYẾN

## Test 01 — Câu cực ngắn

### Đề bài
`anattā?`

### Kỳ vọng
- Tự nhận diện là thuật ngữ Phật học; không hỏi người dùng có muốn áp dụng bộ quy tắc không.
- Trả lời gọn, rõ bằng tiếng Việt; có thể nêu *anattā/anātman* khi hữu ích.
- Không phô Stage, router, tên file hay nhật ký nội bộ.
- Không biến một câu khái niệm đơn giản thành báo cáo dài không cần thiết.
- Nếu mở khác biệt truyền thống, phải nêu đúng phạm vi thay vì mặc định toàn Phật giáo = Theravāda.

### Dấu hiệu FAIL
- “Bạn muốn tôi nghiên cứu sâu không?”
- Chỉ định nghĩa theo chú giải Theravāda rồi gọi đó là toàn bộ Phật giáo.
- Xuất tên các file phương pháp như citation.

---

## Test 02 — Tên kinh mơ hồ

### Đề bài
`Phạm Võng kinh có cổ không?`

### Kỳ vọng
- Phát hiện ít nhất hai đối tượng nổi bật: Brahmajāla Sutta/DN 1 và 梵網經/T1484.
- Không âm thầm chọn một nghĩa rồi nghiên cứu như chắc chắn.
- Có thể trả lời phân biệt hai trường hợp mà không cần hỏi lại nếu làm được rõ ràng.
- Nếu đưa kết luận lịch sử, phải kiểm nguồn thích hợp.

### Dấu hiệu FAIL
- Chọn T1484 hoặc DN 1 làm nghĩa duy nhất mà không cảnh báo.
- Dẫn chính file skill làm chứng cứ.

---

## Test 03 — Độ ngắn không làm giảm độ sâu

### Đề bài
`T1484 do Kumārajīva dịch thật không?`

### Kỳ vọng
- Tự nhận ra đây là câu hỏi tác quyền/lịch sử văn bản, cần nghiên cứu sâu hơn độ dài câu hỏi.
- Định tuyến hợp lý sang Đại thừa + Đông Á, và Vinaya/Bồ-tát giới nếu cần.
- Phân biệt attribution truyền thống/mục lục với kết luận lịch sử hiện đại.
- Ưu tiên công trình trực tiếp và nguồn mục lục/văn bản phù hợp thay vì chỉ trang tổng hợp.
- Không tuyên bố “học giới đồng thuận” nếu chưa đủ bao phủ.

---

## Test 04 — Đề tài ngoài Map không bị ép sai

### Đề bài
`Khảo sát lịch sử hình thành Phật giáo hiện đại ở Brazil và sự tiếp nhận Thiền Nhật Bản tại đó.`

### Kỳ vọng
- Nhận ra Source Map hiện tại không có mô-đun chuyên cho Phật giáo hiện đại ở Mỹ Latinh.
- Không ép đề tài vào “Phật giáo Đông Á” như thể module 09 bao phủ toàn bộ lịch sử Brazil.
- Dùng core + quy chuẩn nguồn để tự xác lập phạm vi mở có kiểm soát; module 09 chỉ có thể là nhánh phụ cho phần Thiền Nhật Bản.
- Không bịa module mới như thể đã tồn tại.

---

# NHÓM B — PHẠM VI, Ý ĐỊNH NGƯỜI DÙNG VÀ GIẢ THUYẾT

## Test 05 — Phạm vi đóng tuyệt đối

### Đề bài
`Chỉ dùng năm Nikāya Pāli. Giải thích anattā trong phạm vi đó; không dùng Āgama, Abhidhamma, chú giải hay học giả hiện đại làm chứng cứ.`

### Kỳ vọng
- Nhận diện phạm vi đóng.
- Không đưa Āgama, Abhidhamma, chú giải hoặc học giả hiện đại vào lập luận chứng minh.
- Có thể dùng hạ tầng để định vị chính năm Nikāya.
- Nếu phạm vi không đủ cho một kết luận, nói rõ giới hạn thay vì phá khóa.

### Lỗi nghiêm trọng
Dùng nguồn ngoài phạm vi để củng cố kết luận mà không được người dùng cho phép.

---

## Test 06 — “Chủ yếu” không đồng nghĩa “chỉ”

### Đề bài
`Tôi muốn tham khảo chủ yếu MMK và vài bài kinh Nikāya để xem Nāgārjuna có tiếp nối duyên khởi trong kinh hay không.`

### Kỳ vọng
- Nhận diện phạm vi mở có kiểm soát, không khóa cứng.
- Định tuyến 01 + 04.
- Cho phép bản dịch/truyền bản và nghiên cứu trực tiếp cần thiết nếu ảnh hưởng kết luận.
- Không mở vô hạn toàn bộ Đại thừa hoặc mọi Abhidharma.
- “Nāgārjuna tiếp nối” là giả thuyết cần kiểm, không phải kết luận sẵn.

---

## Test 07 — Trung lập hóa câu hỏi dẫn dắt

### Đề bài
`Đoạn này rõ ràng là người đời sau thêm vào phải không?`

### Kỳ vọng
- Không thuận theo giả định chỉ vì người dùng nói “rõ ràng”.
- Yêu cầu/xác định đoạn và văn bản nếu chưa đủ dữ liệu.
- Chuyển thành câu hỏi về lịch sử hình thành và chứng cứ.
- Không dùng “thêm sau” như điểm xuất phát bắt buộc.

---

## Test 08 — Thuật ngữ lịch sử mơ hồ

### Đề bài
`Phật giáo nguyên thủy có chủ trương chỉ hiện tại thực hữu không?`

### Kỳ vọng
- Không đồng nhất “Phật giáo nguyên thủy” với Theravāda, Nikāya hay tiền bộ phái một cách âm thầm.
- Làm rõ hoặc phân biệt các nghĩa có thể dùng.
- Nếu liên quan Sarvāstivāda/Abhidharma, không nhập chúng vào “nguyên thủy” mà phải phân tầng lịch sử.
- Định tuyến theo câu hỏi sau khi gỡ mơ hồ.

---

# NHÓM C — QUẢN TRỊ NGUỒN VÀ MỨC TRUY CẬP

## Test 09 — Abstract không phải toàn văn

### Đề bài
`Nếu bạn chỉ truy cập được abstract của một bài nghiên cứu, bạn có được viết “tác giả đã chứng minh rằng X” không?`

### Kỳ vọng
- Trả lời không.
- Phân biệt mức truy cập D/định vị với đọc trực tiếp phần lập luận.
- Có thể nói “abstract cho biết công trình khảo sát/đề xuất...” ở mức phù hợp.
- Không suy chi tiết phương pháp hoặc kết luận vượt abstract.

---

## Test 10 — Hạ tầng không phải tác giả

### Đề bài
`CBETA nói Phạm Võng T1484 là kinh ngụy phải không?`

### Kỳ vọng
- Sửa khung câu hỏi: CBETA là hạ tầng truy cập, không phải tác giả/phán quyết học thuật.
- Truy về văn bản mục lục, ghi chú catalog hoặc công trình học thuật cụ thể nếu cần.
- Không viết “CBETA chứng minh...” hoặc “CBETA cho rằng...”.

---

## Test 11 — Năm citation không đồng nghĩa năm chứng cứ độc lập

### Đề bài
`Tôi có 5 bài nghiên cứu đều nói cùng một điều, nhưng cả 5 đều dẫn lại cùng một công trình cũ. Có thể coi là 5 chứng cứ độc lập không?`

### Kỳ vọng
- Trả lời không.
- Giải thích phụ thuộc nguồn/chains of citation.
- Phân biệt số lượng citation với số chứng cứ độc lập.
- Nếu đánh giá “đồng thuận”, phải xét mức độ độc lập và bao phủ.

---

## Test 12 — “Đồng thuận học giới” phải được kiểm

### Đề bài
`Có phải học giới đều đồng ý rằng T1484 được biên soạn ở Trung Quốc không?`

### Kỳ vọng
- Không chấp nhận từ “đều” mà không kiểm.
- Tìm nhiều công trình độc lập hoặc tổng quan chuyên ngành phù hợp.
- Phân biệt: chất lượng công trình, mức phổ biến quan điểm, độ chắc chắn của mệnh đề.
- Nếu chỉ kiểm được vài tác giả, viết “một số nghiên cứu/học giả...” và nêu giới hạn bao phủ.

---

# NHÓM D — PHÂN TẦNG VĂN BẢN VÀ LỊCH SỬ HÌNH THÀNH

## Test 13 — Vắng ở một truyền bản

### Đề bài
`Nếu một đoạn chỉ có trong bản Pāli mà không có trong truyền bản Hán song song, có thể kết luận ngay là thêm về sau không?`

### Kỳ vọng
- Trả lời không.
- Công thức an toàn: hiện đoạn này chỉ được chứng thực ở Pāli, nếu dữ liệu đúng.
- Cần thêm cấu trúc, ngữ văn, các truyền bản khác, lịch sử biên tập, nghiên cứu chuyên ngành.
- Không biến vắng mặt thành bằng chứng quyết định.

---

## Test 14 — Ngắn hơn không tự động cổ hơn

### Đề bài
`Hai bản song song, bản Hán ngắn hơn bản Pāli. Có phải bản Hán chắc chắn cổ hơn?`

### Kỳ vọng
- Trả lời không.
- Nêu các khả năng: mở rộng, rút gọn, dịch thuật, truyền khẩu, biên tập dòng truyền, mất văn bản.
- Chỉ kết luận hướng biến đổi khi có tổ hợp chứng cứ.

---

## Test 15 — Phạm Võng DN 1

### Đề bài
`Phạm Võng kinh trong Trường Bộ có phải là một bài kinh rất sớm không?`

### Kỳ vọng
- Tự kích hoạt protocol phân tầng.
- Không coi toàn bộ DN 1 Pāli hiện nay là một khối đồng niên.
- Tìm các truyền bản song hành phù hợp và nghiên cứu trực tiếp.
- Phân biệt lõi/chứng thực sớm với nguyên văn từng chữ của Đức Phật.
- Nếu phán phần nào mở rộng, phải nêu chứng cứ và mức chắc chắn.

---

## Test 16 — “Đức Phật có nói thật không?”

### Đề bài
`Đức Phật có thật sự nói “sabbe dhammā anattā” không?`

### Kỳ vọng
- Không trả lời nhị phân “có/chắc chắn” chỉ vì câu xuất hiện trong Pāli.
- Xác định nguồn/locus chính xác trước.
- Tìm chứng thực song hành hoặc lịch sử truyền bản khi khả dụng.
- Phân biệt “được chứng thực sớm”, “có khả năng thuộc lớp sớm” và “nguyên văn từng chữ của Đức Phật lịch sử”.
- Không back-translate rồi gọi là nguyên văn.

---

# NHÓM E — ĐA TRUYỀN THỐNG, ĐA NGÔN NGỮ VÀ ROUTER

## Test 17 — Sarvāstivāda không chỉ qua tiếng Anh

### Đề bài
`Khảo sát học thuyết ba thời của Sarvāstivāda và lịch sử nghiên cứu hiện đại về học thuyết này.`

### Kỳ vọng
- Module 03 là tuyến chính.
- Nhận diện nguồn Hán Abhidharma quan trọng khi phù hợp.
- Không chỉ dựa nghiên cứu tiếng Anh nếu Nhật/Hoa có đóng góp trực tiếp.
- Không đặt quota quốc gia.
- Nếu không truy được nhánh quan trọng, ghi giới hạn bao phủ.

---

## Test 18 — Yogācāra không bị giản lược thành “duy tâm”

### Đề bài
`Yogācāra có phải là duy tâm cho rằng chỉ có tâm tồn tại không?`

### Kỳ vọng
- Định tuyến module 05.
- Không dùng một nhãn triết học phương Tây như kết luận sẵn.
- Phân biệt văn bản, tác giả, giai đoạn và các cách diễn giải cạnh tranh.
- Nếu nói về vijñaptimātra/cittamātra, phải làm rõ ngữ cảnh và không đại diện toàn Yogācāra bằng một khẩu hiệu.

---

## Test 19 — Đại thừa không bị xử lý theo khung “thật/giả” đơn giản

### Đề bài
`Kinh Đại thừa đều là người sau bịa thêm phải không?`

### Kỳ vọng
- Trung lập hóa ngôn ngữ “bịa”.
- Phân biệt niên đại, lịch sử hình thành, attribution truyền thống, chức năng tôn giáo và giá trị lịch sử.
- Không dùng “muộn = giả mạo”.
- Nếu câu hỏi chung, module 06 là chính nhưng phải chọn corpus cụ thể trước khi kết luận lịch sử chi tiết.

---

## Test 20 — Guhyasamāja cần đúng router

### Đề bài
`Khảo sát nguồn gốc và các lớp văn bản của Guhyasamāja Tantra.`

### Kỳ vọng
- Định tuyến module 08 + protocol phân tầng; module 10 hoặc 12 chỉ nếu chứng cứ thực tế đòi hỏi.
- Không xử lý tantra như một khối đồng nhất.
- Phân biệt Sanskrit/Tạng, lịch sử dịch, truyền bản và chú giải.
- Không coi Kangyur/Tengyur là “nguồn gốc” thay cho item cụ thể.

---

# NHÓM F — THỦ BẢN, KHẢO CỔ, DỊCH THUẬT VÀ ĐẦU RA

## Test 21 — Niên đại thủ bản ≠ niên đại sáng tác

### Đề bài
`Nếu một bản chép Gāndhārī được định niên đại thế kỷ I CN thì có nghĩa bài kinh được sáng tác ở thế kỷ I CN phải không?`

### Kỳ vọng
- Trả lời không.
- Phân biệt niên đại vật mang/manuscript với niên đại nội dung hoặc tiền thân văn bản.
- Module 10 là chính; module 01 nếu là kinh sớm.
- Không dùng niên đại carbon/paleography của vật mang để định niên đại tuyệt đối của toàn nội dung.

---

## Test 22 — Bia ký và văn bản là hai loại chứng cứ

### Đề bài
`Bia Aśoka không nhắc một giáo lý nào đó thì có chứng minh giáo lý ấy chưa tồn tại không?`

### Kỳ vọng
- Không biến sự im lặng của bia ký thành phủ định tuyệt đối.
- Phân biệt mục đích/chức năng corpus bia ký với corpus kinh điển.
- Module 12; mở module khác nếu giáo lý cụ thể cần.
- Đánh giá absence với xác suất bảo tồn và phạm vi thể loại.

---

## Test 23 — Tiếng Việt sạch và không phô nội bộ

### Đề bài
`Giải thích ngắn gọn cách phân tầng một bài kinh. Không dùng từ tiếng Anh nếu tiếng Việt có thể diễn đạt được.`

### Kỳ vọng
- Tiếng Việt tự nhiên, nhất quán.
- Không lộ tên Stage, marker, tên file, checklist nội bộ.
- Không có `&#x20;`, `&nbsp;`, `\n` lộ ra hoặc placeholder kỹ thuật.
- Có các ý cốt lõi: chia đơn vị, đối chiếu truyền bản, cấu trúc/ngữ văn/lịch sử, tổ hợp chứng cứ, mức chắc chắn.

---

## Test 24 — Không trích file phương pháp như chứng cứ

### Đề bài
`Phạm Võng DN 1 có phần mở rộng muộn không? Hãy cho nguồn.`

### Kỳ vọng
- Citation/chứng cứ phải là văn bản, bản song hành hoặc công trình học thuật thực tế.
- Không trích `PHUONG_PHAP_NGHIEN_CUU_COT_LOI.md`, `QUY_TRINH_PHAN_TANG_VAN_BAN.md`, Source Map hay Project Instructions như bằng chứng rằng DN 1 có lớp muộn.
- Các file phương pháp chỉ được nhắc nếu người dùng hỏi chính về cách nghiên cứu.

### Lỗi nghiêm trọng
Tên file skill xuất hiện như citation nội dung Phật học.

---

# 1. BÀI NEO HỒI QUY SO VỚI v2

Bốn test sau là **neo bắt buộc**, vì chúng trực tiếp phản ánh các vấn đề đã thấy khi xây v2:

- Test 02 — `Phạm Võng kinh có cổ không?` → phải xử lý mơ hồ tốt hơn v2.
- Test 15 — DN 1 có rất sớm không? → phải giữ được chất lượng phân tầng đã đạt ở v2.
- Test 12 — “học giới đều…” → v3 phải thận trọng hơn về đồng thuận và bao phủ.
- Test 24 — không được để tên file phương pháp chen vào citation như đã từng xảy ra.

Nếu một trong bốn test neo từ PASS ở baseline xuống FAIL ở v3, coi là **hồi quy nghiêm trọng** dù tổng điểm vẫn cao.

---

# 2. MA TRẬN BAO PHỦ TĨNH

Bảng này chỉ kiểm **rule coverage trong thiết kế**, không thay test hành vi runtime.

| Test | Lớp quy tắc chính |
|---|---|
| 01 | Project Instructions + Core |
| 02 | Core + Router + 01/06/09 tùy nghĩa |
| 03 | Core + Source Gov + 06/09 + Audit |
| 04 | Router ngoài Map + Core + Source Gov |
| 05 | Core phạm vi đóng + Source Gov |
| 06 | Core phạm vi mở có kiểm soát + 01 + 04 |
| 07 | Core trung lập hóa + Stratification |
| 08 | Core gỡ mơ hồ + 01/03 tùy nghĩa |
| 09 | Source Gov + Audit |
| 10 | Source Gov + Audit |
| 11 | Source Gov tính độc lập + Audit |
| 12 | Source Gov đồng thuận + Audit |
| 13 | Stratification + 01 |
| 14 | Stratification + 01 |
| 15 | Stratification + 01 + Audit |
| 16 | Stratification + 01 + Source Gov |
| 17 | 03 + Source Gov đa ngôn ngữ |
| 18 | 05 + Core |
| 19 | 06 + Core + Stratification khi cần |
| 20 | 08 + Stratification + Source Gov |
| 21 | 10 + 01 + Stratification |
| 22 | 12 + Source Gov |
| 23 | Project Instructions + Audit |
| 24 | Source Gov + Audit + Stratification |

**Kết quả kiểm bao phủ tĩnh ở thời điểm viết bộ test:** 24/24 test đều có quy tắc sở hữu rõ trong v3. Điều này chỉ cho thấy thiết kế có rule tương ứng; chỉ chạy trong ChatGPT Project mới xác nhận được retrieval và hành vi thực tế.

---

# 3. CÁCH GHI KẾT QUẢ

Cho mỗi test ghi:

- **Điểm:** 0 / 1 / 2 / 3
- **Trạng thái:** PASS / PARTIAL / FAIL
- **Lỗi chính:** một câu ngắn
- **Lớp sở hữu lỗi:** Instructions / Core / Source Gov / Router / Module / Stratification / Audit / Retrieval / Tool limitation
- **Có phải lỗi nghiêm trọng không:** Có/Không
- **Sửa đề xuất:** nếu cần

Mẫu:

```text
Test 15 — Điểm 2/3 — PARTIAL
Lỗi: Có tìm song hành nhưng dùng một bài tổng hợp thay cho công trình trực tiếp.
Chủ sở hữu: Source Gov / Retrieval
Nghiêm trọng: Không
Sửa: tăng ưu tiên nguồn học thuật trực tiếp trước nguồn tổng hợp.
```

---

# 4. NGUYÊN TẮC KHÔNG “DẠY TỦ” THEO TEST

Không được sửa Project Instructions thành danh sách 24 câu hỏi này.

Mục tiêu regression là đo **nguyên tắc tổng quát**. Một sửa đổi chỉ hợp lệ khi:
- giải quyết lớp lỗi tổng quát;
- không làm prompt phình vô ích;
- không phá phạm vi hoặc router khác;
- có khả năng cải thiện nhiều ca tương tự.

Nếu chỉ một test quá đặc thù thất bại, ưu tiên sửa module hoặc test expectation trước khi nhồi thêm luật vào Instructions.

---

# 5. THỨ TỰ CHẠY KHUYẾN NGHỊ

Để phát hiện lỗi sớm, chạy theo thứ tự:

1. Test 01, 02, 05 — activation, ambiguity, closed scope.
2. Test 09, 10, 11, 12 — source governance.
3. Test 13, 14, 15, 16 — stratification.
4. Test 17–22 — router chuyên ngành và đa chứng cứ.
5. Test 23, 24 — đầu ra và leakage.
6. Cuối cùng chạy 03, 04, 06, 07, 08 như stress test định tuyến/phạm vi.

Nếu test 05, 09, 13 hoặc 24 FAIL nghiêm trọng, nên dừng vòng test và sửa trước khi tiếp tục chấm tổng thể.
