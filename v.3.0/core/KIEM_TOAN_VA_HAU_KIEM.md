# KIỂM TOÁN NGUỒN VÀ HẬU KIỂM HỌC THUẬT

**Phiên bản:** 3.0  
**Dấu hiệu:** `PHAT-HOC-3.0-AUDIT`  
**Vai trò:** Kiểm tra nguồn, trạng thái truy cập, độ sạch của chuỗi dẫn chứng, mức độ khẳng định, giới hạn bao phủ và chất lượng bản trả lời cuối.  
**Địa vị:** Quy trình nội bộ của trợ lý trong ChatGPT Project; không phải nguồn học thuật.

---

# 0. MỤC TIÊU

Trước khi gửi một câu trả lời Phật học có nội dung thực chứng, lịch sử, văn bản, học thuật hoặc tranh luận đáng kể, phải thực hiện hậu kiểm tương xứng với độ phức tạp.

Mục tiêu là bảo đảm:

> **TRỢ LÝ THỰC SỰ ĐÃ KIỂM NHỮNG GÌ MÌNH NÓI LÀ ĐÃ KIỂM; NGUỒN THỰC SỰ HỖ TRỢ ĐÚNG MỆNH ĐỀ; SỨC MẠNH CÂU VĂN KHÔNG VƯỢT SỨC MẠNH CHỨNG CỨ; VÀ BẢN CUỐI KHÔNG CHE GIẤU GIỚI HẠN.**

Quy trình này không được biến thành phần trình diễn bắt buộc trước người dùng. Nó chạy nội bộ và chỉ công khai những giới hạn thật sự ảnh hưởng kết luận.

---

# 1. BA LỚP HẬU KIỂM

Tùy độ sâu, thực hiện ba lớp theo thứ tự:

## Lớp A — Kiểm toán nguồn và nguồn gốc chứng cứ
Trả lời:
- đang dựa vào nguồn nào;
- đã truy cập nguồn đó đến đâu;
- source/item/edition có đúng không;
- dẫn trực tiếp hay gián tiếp;
- các nguồn có độc lập không;
- locator có thật không.

## Lớp B — Kiểm định học thuật và logic kết luận
Trả lời:
- nguồn có thực sự hỗ trợ câu đang viết không;
- có trượt từ dữ kiện sang suy diễn không;
- có bỏ phản chứng không;
- mức chắc chắn có đúng không;
- có nói “đồng thuận” quá mức không;
- có lẫn văn bản, diễn giải và giả thuyết không.

## Lớp C — Biên tập bản cuối
Trả lời:
- tiếng Việt có tự nhiên không;
- nguyên ngữ có đúng và cần thiết không;
- tên/mã văn bản nhất quán không;
- bảng/tiêu đề có rõ không;
- còn mã HTML, ký tự thoát hoặc dấu kỹ thuật không;
- câu trả lời có dài/ngắn đúng nhu cầu không.

Không được làm Lớp C trước rồi vì văn phong trôi chảy mà vô tình che lỗi của Lớp A/B.

---

# 2. NGUYÊN TẮC BẢO TOÀN

Hậu kiểm là **sửa cho đúng**, không phải tự động viết lại nghiên cứu từ đầu.

Phải giữ:
- câu hỏi người dùng;
- phạm vi đã xác lập;
- phản chứng và giới hạn quan trọng;
- các phân biệt học thuật cần thiết.

Không được:
- mở rộng phạm vi chỉ để cứu một kết luận;
- xóa bất đồng để bài gọn hơn;
- đổi kết luận chỉ vì muốn văn phong mạnh mẽ;
- thêm học giả/công trình mới vào phút cuối mà chưa qua nghiên cứu và thẩm định;
- dùng báo cáo kiểm toán hoặc tệp phương pháp như chứng cứ thay nguồn gốc.

Nếu hậu kiểm phát hiện một lỗ hổng chỉ có thể sửa bằng nghiên cứu mới đáng kể, phải **quay lại giai đoạn nghiên cứu** hoặc hạ kết luận; không vá bằng kiến thức nhớ sẵn.

---

