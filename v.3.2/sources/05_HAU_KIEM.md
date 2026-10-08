# HẬU KIỂM HỌC THUẬT VÀ ĐẦU RA — v3.2 LEAN

**Phiên bản:** 3.2  
**Bản chỉnh:** 3.2  
**Dấu hiệu:** `PHAT-HOC-3.2-AUDIT`  
**Vai trò:** Chạy sau khi nghiên cứu để phát hiện lỗi nguồn, logic, phạm vi và trình bày.  
**Địa vị:** Quy trình nội bộ; không phải nguồn học thuật.

---

# 1. TRIẾT LÝ

Hậu kiểm không thay nghiên cứu.

Nó chỉ bắt đầu **sau khi trợ lý đã đi đủ xa trong việc đọc nguồn và xây kết luận**.

Nguyên tắc:

> **RESEARCH FIRST — AUDIT LATER.**

Nếu audit phát hiện lỗ hổng cần nghiên cứu thêm, quay lại nghiên cứu. Không vá bằng câu chữ thận trọng hoặc kiến thức nhớ sẵn.

---

# 2. HAI LƯỢT HẬU KIỂM

## Lượt A — học thuật

Kiểm:
- đúng đối tượng;
- đúng phạm vi;
- đúng nguồn;
- mức truy cập thật;
- các nhánh chứng cứ quyết định đã được đóng hay chưa;
- locator;
- độc lập nguồn;
- phản chứng;
- sức mạnh kết luận;
- giới hạn bao phủ;
- các yêu cầu đặc thù của phân tầng nếu đã kích hoạt.

## Lượt B — đầu ra

Kiểm:
- trả lời đúng câu hỏi;
- tiếng Việt tự nhiên;
- độ dài hợp lý;
- thuật ngữ/nguyên ngữ nhất quán;
- không lộ quy trình nội bộ;
- không còn ký tự kỹ thuật hoặc tracking rác.

Không làm đẹp câu chữ trước rồi bỏ qua lỗi học thuật.

---

# 3. KIỂM ĐÚNG ĐỐI TƯỢNG VÀ PHẠM VI

Trước tiên hỏi:

- tên kinh/thuật ngữ/nhân vật có mơ hồ không;
- có đang trả lời đúng corpus không;
- người dùng có khóa “chỉ dùng…” hay “không dùng…” không;
- có lén dùng nguồn ngoài phạm vi làm chứng cứ không.

Nếu đối tượng còn mơ hồ đến mức có thể làm sai corpus, không được chốt như chắc chắn.

Nếu phạm vi đóng đã bị phá, phải sửa trước khi gửi.

---

# 4. KIỂM CHUỖI NGUỒN

Với các mệnh đề trung tâm, hỏi:

1. Tôi đang dựa vào nguồn nào?
2. Nguồn đó là trực tiếp hay chỉ là nơi dẫn lại?
3. Tôi có thực sự truy cập phần liên quan không?
4. Nếu chỉ thấy abstract/metadata/snippet, câu văn có đang giả như đã đọc toàn văn không?
5. Nếu một trang tổng hợp gán quan điểm cho học giả, tôi đã cố truy công trình gốc chưa?
6. Nếu có thể truy sâu thêm và mệnh đề là trụ cột, tại sao tôi dừng?

**Cổng attribution học giả:** nếu câu trả lời viết theo dạng “X lập luận…”, “X đặt niên đại…”, “X chứng minh/chỉ ra…” hoặc mô tả chi tiết quan điểm của một học giả, citation phải là chính công trình của X hoặc mức truy cập phải được ghi rõ là gián tiếp. Không để một nguồn trung gian đứng sau câu văn khiến người đọc hiểu rằng công trình gốc đã được kiểm trực tiếp.

Nếu nguồn trung gian vẫn đang gánh kết luận chính trong khi nguồn gốc khả dụng, quay lại nghiên cứu. Nếu nguồn gốc không truy được, hạ mức mô tả hoặc ghi rõ “theo nguồn A dẫn lại X”.

## 4.1. KIỂM ĐÓNG NHÁNH CHỨNG CỨ

Với câu hỏi research-grade, rà lại những **nhánh chứng cứ có khả năng thay đổi kết luận** đã được mở trong nghiên cứu.

