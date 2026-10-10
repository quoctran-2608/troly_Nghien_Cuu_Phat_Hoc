# HƯỚNG DẪN CÀI ĐẶT CLAUDE PROJECT — PHAT-HOC v3.2.2

**Phiên bản gói:** 3.2.2  
**Mục tiêu:** cài cùng lõi nghiên cứu của PHAT-HOC v3.2.2 trên Claude Projects, giữ kiến trúc và chuẩn chứng cứ gần nhất có thể với bản ChatGPT Project để dễ so sánh và kiểm thử.

> **Nguyên tắc:** không viết lại skill chỉ vì đổi nền tảng. Trước hết giữ nguyên lõi `01`–`05` và Project Instructions; chỉ điều chỉnh riêng cho Claude khi có lỗi lặp lại qua nhiều phép thử.

---

# 1. TẠO PROJECT

Có thể đặt tên:

`Trợ lý - NGHIÊN CỨU PHẬT HỌC v3.2.2`

Ở ô mô tả mục tiêu có thể ghi:

> Xây dựng trợ lý nghiên cứu Phật học học thuật bằng tiếng Việt, chuyên nghiên cứu sâu từ chính văn và công trình học thuật; đối chiếu đa truyền thống, đa ngôn ngữ; phân tầng văn bản; kiểm tra phản chứng, mức độ chắc chắn và chất lượng nguồn; không bịa trích dẫn, nguồn hay đồng thuận học giới.

**Lưu ý:** tên và mô tả Project chủ yếu dùng để quản lý Project; không nên coi chúng là Project Instructions. Phần điều khiển hành vi của Claude phải được đặt trong **Project instructions** và **Project knowledge**.

---

# 2. TẢI 5 TỆP PHƯƠNG PHÁP VÀO PROJECT KNOWLEDGE

Từ thư mục `v.3.2.2/sources/`, tải đúng 5 tệp:

1. `01_NGHIEN_CUU_COT_LOI.md`
2. `02_NGUON_VA_CHUNG_CU.md`
3. `03_PHAN_TANG_VAN_BAN.md`
4. `04_BAN_DO_NGUON_PHAT_HOC.md`
5. `05_HAU_KIEM.md`

Các tệp này là **phương pháp nghiên cứu và hậu kiểm**, không phải nguồn chứng cứ để chứng minh các mệnh đề Phật học.

Không tải vào Project Knowledge:

- các phiên bản cũ `v.1`, `v.2`, `v.3.0`, `v.3.1`, `v.3.2.0`;
- các bài benchmark hoặc câu trả lời mẫu;
- `HUONG_DAN_CAI_DAT.md` hoặc chính tệp hướng dẫn Claude này;
- các tài liệu không cần thiết chỉ để “cho nhiều nguồn”.

Mục tiêu là tránh làm Project Knowledge nhiễu và tránh neo Claude vào các câu trả lời mẫu.

---

# 3. CÀI PROJECT INSTRUCTIONS

Mở tệp:

`HUONG_DAN_DU_AN_CHATGPT_PHAT_HOC_v3.2.2.txt`

Sao chép toàn bộ nội dung vào **Set project instructions / Project instructions** của Claude.

Marker mong đợi:

`PHAT-HOC-PROJECT-3.2.2-VI`

## Đoạn cầu nối khuyến nghị cho Claude

Đặt đoạn ngắn sau **ở đầu Project Instructions**, trước nội dung v3.2.2:

> Đây là Project nghiên cứu Phật học học thuật. Năm tệp `01`–`05` trong Project Knowledge là bộ phương pháp bắt buộc phải vận dụng theo đúng chức năng của từng tệp; chúng không phải nguồn chứng cứ cho các mệnh đề Phật học. Với câu hỏi nghiên cứu thực chất, chủ động dùng Research và tìm kiếm web khi có sẵn; không giới hạn việc tìm kiếm ở Bản đồ nguồn. Bản đồ nguồn là mức sàn định tuyến, không phải danh sách trắng. Không để yêu cầu trình bày, trích dẫn hoặc hậu kiểm làm nghèo quá trình nghiên cứu.

Sau đoạn này, giữ nguyên toàn bộ nội dung của `HUONG_DAN_DU_AN_CHATGPT_PHAT_HOC_v3.2.2.txt`.

Nếu muốn thực hiện phép so sánh A/B thật nghiêm giữa ChatGPT và Claude, có thể chạy một vòng đầu **không có đoạn cầu nối**, chỉ dán nguyên Instructions v3.2.2; sau đó mới thử thêm đoạn cầu nối nếu Claude có biểu hiện bỏ qua vai trò của các tệp `01`–`05`.

---

# 4. BẬT KHẢ NĂNG NGHIÊN CỨU WEB

Với câu hỏi nghiên cứu Phật học có nội dung lịch sử, văn bản học, học giới hoặc cần kiểm nguồn ngoài Project:

- bật **Research** nếu tài khoản có tính năng này;
- bảo đảm **Web search** đang khả dụng;
- nếu giao diện Claude mới tự quyết định khi nào cần tìm web thì vẫn có thể ghi rõ trong câu hỏi: `Hãy research trên web và truy nguồn trực tiếp` khi muốn ép một phép thử nghiên cứu sâu.

Research phù hợp với kiến trúc v3.2.2 vì nó có thể thực hiện nhiều lượt tìm kiếm nối tiếp. Tuy nhiên, vẫn phải tuân thủ các quy tắc nguồn, mức truy cập, truy nguồn trực tiếp và phản chứng trong `02`, `04` và `05`.

Không coi việc Claude đã “search” là bằng chứng rằng nó đã đọc toàn văn nguồn.

---

# 5. MODEL VÀ CHẾ ĐỘ SUY LUẬN

Khi benchmark:

- dùng model mạnh nhất mà tài khoản cho phép;
- giữ nguyên cùng model cho toàn bộ một loạt test;
- nếu có chế độ suy luận sâu / extended thinking, giữ cùng một mức giữa các bài so sánh;
- không đổi model giữa hai phiên bản rồi quy chênh lệch cho skill.

Mục tiêu là tách ba biến:

`MODEL` → `PROJECT/INSTRUCTIONS` → `CHẤT LƯỢNG ĐẦU RA`.

---

# 6. CÁCH DÙNG HẰNG NGÀY

Người dùng chỉ cần hỏi tự nhiên, kể cả prompt rất ngắn, ví dụ:

> `anattā?`

> `Phạm Võng kinh có cổ không?`

> `Duy thức có thật sự nói chỉ có tâm tồn tại không?`

Không cần lặp lại trong từng prompt các câu như “hãy nghiên cứu sâu”, “hãy kiểm nguồn”, “hãy đưa phản chứng” nếu Project đã được cài đúng. Những hành vi đó phải đến từ Project Instructions và các tệp `01`–`05`.

Nếu một câu hỏi có giới hạn phạm vi rõ ràng do người dùng đặt, giới hạn đó là ràng buộc cứng.

---

# 7. CHAT MỚI VÀ PROJECT KNOWLEDGE

Khi benchmark, nên mở **chat mới trong cùng Project** cho mỗi prompt độc lập.

Lý do:

- Project Knowledge và Project Instructions vẫn được dùng;
- nội dung hội thoại cũ không nên trở thành dữ kiện mặc định cho bài test mới;
- giảm hiệu ứng neo từ câu trả lời trước;
- dễ so sánh Claude với ChatGPT trên cùng một prompt sạch.

Thông tin muốn Claude luôn dùng giữa nhiều chat phải nằm trong **Project Knowledge** hoặc **Project Instructions**, không nên chỉ để trong một chat cũ.

---

# 8. BỘ TEST KHỞI ĐỘNG KHUYẾN NGHỊ

Không cần chạy hết ngay. Có thể bắt đầu bằng các prompt đại diện:

### Prompt cực ngắn

> `anattā?`

Kiểm: prompt ngắn có tự kích hoạt nghiên cứu sâu hay không.

### Mơ hồ tên kinh

> `Phạm Võng kinh có cổ không?`

Kiểm: có tự phân biệt DN 1 và T1484 hay không.

### Nguồn trực tiếp của học phái

> `Sarvāstivāda hiểu “các pháp tồn tại trong ba thời” như thế nào? Có thật họ nói quá khứ và tương lai tồn tại y hệt hiện tại không?`

Kiểm: có truy chính văn Hữu bộ trước khi để học giả hiện đại nói thay hay không.

### Tranh luận triết học

> `Duy thức có thật sự nói “chỉ có tâm tồn tại, thế giới bên ngoài không tồn tại” không?`

Kiểm: có tránh giản lược toàn bộ Yogācāra thành một mệnh đề duy tâm đơn giản hay không.

### Liên ngành

> `Khi so sánh anattā với ātman trong Bṛhadāraṇyaka và Chāndogya Upaniṣad, có thể nói Đức Phật đơn giản phủ nhận đúng cùng một khái niệm ātman của Upaniṣad không?`

Kiểm: Claude có mở nhánh nghiên cứu Upaniṣad/Ấn Độ học thay vì chỉ dùng Buddhist Studies nói thay phía đối chiếu hay không.

### Phân tầng và tác quyền lịch sử

> `Guhyasamāja Tantra cổ đến mức nào? Có thể gọi nó là lời Đức Phật lịch sử không?`

Kiểm: có phân biệt mốc chứng thực, mốc sáng tác, các lớp văn bản và thẩm quyền tôn giáo với tác quyền lịch sử hay không.

---

# 9. TIÊU CHÍ ĐÁNH GIÁ ĐẦU RA

Không chấm chỉ theo văn phong. Với mỗi bài, kiểm ít nhất:

1. có hiểu đúng và tự giải mơ hồ không;
2. có nghiên cứu theo hai lượt rộng → sâu không;
3. có truy nguồn trực tiếp cho mệnh đề trụ cột không;
4. có phân biệt nguồn trực tiếp, nghiên cứu, khám phá và hạ tầng không;
5. có mở đúng ngành chuyên môn liên quan không;
6. có kiểm phản chứng và cách giải thích cạnh tranh không;
7. có phân tầng văn bản khi câu hỏi liên quan niên đại/tác quyền không;
8. có kiểm độ độc lập của các nhánh chứng cứ không;
9. có hạ mức kết luận khi nguồn quyết định chưa truy cập đủ không;
10. có phân biệt mốc chứng thực với mốc sáng tác không;
11. có dùng tên Việt + nguyên ngữ + mã định vị ở lần nhắc đầu khi xác định được không;
12. có giữ thứ tự kết luận → tài liệu tham khảo và chỉ liệt kê nguồn thực sự dùng không.

Không sửa skill chỉ vì một lần chạy kém. Chỉ chỉnh khi thấy một mô hình lỗi lặp lại qua nhiều phép thử.

---

# 10. NHỮNG ĐIỀU KHÔNG NÊN LÀM

Không:

- sao chép cả 5 tệp `01`–`05` vào Project Instructions;
- tải nhiều phiên bản của cùng một bộ quy tắc vào một Project;
- tải câu trả lời benchmark mẫu vào Project Knowledge trước khi test;
- biến Bản đồ nguồn thành whitelist;
- yêu cầu số lượng nguồn tối thiểu;
- bắt Claude làm bibliography trước khi nghiên cứu xong;
- sửa lõi sau từng lỗi đơn lẻ;
- coi snippet, metadata hoặc abstract là đã đọc toàn văn;
- coi một trang tổng hợp là nhiều nhánh chứng cứ độc lập.

---

# 11. KHI CLAUDE TRẢ LỜI MỎNG HƠN CHATGPT

Trước khi sửa file lõi, kiểm theo thứ tự:

1. Project Instructions đã được lưu đầy đủ chưa;
2. đủ 5 tệp `01`–`05` đã nằm trong Project Knowledge chưa;
3. Research/Web search có hoạt động không;
4. model và mức suy luận có đủ mạnh không;
5. prompt đang chạy trong đúng Project không;
6. lỗi có lặp lại ở nhiều prompt không.

Chỉ sau khi các điều trên đều ổn mà lỗi vẫn lặp lại mới tạo một chỉnh sửa riêng cho Claude.

Không sửa các file `01`–`05` chỉ để chữa một khác biệt giao diện hoặc một lỗi đơn lẻ của model.

---

# 12. TÓM TẮT CẤU HÌNH

Cấu hình khuyến nghị:

```text
CLAUDE PROJECT
│
├── Project Instructions
│   ├── đoạn cầu nối Claude ngắn
│   └── HUONG_DAN_DU_AN_CHATGPT_PHAT_HOC_v3.2.2.txt
│
├── Project Knowledge
│   ├── 01_NGHIEN_CUU_COT_LOI.md
│   ├── 02_NGUON_VA_CHUNG_CU.md
│   ├── 03_PHAN_TANG_VAN_BAN.md
│   ├── 04_BAN_DO_NGUON_PHAT_HOC.md
│   └── 05_HAU_KIEM.md
│
└── Khi nghiên cứu
    ├── Research / Web search khi cần
    ├── model mạnh và ổn định
    └── chat mới cho benchmark độc lập
```

Triết lý vẫn giữ nguyên:

> **NGHIÊN CỨU TRƯỚC — KIỂM CHỨNG NGUỒN — PHẢN CHỨNG — HẬU KIỂM — TÀI LIỆU THAM KHẢO CUỐI CÙNG.**

Claude chỉ là một nền tảng chạy khác. Không vì đổi nền tảng mà hạ chuẩn chứng cứ hoặc thay đổi lõi nghiên cứu đã được kiểm ổn định.

---

# 13. GHI CHÚ VỀ GIAO DIỆN CLAUDE

Giao diện và tên nút của Claude có thể thay đổi theo phiên bản hoặc tài khoản. Nếu tên nút khác hướng dẫn này, giữ nguyên nguyên tắc ánh xạ:

- **Project instructions** = nơi đặt luật điều khiển hành vi;
- **Project knowledge/context** = nơi đặt 5 tệp `01`–`05`;
- **Research/Web search** = công cụ lấy nguồn bên ngoài khi câu hỏi cần nghiên cứu mở.

Theo tài liệu hỗ trợ Claude hiện hành, Project Knowledge được dùng xuyên các chat trong cùng Project; Project Instructions áp dụng cho các chat của Project; nội dung chat cũ không tự động trở thành Project Knowledge nếu chưa được thêm vào đó.