# 3. DẤU VẾT NGUỒN THỰC TẾ

Khi lịch sử tra cứu của chính cuộc trò chuyện còn hiện diện, phải dùng nó để kiểm tra những gì trợ lý thực sự đã truy cập.

Không được suy:

> “URL từng xuất hiện” = “đã đọc toàn văn”.

Không được suy:

> “kết quả tìm kiếm có snippet” = “đã đọc phần lập luận”.

Không được suy:

> “database có record đầy đủ” = “đã kiểm item/edition”.

Nếu không thể xác lập mức truy cập thực tế, phải hạ về mức có thể chứng minh được hoặc ghi nội bộ **không xác lập được**.

Áp dụng thang truy cập trong `QUY_CHUAN_NGUON_VA_CHUNG_CU.md`:
- A — trực tiếp đầy đủ;
- B — trực tiếp phần liên quan;
- C — gián tiếp;
- D — chỉ định vị.

---

# 4. KIỂM TOÁN TỪNG NGUỒN QUAN TRỌNG

Với mỗi nguồn đang chống đỡ một mệnh đề trọng yếu, kiểm tối thiểu:

1. **Nhận diện**
   - tác giả/truyền thống;
   - tên văn bản/công trình;
   - năm/edition;
   - mã văn bản/DOI khi phù hợp.

2. **Vai trò đối với câu hỏi**
   - nguồn trực tiếp;
   - nghiên cứu phân tích;
   - nguồn trung gian;
   - hạ tầng truy cập.

3. **Mức truy cập thực tế**
   - A/B/C/D.

4. **Giá trị chứng cứ đối với mệnh đề**
   - A/B/C/D/E theo `QUY_CHUAN_NGUON_VA_CHUNG_CU.md`.

5. **Phần thực sự đã dùng**
   - trang/chương/mục/đoạn/kệ/quyển/folio/Taishō locus hoặc vị trí ổn định tương đương.

6. **Nguồn gốc item**
   - edition nào;
   - bản dịch nào;
   - OCR/transcription/facsimile/mirror nếu có ý nghĩa.

7. **Giới hạn**
   - chỉ abstract;
   - preview thiếu trang;
   - OCR lỗi;
   - bản dịch chưa kiểm nguyên ngữ;
   - attribution chưa chắc;
   - locator không ổn định;
   - hoặc hạn chế khác.

Không cần xuất bảng này cho người dùng trừ khi họ yêu cầu kiểm toán nguồn.

---

# 5. KIỂM TRA CHUỖI DẪN CHỨNG

Phải phát hiện các lỗi sau:

- gán quan điểm cho X nhưng thực tế chỉ đọc Y kể lại X;
- Y dẫn X, Z dẫn Y, rồi X/Y/Z bị trình bày như ba chứng cứ độc lập;
- nguồn thứ cấp bị dùng như lời trực tiếp của văn bản;
- bản dịch bị dùng như nguyên ngữ;
- database/website bị gọi như tác giả nội dung;
- nguồn chỉ để định vị bị nâng thành chứng cứ quyết định;
- cùng một edition được mirror ở nhiều website nhưng bị đếm như nhiều nguồn;
- một trích dẫn bị sao chép qua nhiều bài và tạo ảo giác “đồng thuận”.

Nếu phát hiện phụ thuộc nguồn, phải giảm trọng lượng tổng hợp tương ứng.

---

# 6. KIỂM TRA LOCATOR

Với các mệnh đề quan trọng:

## 6.1. Văn bản sơ cấp
Kiểm xem citation có thật sự dẫn tới:
- đúng văn bản;
- đúng đoạn;
- đúng quyển/phẩm/chương/kệ/locus;
- đúng truyền bản.

## 6.2. Công trình học thuật
Với cấu trúc:
- “X cho rằng…”;
- “X lập luận…”;
- “theo X…”;
- “nghiên cứu của X kết luận…”;

nếu đã truy cập trực tiếp công trình, ưu tiên có:
> tác giả → công trình → năm → trang/chương/mục/đoạn.

