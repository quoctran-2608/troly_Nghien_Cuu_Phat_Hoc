# HƯỚNG DẪN CÀI ĐẶT CLAUDE PROJECT — PHAT-HOC v3.2.2

**Gói:** `v.3.2.2/Setup-for-claude/`  
**Mục tiêu:** cài PHAT-HOC v3.2.2 trên Claude Projects bằng một bộ độc lập, giữ nguyên lõi nghiên cứu và chỉ thêm điều phối nhỏ đã rút ra từ benchmark thực tế.

> **Nguyên tắc:** giữ nguyên lõi `01`–`05`; chỉ điều chỉnh lớp Project Instructions cho hành vi đặc thù của Claude.

---

# 1. TẠO CLAUDE PROJECT

Tên gợi ý:

`Trợ lý - NGHIÊN CỨU PHẬT HỌC v3.2.2`

Mô tả mục tiêu có thể dùng:

> Xây dựng trợ lý nghiên cứu Phật học học thuật bằng tiếng Việt, chuyên nghiên cứu sâu từ chính văn và công trình học thuật; đối chiếu đa truyền thống, đa ngôn ngữ; phân tầng văn bản; kiểm tra phản chứng, mức độ chắc chắn và chất lượng nguồn; không bịa trích dẫn, nguồn hay đồng thuận học giới.

Tên và mô tả chỉ dùng để quản lý Project; không thay Project Instructions.

---

# 2. TẢI PROJECT KNOWLEDGE

Từ thư mục:

`Setup-for-claude/sources/`

tải đúng 5 tệp:

1. `01_NGHIEN_CUU_COT_LOI.md`
2. `02_NGUON_VA_CHUNG_CU.md`
3. `03_PHAN_TANG_VAN_BAN.md`
4. `04_BAN_DO_NGUON_PHAT_HOC.md`
5. `05_HAU_KIEM.md`

Đây là bộ phương pháp, không phải chứng cứ học thuật cho các mệnh đề Phật học.

Không tải các phiên bản cũ, bài benchmark hay câu trả lời mẫu vào Project Knowledge.

---

# 3. DÁN PROJECT INSTRUCTIONS

Mở:

`HUONG_DAN_DU_AN_CLAUDE_PHAT_HOC_v3.2.2.txt`

Sao chép toàn bộ nội dung vào **Project Instructions**.

Marker mong đợi:

`PHAT-HOC-PROJECT-3.2.2-CLAUDE-VI`

Tệp này đã ghép sẵn lõi v3.2.2 với ba điều chỉnh riêng cho Claude:

- truy đến chính văn cho mệnh đề trụ cột khi nguồn trực tiếp còn truy được hợp lý;
- trước kết luận cuối, âm thầm hiệu chỉnh sức mạnh câu chữ theo đúng phạm vi nguồn đã kiểm;
- không phô hậu kiểm/checklist ra thành phần trình diễn trong bài cuối.

Không cần ghép thêm `HUONG_DAN_DU_AN_CHATGPT...` vào Claude Project.

---

# 4. RESEARCH / WEB SEARCH

Với câu hỏi lịch sử, văn bản học, học giới, niên đại, tác quyền hoặc câu hỏi cần nguồn ngoài Project:

- bật **Research** nếu tài khoản có;
- bảo đảm **Web search** khả dụng;
- không coi kết quả search, snippet, abstract hay metadata là đã đọc toàn văn;
- ưu tiên các hạ tầng chuyên ngành theo `04_BAN_DO_NGUON_PHAT_HOC.md`, nhưng không biến Source Map thành whitelist.

Người dùng vẫn chỉ cần hỏi tự nhiên; không cần lặp “hãy research sâu” trong từng prompt nếu Project hoạt động đúng.

---

# 5. MEMORY

Cấu hình khuyến nghị:

```text
Project memory:      ON / hoạt động bình thường
Use account memory:  OFF
```

Lý do: giữ tính liên tục riêng của Project nhưng tránh trộn các chat ngoài Project vào trợ lý nghiên cứu.

`No memory yet` ở Project mới là bình thường.

Memory không thay thế Project Knowledge hay Project Instructions.

Khi benchmark A/B nghiêm, mở chat mới cho mỗi prompt. Nếu giao diện cho phép tắt Memory riêng cho một chat và cần phép thử hoàn toàn cô lập, có thể tắt cho chat benchmark đó.

---

# 6. MODEL VÀ BENCHMARK

Khi so với ChatGPT:

- dùng model Claude mạnh nhất mà tài khoản cho phép;
- giữ nguyên model và mức suy luận trong cả loạt test;
- dùng cùng prompt;
- mở chat mới cho mỗi test độc lập;
- không sửa prompt sau một lỗi đơn lẻ.

Các prompt benchmark đại diện:

> `anattā?`

> `Phạm Võng kinh có cổ không?`

> `Sarvāstivāda hiểu “các pháp tồn tại trong ba thời” như thế nào? Có thật họ nói quá khứ và tương lai tồn tại y hệt hiện tại không?`

> `Khi so sánh anattā với ātman trong Bṛhadāraṇyaka và Chāndogya Upaniṣad, có thể nói Đức Phật đơn giản phủ nhận đúng cùng một khái niệm ātman của Upaniṣad không?`

> `Guhyasamāja Tantra cổ đến mức nào? Có thể gọi nó là lời Đức Phật lịch sử không?`

---

# 7. HAI ĐIỂM CẦN THEO DÕI RIÊNG Ở CLAUDE

Qua benchmark ban đầu, Claude cho thấy ưu thế rất mạnh ở độ rộng, phân tầng, phản chứng và minh bạch mức truy cập. Hai điểm cần kiểm lặp lại là:

## 7.1. Đóng nguồn trực tiếp

Claude có thể đào rất rộng nhưng đôi khi dừng ở một học giả hiện đại dẫn chính văn. Với mệnh đề trụ cột về tác giả/trường phái/truyền thống tự nói gì, nếu chính văn còn truy được hợp lý thì phải đi thêm một bước tới chính văn.

## 7.2. Hiệu chỉnh kết luận

Claude đôi khi nghiên cứu rất thận trọng nhưng câu kết luận mạnh hơn một nấc so với độ bao phủ thực tế. Trước khi gửi, phải hạ các cụm như “loại trừ”, “không thể”, “đa số”, “đồng thuận”, “tốt hơn mọi cách giải thích khác” nếu nguồn chưa đủ sức gánh chúng.

Không vì hai điểm này mà ép Claude trả lời ngắn hơn hoặc giảm breadth.

---

# 8. CẤU TRÚC ĐẦU RA MONG ĐỢI

Với câu hỏi nghiên cứu thực chất, bài cuối cần phản ánh đủ:

- kết luận chính;
- chứng cứ trực tiếp;
- parallel/corpus hoặc truyền bản liên quan;
- nghiên cứu hiện đại quan trọng;
- phản chứng/cách giải thích cạnh tranh;
- mức chắc chắn và giới hạn.

Thứ tự cuối bài:

`KẾT LUẬN → TÀI LIỆU THAM KHẢO`

Nếu cần ghi mức truy cập nguồn, đặt thành chú thích riêng sau danh mục, không nhồi vào từng entry thư mục.

---

# 9. KHÔNG NÊN LÀM

Không:

- chép 5 file phương pháp vào Project Instructions;
- tải nhiều phiên bản lõi vào cùng Project;
- thêm quota số lượng nguồn;
- ép Claude dùng mọi ngôn ngữ/học giới chỉ để “cho đủ”;
- coi một aggregator là nhiều nhánh chứng cứ;
- dùng bibliography làm mục tiêu dẫn dắt nghiên cứu;
- bật `Use account memory` chỉ để mong Claude nhớ nhiều hơn;
- sửa lõi `01`–`05` chỉ vì một khác biệt giao diện hoặc một lỗi đơn lẻ.

---

# 10. TÓM TẮT CẤU HÌNH

```text
CLAUDE PROJECT
│
├── Project Instructions
│   └── HUONG_DAN_DU_AN_CLAUDE_PHAT_HOC_v3.2.2.txt
│
├── Project Knowledge
│   ├── 01_NGHIEN_CUU_COT_LOI.md
│   ├── 02_NGUON_VA_CHUNG_CU.md
│   ├── 03_PHAN_TANG_VAN_BAN.md
│   ├── 04_BAN_DO_NGUON_PHAT_HOC.md
│   └── 05_HAU_KIEM.md
│
├── Memory
│   ├── Project memory: ON
│   └── Use account memory: OFF
│
└── Khi nghiên cứu
    ├── Research / Web search khi cần
    ├── model mạnh và ổn định
    └── chat mới cho benchmark độc lập
```

Triết lý giữ nguyên:

> **NGHIÊN CỨU TRƯỚC — TRUY NGUỒN TRỰC TIẾP — PHẢN CHỨNG — HIỆU CHỈNH KẾT LUẬN — HẬU KIỂM — TÀI LIỆU THAM KHẢO CUỐI CÙNG.**
