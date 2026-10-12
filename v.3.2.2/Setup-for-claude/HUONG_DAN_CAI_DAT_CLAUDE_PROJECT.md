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
- bảo đảm **Web search** khả dụng; Research cần Web search để hoạt động;
- không coi kết quả search, snippet, abstract hay metadata là đã đọc toàn văn;
- ưu tiên các hạ tầng chuyên ngành theo `04_BAN_DO_NGUON_PHAT_HOC.md`, nhưng không biến Source Map thành whitelist.

Research là chế độ nghiên cứu nhiều lượt: Claude có thể tự thực hiện các lượt tìm kiếm nối tiếp, mở các hướng khác nhau và quyết định cần điều tra gì tiếp theo. Đây là chế độ nên dùng cho các câu hỏi nghiên cứu mở của Project này.

Người dùng vẫn chỉ cần hỏi tự nhiên; không cần lặp “hãy research sâu” trong từng prompt nếu Project hoạt động đúng.

## 4.1. CẤU HÌNH KHUYẾN NGHỊ ĐỂ NGHIÊN CỨU MẠNH NHẤT

Tên model và giao diện Claude có thể thay đổi. Vì vậy ưu tiên nguyên tắc **model mạnh nhất phù hợp → effort đủ cao → Research + Web search cho câu hỏi mở**, thay vì khóa vĩnh viễn vào một tên model.

### CHỌN NHANH MỘT TRONG HAI OPTION

#### OPTION A — MẠNH NHẤT / MAX QUALITY

Dùng khi mục tiêu là **chất lượng nghiên cứu cao nhất có thể**, đặc biệt cho benchmark, tác quyền, niên đại, phân tầng văn bản, so sánh triết học khó hoặc tranh luận học giới phức tạp.

```text
Model:             model top-tier mạnh nhất đã benchmark tốt nhất
                   (hiện có thể dùng Opus 5.5; nếu có Fable 5.1 thì so cùng prompt)
Effort:            Max
Research:          ON
Web search:        ON / khả dụng
Thinking:          dùng cơ chế Thinking hiện hành của model; không cần bật thêm nếu model đã tự dùng
Permission mode:   Auto nếu chỉ đọc/tìm kiếm và muốn giảm ngắt quãng
                   Manual nếu có công cụ có thể ghi/xóa hoặc tạo hành động có hậu quả
Memory:            theo cấu hình ở mục 5
```

Đây là **option ưu tiên chất lượng hơn tốc độ và mức tiêu thụ**. Nếu đang đánh giá năng lực tối đa của Project, dùng option này và giữ nguyên cấu hình cho toàn bộ loạt benchmark.

#### OPTION B — NGHIÊN CỨU HẰNG NGÀY / CÂN BẰNG

Dùng khi muốn giữ chất lượng nghiên cứu rất cao nhưng tiết kiệm thời gian và giới hạn sử dụng hơn.

```text
Model:             model top-tier đã chọn làm mặc định
Effort:            High
Research:          ON khi câu hỏi cần nghiên cứu mở
Web search:        khả dụng
Permission mode:   Auto hoặc Manual tùy quyền của công cụ đang nối
Memory:            theo cấu hình ở mục 5
```

Nếu không có lý do đặc biệt để tiết kiệm thời gian/usage và câu hỏi thực sự quan trọng, ưu tiên **OPTION A — MẠNH NHẤT**.

Tại thời điểm cập nhật **10/2026**, cấu hình khuyến nghị cho Project này là:

```text
Model:             Claude Opus 5.5 nếu tài khoản có
                   Fable 5.1 là lựa chọn top-tier khác; nếu có cả hai,
                   nên benchmark cùng prompt trước khi đổi model mặc định
Effort:            Max cho bài khó/benchmark quan trọng
                   High cho sử dụng nghiên cứu hằng ngày
Research:          ON cho câu hỏi nghiên cứu mở
Web search:        ON / khả dụng — bắt buộc để Research hoạt động
Thinking:          luôn hoạt động trên Opus 5.5 và Fable 5.1;
                   không cần tìm thêm một nút bật Thinking
Permission mode:   Auto có thể dùng cho tác vụ đọc/tìm kiếm để giảm ngắt quãng;
                   Manual khi có công cụ có thể ghi/xóa hoặc hành động có hậu quả
Memory:            theo cấu hình ở mục 5
```

### Model

Nếu giao diện đang có **Claude Opus 5.5**, đây là lựa chọn rất mạnh và phù hợp làm model mặc định cho Project nghiên cứu này. Nếu tài khoản đồng thời có **Fable 5.1**, coi đó là một lựa chọn cao cấp khác; không tự động kết luận model nào tốt hơn cho Phật học mà nên chạy cùng bộ benchmark trước khi thay model mặc định.

Khi benchmark, không đổi model giữa các bài rồi quy chênh lệch cho skill.

### Effort: High hay Max?

- **Max**: dùng khi cần chất lượng tối đa — tác quyền, niên đại, phân tầng văn bản, so sánh triết học khó, tranh luận học giới, hoặc benchmark quan trọng. Max là mức kỹ nhất nhưng chậm hơn và tiêu tốn usage/token nhiều hơn.
- **High**: mặc định tốt cho nghiên cứu hằng ngày; cân bằng chất lượng, tốc độ và giới hạn sử dụng.
- Không hạ xuống Low/Medium trong một phép benchmark nếu mục tiêu là đo năng lực tối đa của hệ.