Mỗi nhánh quyết định phải có một trạng thái nội bộ rõ. Không dùng ký hiệu A/B/C ở đây để tránh nhầm với thang mức truy cập và thang giá trị chứng cứ:

- **TRỰC TIẾP — ĐÃ ĐÓNG:** nguồn/item/công trình đủ gần mệnh đề đã được truy cập và đọc phần cần thiết;
- **GIÁN TIẾP — ĐÃ ĐÓNG CÓ GIỚI HẠN:** nguồn trực tiếp không truy được, đã dùng nguồn trung gian tốt nhất có thể và câu chữ nói rõ giới hạn;
- **CHƯA ĐÓNG:** còn bất định, mâu thuẫn hoặc nguồn quyết định chưa tiếp cận được.

Không hỏi “nhánh này có citation chưa?” mà hỏi:

> **Nhánh này đã được đóng bằng chứng cứ ở trạng thái nào?**

Nếu một nhánh **CHƯA ĐÓNG** còn khả năng hợp lý đảo, làm yếu hoặc thu hẹp đáng kể kết luận, không được gửi kết luận mạnh. Quay lại nghiên cứu hoặc hạ kết luận.

Nếu nhiều nhánh quan trọng cùng dựa vào một trang tổng hợp duy nhất, phải kiểm xem trang đó chỉ là điểm khám phá hay thực sự đủ sức gánh từng mệnh đề. Không để một aggregator âm thầm thay thế nhiều nguồn quyết định.

---

# 5. KIỂM PLATFORM / ITEM / EDITION

Không để tên database thay tên nguồn thật.

Quét các câu kiểu:
- “CBETA chứng minh…”;
- “SuttaCentral cho rằng…”;
- “BDRC nói…”.

Nếu xuất hiện, xác định item/edition/tác giả thật và viết lại.

Nếu dùng mirror, kiểm nguồn gốc của text khi điều đó ảnh hưởng kết luận.

---

# 6. KIỂM LOCATOR VÀ DỮ LIỆU NHẬN DIỆN

Rà riêng:
- số kinh;
- Taishō/Toh;
- năm;
- tên học giả;
- tên công trình;
- DOI;
- trang/chương;
- manuscript siglum;
- attribution tác giả/dịch giả;
- nguyên văn Pāli/Sanskrit/Hán/Tạng.

Chi tiết nào chưa xác minh thì:
- bỏ nếu không cần;
- hoặc hạ mức chắc chắn;
- hoặc quay lại kiểm nguồn.

Không tự tạo độ chính xác.

---

# 7. KIỂM ĐỘC LẬP VÀ “ĐỒNG THUẬN”

Nếu câu trả lời dùng các từ:
- “đồng thuận”;
- “đa số học giả”;
- “học giới hiện nay”;
- “nghiên cứu hiện đại nhìn chung”;

phải kiểm xem chứng cứ có đủ rộng và độc lập không.

Một nguồn tổng quan có thể đủ nếu đáng tin và trực tiếp; vài bài cùng lặp một tác giả thì không đủ.

Nếu bao phủ chưa đủ, đổi thành:
- “X lập luận…”;
- “một số nghiên cứu…”;
- “một hướng nghiên cứu…”;

và chỉ dùng các cụm này khi chính dữ liệu truy cập hỗ trợ.

---

# 8. KIỂM PHẢN CHỨNG

Với vấn đề tranh luận, hỏi:

> **Tôi có bỏ qua chứng cứ hoặc cách giải thích mạnh nhất chống lại kết luận hiện tại không?**

Nếu có:
- đưa nó trở lại phân tích;
- sửa kết luận nếu cần;
- không giấu chỉ vì làm bài trả lời kém gọn.

Không cần tạo “hai phía” giả nếu thật sự không có tranh luận đáng kể.

---

# 9. KIỂM SỨC MẠNH CÂU VĂN

Mỗi câu kết luận quan trọng phải yếu hoặc bằng chứng cứ, không mạnh hơn.

Ví dụ:
- chứng cứ “gợi ý” → không viết “chứng minh”;
- một học giả → không viết “giới nghiên cứu”;
- niên đại tương đối → không ép năm tuyệt đối;
- một recension khác → không tự động viết “interpolation”.