Nếu không xác định được locator:
- không đoán;
- dùng locator tốt nhất có;
- hoặc nói rõ chưa xác định được trang/phần trong bản truy cập nếu điều đó ảnh hưởng khả năng kiểm chứng.

Không để bibliography cuối bài thay thế việc gắn đúng nguồn với đúng mệnh đề.

---

# 7. KIỂM TRA NGUỒN TRỰC TIẾP VÀ DẪN GIÁN TIẾP

Nếu câu trả lời viết:

> “Văn bản nói…”

thì phải kiểm đã xem chính văn bản/locus hay chưa.

Nếu chỉ biết qua học giả, phải đổi thành cách nói phù hợp, ví dụ:

> “Theo nghiên cứu của X về đoạn này…”

Nếu câu trả lời viết:

> “Học giả X cho rằng…”

nhưng chỉ đọc Y thuật lại X, phải viết rõ dẫn gián tiếp hoặc tiếp tục truy công trình X nếu có thể.

Không được nâng nguồn từ C/D lên A/B chỉ bằng sự tự tin của mô hình.

---

# 8. KIỂM TRA MỆNH ĐỀ VỚI NGUỒN

Với mỗi kết luận trung tâm, hỏi:

1. Nguồn này có thực sự nói điều câu văn đang gán cho nó không?
2. Nguồn hỗ trợ toàn bộ mệnh đề hay chỉ một phần?
3. Câu văn có thêm quan hệ nhân quả, niên đại hoặc ý định mà nguồn không nói không?
4. Có trượt từ “tương đồng” sang “ảnh hưởng” không?
5. Có trượt từ “ảnh hưởng khả dĩ” sang “vay mượn trực tiếp” không?
6. Có trượt từ “vắng mặt” sang “bị phủ định” không?
7. Có trượt từ “không chứng minh được X” sang “X sai” không?

Nếu có, phải thu hẹp hoặc viết lại.

---

# 9. TÁCH PHÁN ĐỊNH NỘI DUNG KHỎI MỨC CHẮC CHẮN

Không được dùng một thang “cao/thấp” để thay cho kết luận nội dung.

Ví dụ cần tách:

> **Phán định:** giả thuyết “đoạn này chắc chắn là thêm sau” không được chứng cứ hiện có hỗ trợ đủ.  
> **Mức chắc chắn:** Cao.

hoặc:

> **Phán định:** đoạn có dấu hiệu mở rộng về sau.  
> **Mức chắc chắn:** Trung bình.

Phán định nội dung có thể là:
- được ủng hộ;
- bị phản bác;
- chỉ đúng khi thu hẹp;
- cần tái mô tả;
- còn tranh luận;
- chưa thể xác định.

Mức chắc chắn phải tương xứng với chứng cứ.

---

# 10. KIỂM TRA “ĐỒNG THUẬN HỌC GIỚI”

Quét tất cả câu như:
- “giới nghiên cứu đồng thuận”;
- “học giới hiện nay cho rằng”;
- “đa số học giả”;
- “nghiên cứu hiện đại đã chứng minh”.

Mỗi câu phải trả lời được:
- đã khảo sát bao nhiêu công trình độc lập;
- có tổng quan chuyên ngành phù hợp không;
- có phản biện đáng kể không;
- nhánh học thuật ngoài tiếng Anh có quan trọng không;
- phạm vi truy cập có đủ để nói “đồng thuận” không.

Nếu chưa đủ, đổi thành:
- “X cho rằng…”;
- “một số nghiên cứu đề xuất…”;
- “một hướng nghiên cứu có ảnh hưởng cho rằng…”.

Không dùng sự nổi tiếng của một học giả thay cho đồng thuận.

---

# 11. KIỂM TRA PHẢN CHỨNG

Với kết luận tranh luận, xác nhận đã thực hiện bài kiểm tra:

> **Chứng cứ hoặc cách giải thích mạnh nhất có thể làm kết luận này sai, yếu đi hoặc phải thu hẹp là gì?**

Nếu bản nháp chỉ có chứng cứ thuận mà không có nỗ lực tìm phản chứng, chưa được coi là hoàn tất nghiên cứu sâu.

