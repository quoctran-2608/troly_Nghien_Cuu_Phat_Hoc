# HƯỚNG DẪN CÀI ĐẶT DỰ ÁN CHATGPT NGHIÊN CỨU PHẬT HỌC

## Mục tiêu

Thiết lập một Dự án ChatGPT riêng để mọi cuộc trò chuyện Phật học trong dự án đều dùng cùng một bộ quy tắc nghiên cứu và cùng một nền ngữ cảnh.

## Hai tệp cần dùng

1. `BO_QUY_TAC_NGHIEN_CUU_PHAT_HOC_TOAN_DIEN_v2.0.md` — bộ quy tắc đầy đủ.
2. `HUONG_DAN_DU_AN_CHATGPT_PHAT_HOC.txt` — phần chỉ dẫn ngắn để dán vào Hướng dẫn dự án.

## Các bước cài đặt

### Bước 1 — Tạo Dự án mới

Trong thanh bên của ChatGPT, chọn **Dự án mới**.

Đặt tên gợi ý:

> SƯ PHỤ — NGHIÊN CỨU PHẬT HỌC

### Bước 2 — Chọn bộ nhớ chỉ dành cho dự án

Mở dự án → chọn dấu ba chấm → **Cài đặt dự án** → **Bộ nhớ** → chọn **Bộ nhớ chỉ dành cho dự án** → **Lưu**.

Mục đích: các cuộc trò chuyện trong dự án dùng ngữ cảnh của chính dự án và không lấy ngữ cảnh từ các cuộc trò chuyện bên ngoài.

### Bước 3 — Tải bộ quy tắc đầy đủ vào Nguồn của dự án

Tải tệp sau vào phần nguồn/tệp của dự án:

> `BO_QUY_TAC_NGHIEN_CUU_PHAT_HOC_TOAN_DIEN_v2.0.md`

Không đổi nội dung tệp sau khi đã kiểm tra, trừ khi bạn muốn nâng phiên bản.

### Bước 4 — Dán Hướng dẫn dự án

Mở:

> `HUONG_DAN_DU_AN_CHATGPT_PHAT_HOC.txt`

Sao chép toàn bộ nội dung rồi dán vào ô **Hướng dẫn dự án** trong **Cài đặt dự án**.

Sau đó lưu lại.

### Bước 5 — Không cần dán lại bộ quy tắc trong từng cuộc trò chuyện

Từ đây, hãy mở mọi câu hỏi Phật học bên trong chính dự án này.

Bạn chỉ cần đưa yêu cầu thực tế, ví dụ:

> Hãy nghiên cứu chuyên sâu bài kinh sau, đặc biệt kiểm tra lịch sử hình thành, các truyền bản song song và khả năng có những lớp văn bản khác nhau.

Sau đó dán bài kinh hoặc tải tệp lên.

### Bước 6 — Kiểm tra cài đặt lần đầu

Mở một cuộc trò chuyện mới trong dự án và hỏi:

> Bạn đang áp dụng bộ quy tắc nghiên cứu Phật học nào? Hãy cho biết dấu hiệu phiên bản và nêu ngắn gọn 5 nguyên tắc bắt buộc về nguồn, thiên lệch, mức độ chắc chắn và tiếng Việt.

Kết quả mong đợi phải nhận ra dấu hiệu:

> `PHAT-HOC-2.0-VI`

### Bước 7 — Kiểm tra phương pháp luận

Hỏi tiếp:

> Nếu một đoạn chỉ xuất hiện trong bản Pāli nhưng không có trong một truyền bản Hán song song, theo bộ quy tắc bạn có được phép kết luận ngay rằng đoạn ấy được thêm vào về sau không? Vì sao?

Kết quả đúng phải nói rằng sự vắng mặt ở một truyền bản là một dữ kiện đáng chú ý nhưng **không đủ để tự động kết luận** đó là phần thêm về sau; cần thêm chứng cứ văn bản, ngữ văn, lịch sử và nghiên cứu chuyên ngành.

### Bước 8 — Kiểm tra tiếng Việt

Hỏi:

> Hãy giải thích cách bạn sẽ phân tầng một bài kinh. Không dùng lối viết nửa Việt nửa Anh; ngoại ngữ chỉ giữ khi thật sự cần để kiểm chứng.

Nếu câu trả lời vẫn dùng nhiều từ tiếng Anh không cần thiết, hãy kiểm tra lại rằng nội dung `HUONG_DAN_DU_AN_CHATGPT_PHAT_HOC.txt` đã được dán đầy đủ vào Hướng dẫn dự án.

## Cách sử dụng hằng ngày

Mỗi đề tài lớn hoặc mỗi bài kinh nên mở một cuộc trò chuyện riêng trong cùng dự án. Điều này giúp lịch sử trao đổi dễ theo dõi trong khi vẫn dùng chung tệp và hướng dẫn của dự án.

Khi nghiên cứu một bài kinh dài, nên yêu cầu lập bản đồ cấu trúc và thư mục nghiên cứu trước, rồi mới đi sâu vào từng đoạn.

## Khi nâng cấp bộ quy tắc

Nếu sau này có bản 2.1 hoặc 3.0:

1. tải bản mới vào dự án;
2. xóa hoặc lưu trữ bản cũ nếu không muốn gây nhầm lẫn;
3. sửa tên tệp và dấu hiệu phiên bản trong Hướng dẫn dự án;
4. mở cuộc trò chuyện mới và chạy lại ba bài kiểm tra ở trên.

## Lưu ý quan trọng

Bộ quy tắc là chỉ dẫn phương pháp luận, không phải tài liệu học thuật dùng làm chứng cứ. Khi trả lời câu hỏi thực tế, ChatGPT vẫn phải tìm và kiểm chứng các nguồn sơ cấp và nghiên cứu chuyên ngành phù hợp.