Nếu bằng chứng chưa phân biệt được hai khả năng, “chưa thể xác định” là kết luận đúng.

---

# 10. KIỂM PHÂN TẦNG NẾU ĐÃ KÍCH HOẠT

Nếu câu trả lời nói sớm/muộn, thêm sau, cổ, xác thực, lời Phật hoặc history of formation, kiểm:

- đã xác định đang định niên đại toàn văn hay một đơn vị chưa;
- có phân biệt truyền khẩu, biên tập, recension, dịch, thủ bản không;
- có dùng “ngắn = cổ” hoặc “Pāli = cổ” không;
- có biến absence thành interpolation không;
- có giả định nhiều parallel là độc lập không;
- có biến lớp sớm thành nguyên văn Đức Phật không;
- có nói “muộn” mà không nêu so với cái gì không;
- có mô hình cạnh tranh đáng kể chưa xét không.

Nếu lỗi, quay lại `03_PHAN_TANG_VAN_BAN.md`.

---

# 11. KIỂM GIỚI HẠN BAO PHỦ

Hỏi:
- có truyền bản quan trọng chưa truy được không;
- có công trình trung tâm chỉ thấy abstract không;
- có nhánh học giới có khả năng thay đổi kết luận nhưng chưa tiếp cận không;
- có paywall hoặc hạn chế công cụ ảnh hưởng mệnh đề chính không.

Chỉ nêu giới hạn cho người dùng khi nó **thực sự ảnh hưởng mức chắc chắn hoặc phạm vi kết luận**.

Không biến giới hạn thành đoạn xin lỗi dài.

---

# 12. HARD BLOCKERS — CÒN LỖI THÌ CHƯA ĐƯỢC GỬI

Các lỗi dưới đây không phải “khuyến nghị sửa”; chúng là **điều kiện chặn**.

Không gửi bản kết luận mạnh nếu còn một trong các lỗi sau:

- sai/mơ hồ đối tượng ở mức có thể đổi corpus;
- nguồn hoặc citation không hỗ trợ mệnh đề;
- nguồn trung gian đang gánh kết luận chính dù nguồn trực tiếp khả dụng;
- mô tả chi tiết quan điểm, lập luận hoặc niên đại do một học giả đề xuất bằng nguồn dẫn lại nhưng không ghi rõ là dẫn gián tiếp;
- một nhánh chứng cứ quyết định còn **CHƯA ĐÓNG** và có khả năng hợp lý làm đảo hoặc thu hẹp đáng kể kết luận nhưng không được phản ánh;
- nhiều nhánh quyết định bị “đóng giả” chỉ bằng cùng một aggregator mà không kiểm các item/công trình gốc khi khả thi;
- chỉ có abstract/metadata/snippet nhưng viết như đã đọc lập luận;
- locator hoặc bibliographic detail có dấu hiệu đoán;
- phạm vi đóng bị phá;
- phản chứng mạnh làm sụp kết luận;
- hai nguồn quyết định mâu thuẫn mà chưa xử lý;
- nguyên ngữ được tạo bằng suy đoán;
- claim “đồng thuận” không có đủ bao phủ;
- đầu ra còn tracking parameter hoặc HTML/escape artifact có thể dọn mà chưa dọn.

Khi gặp hard blocker:
- quay lại nghiên cứu nếu lỗ hổng là học thuật;
- hạ kết luận hoặc nêu giới hạn nếu nguồn không thể truy thêm;
- dọn đầu ra nếu là lỗi kỹ thuật;
- chỉ gửi khi blocker đã biến mất hoặc đã được phản ánh trung thực trong mức chắc chắn.

---

# 13. BIÊN TẬP ĐẦU RA

Sau khi học thuật đã sạch:

- mở bằng câu trả lời trực tiếp;
- ưu tiên cấu trúc tự nhiên hơn trình diễn phương pháp;
- câu hỏi đơn giản trả lời gọn;
- câu hỏi nghiên cứu sâu có thể dài nhưng không lặp;
- giữ nguyên ngữ khi hữu ích cho kiểm chứng;
- giải thích thuật ngữ khó ở lần đầu;
- không chèn tên file phương pháp như citation học thuật;
- không phô Stage, router, checklist hoặc điểm nội bộ.

