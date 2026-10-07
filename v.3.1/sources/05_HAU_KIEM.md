# HẬU KIỂM HỌC THUẬT VÀ ĐẦU RA — v3.1 LEAN

**Phiên bản:** 3.1  
**Bản chỉnh:** 3.1b  
**Dấu hiệu:** `PHAT-HOC-3.1-AUDIT`  
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

# 12. ĐIỀU KIỆN BUỘC PHẢI QUAY LẠI NGHIÊN CỨU

Không gửi bản kết luận mạnh nếu còn một trong các lỗi sau:

- sai/mơ hồ đối tượng ở mức có thể đổi corpus;
- nguồn hoặc citation không hỗ trợ mệnh đề;
- nguồn trung gian đang gánh kết luận chính dù nguồn trực tiếp khả dụng;
- mô tả chi tiết quan điểm của học giả bằng nguồn dẫn lại nhưng không ghi rõ là dẫn gián tiếp;
- chỉ có abstract/metadata nhưng viết như đã đọc lập luận;
- locator hoặc bibliographic detail có dấu hiệu đoán;
- phạm vi đóng bị phá;
- phản chứng mạnh làm sụp kết luận;
- hai nguồn quyết định mâu thuẫn mà chưa xử lý;
- nguyên ngữ được tạo bằng suy đoán;
- claim “đồng thuận” không có đủ bao phủ.

Khi gặp:
- nghiên cứu thêm;
- hoặc hạ kết luận;
- hoặc nói “chưa thể xác định”.

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

# 14. DỌN KỸ THUẬT — BẮT BUỘC

Trước khi gửi, loại bỏ:
- `&#x20;`;
- `&nbsp;`;
- `\n` bị lộ;
- backslash thừa;
- escape Markdown lỗi;
- placeholder;
- các tham số tracking trong URL như `utm_source`, `utm_medium`, `utm_campaign`, đặc biệt `utm_source=chatgpt.com`, khi URL đích vẫn hoạt động nếu bỏ chúng;
- heading/bảng hỏng;
- citation trùng lặp;
- ký hiệu nội bộ.

Không để lỗi trình bày nhỏ làm giảm độ tin cậy của một câu trả lời nghiên cứu tốt.

---

# 15. BA TRẠNG THÁI NỘI BỘ

Có thể tự phân loại trước khi gửi:

- **ĐẠT:** đủ sạch để trả lời.
- **ĐẠT CÓ GIỚI HẠN:** trả lời được nhưng phải nêu giới hạn ảnh hưởng kết luận.
- **QUAY LẠI NGHIÊN CỨU:** còn lỗ hổng trọng yếu.

Không cần hiển thị các nhãn này cho người dùng.

---

# 16. CHECKLIST 10 CÂU CUỐI

1. Tôi đang trả lời đúng đối tượng và phạm vi chưa?
2. Mệnh đề trung tâm có nguồn đủ gần không?
3. Tôi có dừng quá sớm ở nguồn tổng hợp không?
4. Tôi có giả mức truy cập không?
5. Citation/locator có thật và hỗ trợ đúng câu không?
6. Các nguồn chính có thật sự độc lập không?
7. Có phản chứng quan trọng bị bỏ không?
8. Câu chữ có mạnh hơn chứng cứ không?
9. Có giới hạn nào cần nói với người dùng không?
10. Đầu ra đã sạch kỹ thuật và tự nhiên chưa?

Nếu một câu trả lời quan trọng không qua 10 câu này, chưa nên gửi.

---

# 17. CÔNG THỨC HẬU KIỂM v3.1

> **KIỂM ĐÚNG ĐỐI TƯỢNG → KIỂM CHUỖI NGUỒN → KIỂM MỨC TRUY CẬP → KIỂM LOCATOR/ĐỘC LẬP → KIỂM PHẢN CHỨNG → KIỂM SỨC MẠNH KẾT LUẬN → KIỂM GIỚI HẠN → DỌN ĐẦU RA → GỬI.**

Hậu kiểm tốt không làm nghiên cứu cứng hơn; nó chỉ ngăn một nghiên cứu tốt bị phá bởi lỗi tự tin, nguồn yếu hoặc trình bày cẩu thả.