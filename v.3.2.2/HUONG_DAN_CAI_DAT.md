# HƯỚNG DẪN CÀI ĐẶT CHATGPT PROJECT — PHAT-HOC v3.2.2

**Phiên bản gói:** 3.2.2  
**Mục tiêu nâng cấp:** thêm danh mục **Tài liệu tham khảo** cuối bài mà không làm thay đổi lõi nghiên cứu đã được kiểm ổn định ở v3.2b.

---

# 1. NGUYÊN TẮC CỦA v3.2.2

v3.2.2 là một nâng cấp ở **lớp đầu ra**, không phải thay đổi kiến trúc nghiên cứu.

Bốn tệp nghiên cứu `01`–`04` và logic hậu kiểm hiện có được giữ nguyên từ nền v3.2b. Điểm mới nằm trong Project Instructions:

> **NGHIÊN CỨU XONG TRƯỚC → VIẾT VÀ HẬU KIỂM XONG → MỚI ĐÓNG GÓI CÁC NGUỒN ĐÃ DÙNG THÀNH “TÀI LIỆU THAM KHẢO”.**

Không được mở thêm một vòng tìm kiếm chỉ để làm danh mục đẹp, không đặt số lượng nguồn tối thiểu, không bổ sung nguồn chưa thực sự dùng hoặc kiểm. Mục tiêu là tăng khả năng kiểm chứng cho người đọc mà không làm AI phân tán khỏi bài nghiên cứu chính.

---

# 2. TẠO PROJECT

Nên tạo Project mới để kiểm thử, ví dụ:

`Trợ lý — NGHIÊN CỨU PHẬT HỌC v3.2.2 TEST`

Nếu đang có Project v3.2b ổn định, giữ nó làm bản đối chứng trong giai đoạn đầu.

---

# 3. TẢI 5 TỆP NGUỒN

Từ thư mục `v.3.2.2/sources/`, tải đúng 5 tệp:

1. `01_NGHIEN_CUU_COT_LOI.md`
2. `02_NGUON_VA_CHUNG_CU.md`
3. `03_PHAN_TANG_VAN_BAN.md`
4. `04_BAN_DO_NGUON_PHAT_HOC.md`
5. `05_HAU_KIEM.md`

Các tệp này giữ nền nghiên cứu/hậu kiểm đã được kiểm ở v3.2b; không thêm tệp thứ sáu chỉ để quản lý bibliography, nhằm tránh tăng nhiễu truy hồi.

Không tải các thư mục phiên bản cũ vào cùng Project.

---

# 4. DÁN PROJECT INSTRUCTIONS

Mở:

`HUONG_DAN_DU_AN_CHATGPT_PHAT_HOC_v3.2.2.txt`

Sao chép toàn bộ nội dung vào **Project Instructions / Hướng dẫn dự án**.

Marker mong đợi:

`PHAT-HOC-PROJECT-3.2.2-VI`

Các marker của 5 tệp nguồn vẫn thuộc họ `PHAT-HOC-3.2-*` vì lõi nguồn chưa thay đổi.

---

# 5. ĐIỂM MỚI: TÀI LIỆU THAM KHẢO CUỐI BÀI

Với câu trả lời nghiên cứu có sử dụng nguồn, đầu ra mặc định nên có mục:

## Tài liệu tham khảo

Khi thích hợp, chia thành:

### Văn bản gốc
- tên kinh/luận/văn bản;
- tên nguyên ngữ khi xác định được;
- mã định vị hoặc ấn bản đã dùng.

### Nghiên cứu hiện đại
- tác giả;
- năm;
- tên bài/sách;
- tạp chí hoặc nhà xuất bản;
- tập, số, trang nếu đã xác minh;
- DOI/URL chỉ khi hữu ích.

Không bịa dữ liệu thư mục còn thiếu. Độ chính xác quan trọng hơn hình thức đầy đủ giả tạo.

Danh mục chỉ gồm nguồn **thực sự đã dùng hoặc kiểm trong bài**. Nguồn chỉ dùng để khám phá, trang tổng hợp, favicon, snippet hoặc kết quả tìm kiếm không nên tự động xuất hiện trong danh mục nếu chúng không gánh mệnh đề nào.

---

# 6. QUY TẮC BẢO VỆ CHẤT LƯỢNG BÀI CHÍNH

Danh mục tham khảo không được:

- làm AI rút ngắn phần phân tích chính;
- thay phản chứng bằng danh sách nguồn;
- làm giảm việc truy nguồn trực tiếp;
- tạo quota số lượng tài liệu;
- kích hoạt tìm kiếm mới sau khi kết luận đã hoàn tất chỉ để “đủ bibliography”;
- khiến nguồn chưa kiểm trở thành nguồn “đã tham khảo”.

Nếu có xung đột giữa việc làm danh mục đẹp và việc bảo đảm mệnh đề đúng nguồn, **ưu tiên chất lượng nghiên cứu**.

---

# 7. TEST NHANH SAU KHI CÀI

Dùng một câu hỏi đủ sâu, ví dụ:

> `Đại thừa khởi tín luận có thật sự do Mã Minh (Aśvaghoṣa) soạn ở Ấn Độ không, hay đây là một tác phẩm hình thành tại Trung Quốc?`

Kiểm bốn điểm:

1. phần nghiên cứu chính vẫn sâu như v3.2b;
2. học giả Nhật/Trung Quốc và các tuyến ngoài tiếng Anh vẫn được mở khi có liên quan;
3. lần đầu nhắc kinh/văn bản vẫn dùng tên Việt + nguyên ngữ + mã khi xác định được;
4. cuối bài xuất hiện **Tài liệu tham khảo** chỉ gồm nguồn thực sự đã dùng/kiểm, với tác giả và dữ liệu thư mục không bị bịa.

Có thể hỏi tiếp bằng prompt ngắn để kiểm chiều sâu qua hội thoại; bibliography không được làm lượt sau mỏng đi.

---

# 8. CÁCH ĐÁNH GIÁ v3.2.2

Không kết luận từ một lần chạy. So sánh v3.2b và v3.2.2 bằng cùng prompt, cùng model và cùng mức suy luận.

Nếu phần chính giữ nguyên hoặc tốt hơn, còn danh mục tham khảo chính xác và hữu ích, nâng cấp đạt mục tiêu.

Nếu AI bắt đầu thu gom nguồn để làm danh mục, rút ngắn lập luận, hoặc liệt kê nguồn chưa thật sự kiểm, đó là lỗi cần sửa ở lớp đầu ra — không sửa lõi nghiên cứu nếu lõi vẫn hoạt động tốt.

---

# 9. TÓM TẮT

v3.2.2 giữ triết lý:

> **NGHIÊN CỨU TRƯỚC — HẬU KIỂM SAU — TÀI LIỆU THAM KHẢO CUỐI CÙNG.**

Bibliography là sản phẩm phụ của một nghiên cứu đã hoàn tất, không phải mục tiêu điều khiển quá trình nghiên cứu.