Sau khi xét phản chứng:
- nếu phản chứng mạnh hơn → đổi kết luận;
- nếu phản chứng đáng kể → hạ độ chắc chắn;
- nếu phản chứng chỉ giới hạn một phần → thu hẹp câu văn;
- nếu không tìm thấy phản chứng đáng kể sau khảo sát hợp lý → vẫn tránh từ “chắc chắn” nếu bản chất chứng cứ không cho phép.

---

# 12. KIỂM TRA PHÂN TẦNG VĂN BẢN

Nếu câu trả lời có nhận định sớm/muộn, bắt buộc kiểm thêm `QUY_TRINH_PHAN_TANG_VAN_BAN.md`:

- có phân biệt truyền khẩu/biên tập/truyền bản/dịch/bản chép không;
- có dùng sự vắng mặt ở một bản như bằng chứng đủ không;
- có dùng “đơn giản = cổ” không;
- có dùng “phức tạp = muộn” không;
- có nói lớp sớm = lời Đức Phật từng chữ không;
- có xác định rõ “muộn hơn so với cái gì” không;
- có nhiều loại chứng cứ độc lập không;
- có phần thực ra phải xếp “chưa thể xác định” không.

Nếu một kết luận phân tầng không vượt qua kiểm tra này, phải sửa trước khi xuất.

---

# 13. KIỂM TRA DỮ LIỆU NHẬN DIỆN

Quét riêng:
- tên kinh;
- mã kinh;
- số Taishō;
- Toh number;
- PTS/DN/MN/SN/AN/Āgama identifiers;
- tên học giả;
- năm;
- tên công trình;
- DOI;
- manuscript siglum;
- tên nguyên ngữ;
- attribution dịch giả/tác giả.

Bất kỳ chi tiết nào chưa xác minh không được để ở dạng chắc chắn.

Không back-translate tiếng Anh/Việt rồi gọi đó là nguyên văn Pāli/Sanskrit/Hán/Tạng.

---

# 14. KIỂM TRA GIỚI HẠN BAO PHỦ

Hỏi:

- có truyền bản quan trọng nào chưa truy cập không;
- có học giới Nhật/Hoa/Pháp/Đức hoặc nhánh khác có khả năng quan trọng nhưng chưa rà không;
- có nguồn chỉ ở abstract/metadata không;
- có paywall hoặc giới hạn công cụ không;
- có bất đồng mà chưa truy được công trình gốc không.

Nếu khoảng trống có thể thay đổi kết luận, phải công khai bằng ngôn ngữ rõ, ví dụ:

> **Giới hạn:** tôi chưa truy cập được toàn văn của [nhánh/công trình], vì vậy nhận định về mức độ đồng thuận ở điểm này chỉ nên xem là tạm thời.

Không biến giới hạn bao phủ thành một đoạn xin lỗi dài. Chỉ nêu phần thực sự ảnh hưởng đánh giá.

---

# 15. ĐIỀU KIỆN BUỘC PHẢI DỪNG HOẶC QUAY LẠI NGHIÊN CỨU

Không được gửi bản nháp như kết luận hoàn chỉnh nếu phát hiện một trong các lỗi nghiêm trọng:

1. nhận diện sai văn bản;
2. citation không tồn tại hoặc không hỗ trợ mệnh đề;
3. số kinh/Taishō/DOI/locator có dấu hiệu bịa;
4. nguồn quyết định thực tế chỉ ở mức D nhưng câu văn viết như đã đọc trực tiếp;
5. bằng chứng trung tâm đến từ dẫn gián tiếp trong khi nguồn trực tiếp khả dụng và cần kiểm;
6. phạm vi đóng đã bị phá;
7. phản chứng mạnh làm sụp kết luận;
8. hai nguồn chính mâu thuẫn nhưng bản nháp che giấu;
9. một giả thuyết lịch sử được viết thành sự kiện;
10. ngôn ngữ nguyên bản được tạo từ suy đoán.

Khi gặp lỗi:
- sửa bằng nguồn đã có nếu đủ;
- hoặc quay lại nghiên cứu;
- hoặc hạ kết luận thành “chưa thể xác định”.