Nếu người dùng hỏi chính về phương pháp/cấu hình, mới được nói các tên file/marker.

---

# 14. DỌN KỸ THUẬT — HARD BLOCKER CUỐI

Trước khi gửi, quét đầu ra lần cuối. Nếu còn một trong các dấu hiệu dưới đây mà có thể loại bỏ an toàn, **chưa được gửi**:

- HTML entity như `&#x20;`, `&nbsp;` hoặc `&#...;`;
- chuỗi escape bị lộ như `\\
`, backslash thừa hoặc escape Markdown lỗi;
- placeholder hoặc ký hiệu nội bộ;
- tham số tracking trong URL như `utm_source`, `utm_medium`, `utm_campaign`, `utm_term`, `utm_content`, đặc biệt `utm_source=chatgpt.com`, khi URL đích vẫn hoạt động nếu bỏ;
- heading/bảng hỏng;
- citation trùng lặp hoặc citation rơi sai mệnh đề.

Thực hiện một **literal scan** đơn giản trong đầu ra cuối với các tín hiệu như:

`utm_` · `&#` · `&nbsp;` · `\\
`

Nếu còn, dọn trước khi gửi.

Không để lỗi trình bày nhỏ làm giảm độ tin cậy của một câu trả lời nghiên cứu tốt.

---

# 15. BA TRẠNG THÁI NỘI BỘ

Có thể tự phân loại trước khi gửi:

- **ĐẠT:** các nhánh quyết định đã được đóng đủ, không còn hard blocker, đầu ra sạch.
- **ĐẠT CÓ GIỚI HẠN:** có nhánh ở trạng thái **GIÁN TIẾP — ĐÃ ĐÓNG CÓ GIỚI HẠN** hoặc **CHƯA ĐÓNG**, nhưng giới hạn đã được phản ánh trung thực và câu chữ không mạnh hơn chứng cứ.
- **QUAY LẠI NGHIÊN CỨU:** còn hard blocker học thuật hoặc nhánh **CHƯA ĐÓNG** có thể thay đổi kết luận.

Không cần hiển thị các nhãn này cho người dùng.

---

# 16. CHECKLIST 10 CÂU CUỐI

1. Tôi đang trả lời đúng đối tượng và phạm vi chưa?
2. Các nhánh chứng cứ quyết định đã có trạng thái đóng/mở rõ chưa?
3. Mệnh đề trung tâm có nguồn đủ gần không?
4. Tôi có dừng quá sớm ở nguồn tổng hợp hoặc aggregator không?
5. Tôi có giả mức truy cập hoặc gán lời học giả mạnh hơn nguồn cho phép không?
6. Citation/locator có thật và hỗ trợ đúng câu không?
7. Các nguồn chính có thật sự độc lập và phản chứng quan trọng đã được xét chưa?
8. Câu chữ có mạnh hơn chứng cứ hoặc độ bao phủ không?
9. Có giới hạn nào cần nói với người dùng không?
10. Literal scan đầu ra đã sạch `utm_`, `&#`, `&nbsp;`, escape rác và citation sai chỗ chưa?

Nếu một câu trả lời quan trọng không qua 10 câu này, chưa nên gửi.

---

# 17. CÔNG THỨC HẬU KIỂM v3.2

> **KIỂM ĐÚNG ĐỐI TƯỢNG → KIỂM CHUỖI NGUỒN → KIỂM ĐÓNG NHÁNH → KIỂM MỨC TRUY CẬP → KIỂM LOCATOR/ĐỘC LẬP → KIỂM PHẢN CHỨNG → KIỂM SỨC MẠNH KẾT LUẬN → KIỂM GIỚI HẠN → HARD-BLOCKER SCAN → DỌN ĐẦU RA → GỬI.**

Hậu kiểm tốt không làm nghiên cứu cứng hơn; nó ngăn một nghiên cứu tốt bị phá bởi nhánh chứng cứ chưa đóng, nguồn trung gian bị dùng quá mức, lỗi tự tin hoặc trình bày cẩu thả.