### Thinking

Với **Opus 5.5** và **Fable 5.1**, Thinking luôn hoạt động ở mọi mức effort trong Claude hiện tại. Không cần tìm thêm một công tắc Thinking để “bật cho mạnh hơn”.

### `Auto` trong giao diện mới

Nếu giao diện hiển thị `Auto` cạnh model/effort, cần hiểu đúng: đây là **chế độ quyền hành động**, không phải mức thông minh hay độ sâu suy luận.

- Với Project này chủ yếu đọc nguồn, tìm web và nghiên cứu, có thể để **Auto** để Claude ít bị ngắt vì các bước xin phép.
- `Auto` **không làm model thông minh hơn** và không thay thế `High/Max` hay `Research`.
- Nếu đã nối các công cụ có khả năng gửi, ghi, sửa hoặc xóa dữ liệu bên ngoài, nên cân nhắc **Manual** để tự duyệt hành động.

### Tóm tắt lại hai option

**OPTION A — Mạnh nhất / benchmark khó:**

```text
Opus 5.5 (hoặc model top-tier đã benchmark tốt hơn)
+ Max
+ Research ON
+ Web search khả dụng
+ Auto nếu chỉ đọc/tìm kiếm và muốn giảm ngắt quãng
```

**OPTION B — Nghiên cứu hằng ngày:**

```text
Opus 5.5 (hoặc model top-tier đã chọn)
+ High
+ Research ON khi câu hỏi cần nghiên cứu mở
+ Web search khả dụng
```

Không cần bật Research cho tác vụ thuần dịch, phiên âm, chính tả, nhận diện locator hoặc câu hỏi đơn điểm không cần nghiên cứu mở.

---

# 5. MEMORY

## 5.1. Hiểu đúng ba lớp Memory

Với Claude Project, cần phân biệt rõ:

1. **Memory của Claude ở cấp tài khoản:** tính năng Memory tổng thể phải đang hoạt động để Claude có thể sử dụng cơ chế nhớ.
2. **Project memory:** vùng nhớ riêng của Project hiện tại. Trong giao diện Project, mở **Memory → View** để xem nội dung vùng nhớ này khi đã hình thành. Project memory tách biệt với các Project khác và với chat ngoài Project, trừ khi người dùng cho phép nối account memory.
3. **Use account memory:** công tắc quyết định Project này có được dùng/chia sẻ memory với các chat ngoài Project hay không. Đây **không phải** công tắc bật/tắt Project memory.

Cấu hình khuyến nghị cho Project Phật học này:

```text
Memory của Claude:   bật / đang hoạt động
Project memory:      riêng cho Project; xem tại Memory → View
Use account memory:  OFF
```

Với cấu hình này:

- Claude vẫn duy trì **Project memory riêng** cho trợ lý nghiên cứu Phật học;
- **Use account memory = OFF** giúp tránh đưa memory từ các chat ngoài Project vào đây;
- nếu cửa sổ Memory hiện `No memory yet`, điều đó chỉ có nghĩa Project chưa tích lũy đủ memory để hiển thị; **không có nghĩa Project memory đang bị tắt**;
- Project memory không thay thế Project Knowledge hay Project Instructions. Năm tệp `01`–`05` và Instructions vẫn là nền phương pháp cố định của hệ.

## 5.2. Khi benchmark A/B nghiêm

Để giảm ảnh hưởng giữa các phép thử:

- mở **chat mới** cho mỗi prompt độc lập;
- nếu cần cô lập tuyệt đối một phép thử và giao diện cho phép, mở chat mới rồi tắt **Memory** cho chính chat đó **trước khi gửi tin nhắn đầu tiên**;
- không bật `Use account memory` chỉ để mong Claude “nhớ nhiều hơn”, vì điều đó đưa thêm biến từ các chat ngoài Project vào benchmark.

Trong sử dụng hằng ngày, giữ Project memory riêng của Project hoạt động là phù hợp; chỉ cần để **Use account memory = OFF** theo cấu hình trên.

---

# 6. MODEL VÀ BENCHMARK

Khi so với ChatGPT:

- dùng model Claude mạnh nhất mà tài khoản cho phép và đã chọn trước khi bắt đầu loạt test;
- với phép thử năng lực tối đa, ưu tiên **OPTION A / Max**; nếu so ở chế độ sử dụng thường ngày, dùng **OPTION B / High**;
- giữ nguyên model, effort, trạng thái Research và các điều kiện công cụ cho toàn bộ một loạt test;
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
- coi `Auto` là mức suy luận cao hơn `High/Max`;
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
│   ├── Memory của Claude: bật / đang hoạt động
│   ├── Project memory: riêng cho Project; xem tại Memory → View
│   └── Use account memory: OFF
│
└── Khi nghiên cứu
    ├── OPTION A — Mạnh nhất: model top-tier + Max + Research ON + Web search
    ├── OPTION B — Hằng ngày: model top-tier + High + Research khi cần
    ├── Auto: tùy quyền hành động; không phải mức suy luận
    └── chat mới cho benchmark độc lập
```

Triết lý giữ nguyên:

> **NGHIÊN CỨU TRƯỚC — TRUY NGUỒN TRỰC TIẾP — PHẢN CHỨNG — HIỆU CHỈNH KẾT LUẬN — HẬU KIỂM — TÀI LIỆU THAM KHẢO CUỐI CÙNG.**