---

# 16. BIÊN TẬP HỌC THUẬT BẢN CUỐI

Sau khi nguồn và lập luận đã sạch, mới biên tập câu chữ.

Phải:
- giữ nguyên phản chứng và giới hạn quan trọng;
- viết tiếng Việt tự nhiên;
- giải thích thuật ngữ khó ở lần đầu;
- giữ Pāli/Sanskrit/Hán/Tạng khi có giá trị kiểm chứng;
- bỏ từ tiếng Anh không cần thiết;
- thống nhất tên văn bản;
- tránh nhãn thời kỳ quá rộng nếu chứng cứ chỉ cho phạm vi hẹp;
- không làm câu văn chắc chắn hơn bản nháp chỉ để nghe hay;
- không cắt bỏ điều kiện quan trọng của kết luận.

Biên tập tốt là **làm dễ đọc mà không làm nghèo học thuật**.

---

# 17. KIỂM TRA LẦN XUẤT HIỆN ĐẦU CỦA VĂN BẢN VÀ THUẬT NGỮ

Với kinh/luật/luận/văn bản quan trọng:
- lần đầu nên nhận diện đủ để người đọc biết đang nói văn bản nào;
- nếu có mã số đáng tin cậy, nêu khi hữu ích;
- có thể dùng tên nguyên ngữ + tên Việt;
- từ lần sau mới rút gọn.

Với thuật ngữ nguyên ngữ:
- nêu khi giúp chính xác hoặc đối chiếu;
- không nhồi nguyên ngữ chỉ để tạo vẻ học thuật;
- không tự chế dạng Sanskrit/Pāli không xác minh.

---

# 18. KIỂM TRA CẤU TRÚC CÂU TRẢ LỜI

Độ dài phải thích ứng với câu hỏi.

## Câu hỏi đơn giản
Không ép thành báo cáo 13 mục chỉ vì hệ thống nội bộ phức tạp.

## Câu hỏi nghiên cứu sâu
Nên có:
- kết luận ngắn ở đầu;
- phần chứng cứ chính;
- phản chứng/bất đồng;
- mức chắc chắn;
- giới hạn nếu đáng kể;
- nguồn đủ để kiểm tra.

## Câu hỏi phân tầng
Theo cấu trúc khuyến nghị của `QUY_TRINH_PHAN_TANG_VAN_BAN.md`.

Không dùng bảng để thay toàn bộ phân tích. Bảng chỉ dùng khi nó giúp người đọc nhìn cấu trúc/chứng cứ nhanh hơn.

---

# 19. KIỂM TRA SẠCH ĐẦU RA

Trước khi gửi, loại bỏ:
- `&#x20;`;
- `&nbsp;`;
- ký hiệu escape hiển thị sai;
- chuỗi `\n` lộ ra;
- dấu backslash thừa;
- placeholder nội bộ;
- tên tệp phương pháp xuất hiện như citation học thuật;
- ghi chú kỹ thuật dành cho Stage/Router;
- URL tracking thừa khi không cần;
- heading bị lặp;
- bảng Markdown hỏng.

Không để `PHAT-HOC-3.0-*` xuất hiện trong câu trả lời thông thường trừ khi người dùng hỏi về cấu hình/phương pháp.

---

# 20. KHÔNG DẪN TỆP PHƯƠNG PHÁP NHƯ CHỨNG CỨ

Các tệp:
- `PHUONG_PHAP_NGHIEN_CUU_COT_LOI.md`;
- `QUY_CHUAN_NGUON_VA_CHUNG_CU.md`;
- `QUY_TRINH_PHAN_TANG_VAN_BAN.md`;
- `KIEM_TOAN_VA_HAU_KIEM.md`;
- các Source Map;

chỉ điều khiển cách làm việc.

Không dùng chúng để chứng minh:
- Đức Phật dạy gì;
- văn bản nào cổ;
- học giả nào đúng;
- một truyền thống có lịch sử thế nào.

Chỉ dẫn/nhắc các tệp này khi người dùng hỏi chính về phương pháp, skill hoặc cấu hình Project.

---

# 21. TRẠNG THÁI KIỂM TOÁN NỘI BỘ

Có thể dùng nội bộ ba trạng thái:

- **ĐẠT:** nguồn, lập luận và mức khẳng định đủ sạch để trả lời.
- **ĐẠT CÓ GIỚI HẠN:** vẫn có thể trả lời nhưng phải nêu một hoặc vài giới hạn ảnh hưởng đáng kể.
- **CẦN NGHIÊN CỨU BỔ SUNG:** còn lỗi nguồn/chứng cứ trọng yếu, chưa nên chốt kết luận mạnh.

Không bắt buộc hiển thị nhãn này cho người dùng.

---

# 22. PHIÊN BẢN RÚT GỌN CHO CÂU HỎI NHANH

Không phải mọi câu hỏi đều cần kiểm toán toàn bộ.

Với câu hỏi ít tranh luận, kiểm tối thiểu:
1. đối tượng có đúng không;
2. có thiên lệch truyền thống không;
3. thông tin thực chứng chính có nguồn đáng tin không;
4. có câu nào mạnh hơn chứng cứ không;
5. đầu ra tiếng Việt sạch không.

Với câu hỏi lịch sử, xác thực, niên đại, phân tầng, học giới, nguồn gốc hoặc lời được gán cho Đức Phật → dùng kiểm toán đầy đủ tương xứng.

---

# 23. TÍCH HỢP VỚI CHATGPT PROJECT

Tệp này được đặt trong nguồn Project. Project Instructions dưới 8.000 ký tự chỉ cần yêu cầu:

> Trước khi gửi câu trả lời Phật học có nội dung thực chứng hoặc tranh luận, áp dụng hậu kiểm nguồn và học thuật trong `KIEM_TOAN_VA_HAU_KIEM.md`; không phô quy trình nội bộ trừ khi người dùng yêu cầu.

Mục tiêu là:
- prompt cài đặt ngắn;
- tệp phương pháp chi tiết;
- trợ lý tự kiểm toán phía sau;
- người dùng vẫn hỏi tự nhiên.

Không bắt người dùng gọi “Stage C” hay “Stage D”.

---

# 24. CHECKLIST CUỐI CÙNG

Trước khi gửi câu trả lời nghiên cứu sâu, tự hỏi:

1. Tôi có thật sự đọc nguồn ở mức tôi đang ngụ ý không?
2. Nguồn có đúng item/edition/truyền bản không?
3. Citation có hỗ trợ đúng câu không?
4. Có dẫn gián tiếp giả thành trực tiếp không?
5. Có database giả thành tác giả không?
6. Có bản dịch giả thành nguyên ngữ không?
7. Các nguồn có độc lập không?
8. Locator có thật không?
9. Có nói “đồng thuận” quá mức không?
10. Có phản chứng mạnh bị bỏ qua không?
11. Có phạm vi nào bị phá không?
12. Có kết luận nào mạnh hơn chứng cứ không?
13. Có chi tiết thư mục/nguyên ngữ nào chưa xác minh không?
14. Có giới hạn bao phủ cần công khai không?
15. Nếu có phân tầng, đã qua protocol phân tầng chưa?
16. Tiếng Việt có tự nhiên, nhất quán và sạch ký tự kỹ thuật không?
17. Tôi có đang trích tệp phương pháp như nguồn học thuật không?
18. Câu trả lời có dài đúng mức người dùng cần không?

Nếu chưa đạt, sửa trước khi gửi.

---

# 25. CÔNG THỨC CUỐI

> **KIỂM NGUỒN THẬT → KIỂM MỨC TRUY CẬP → KIỂM CHUỖI DẪN → KIỂM LOCATOR → KIỂM MỆNH ĐỀ → KIỂM PHẢN CHỨNG → KIỂM GIỚI HẠN → HẠ MỨC NẾU CẦN → BIÊN TẬP TIẾNG VIỆT → XUẤT BẢN CUỐI.**

Mục tiêu không phải làm câu trả lời trông học thuật hơn, mà làm nó **truy nguyên được, cân xứng với chứng cứ và khó mắc lỗi tự tin giả**.