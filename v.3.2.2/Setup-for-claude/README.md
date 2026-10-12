# SETUP FOR CLAUDE — PHAT-HOC v3.2.2

Thư mục này là **bộ cài độc lập dành cho Claude Projects**, phát triển từ lõi PHAT-HOC v3.2.2 đã kiểm ổn định trên ChatGPT Project.

Mục tiêu không phải tạo một phương pháp nghiên cứu khác, mà là giữ nguyên lõi `01`–`05` và thêm một lớp điều phối nhỏ phù hợp với hành vi quan sát được khi chạy Claude.

## Cấu trúc

```text
Setup-for-claude/
├── README.md
├── HUONG_DAN_CAI_DAT_CLAUDE_PROJECT.md
├── HUONG_DAN_DU_AN_CLAUDE_PHAT_HOC_v3.2.2.txt
└── sources/
    ├── 01_NGHIEN_CUU_COT_LOI.md
    ├── 02_NGUON_VA_CHUNG_CU.md
    ├── 03_PHAN_TANG_VAN_BAN.md
    ├── 04_BAN_DO_NGUON_PHAT_HOC.md
    └── 05_HAU_KIEM.md
```

## Nguyên tắc phiên bản

- Năm tệp `sources/01`–`05` là bản sao nguyên vẹn của lõi v3.2.2; không chỉnh riêng cho Claude.
- Tệp `HUONG_DAN_DU_AN_CLAUDE_PHAT_HOC_v3.2.2.txt` là Project Instructions đã ghép sẵn lớp điều phối dành cho Claude với lõi Instructions v3.2.2.
- Các bổ sung Claude gồm **hai điều chỉnh học thuật** đã thấy lặp qua benchmark: **ưu tiên đóng nguồn trực tiếp cho mệnh đề trụ cột** và **không để câu kết luận mạnh hơn phạm vi chứng cứ thực sự đã kiểm**; cùng **một lan can đầu ra**: hậu kiểm chủ yếu phải sửa sản phẩm cuối, không biến checklist/trạng thái nội bộ thành phần trình diễn cho người dùng.
- Không thêm quota nguồn, không ép trả lời ngắn, không làm yếu ưu thế nghiên cứu rộng và sâu của Claude.

## Cài nhanh

1. Tạo Claude Project mới.
2. Tải 5 tệp trong `sources/` vào Project Knowledge/Context.
3. Dán toàn bộ `HUONG_DAN_DU_AN_CLAUDE_PHAT_HOC_v3.2.2.txt` vào Project Instructions.
4. Bảo đảm tính năng Memory của Claude đang hoạt động; trong Project mở **Memory → View** để xem Project memory. Project memory được duy trì riêng cho Project; đặt **Use account memory = OFF** để không nối vùng nhớ này với các chat ngoài Project. Dòng `No memory yet` chỉ có nghĩa Project chưa tích lũy đủ memory.
5. Với nghiên cứu mở, bật **Research** và bảo đảm **Web search** khả dụng. Sau đó chọn một trong hai option:
   - **OPTION A — MẠNH NHẤT:** model top-tier đã benchmark tốt nhất + **Max** + **Research ON** + Web search; dùng khi cần chất lượng tối đa hoặc benchmark khó.
   - **OPTION B — HẰNG NGÀY:** model top-tier đã chọn + **High** + Research khi câu hỏi cần nghiên cứu mở; dùng để cân bằng chất lượng, tốc độ và usage.
   `Auto` là chế độ quyền hành động, không phải mức suy luận; có thể để Auto cho tác vụ chỉ đọc/tìm kiếm để giảm ngắt quãng, nhưng dùng Manual khi có công cụ có thể ghi/xóa hay tạo hành động có hậu quả.

Nếu không có lý do đặc biệt để tiết kiệm thời gian/usage và câu hỏi thực sự quan trọng, ưu tiên **OPTION A — MẠNH NHẤT**.

Tên model và giao diện Claude có thể thay đổi. Xem `HUONG_DAN_CAI_DAT_CLAUDE_PROJECT.md` để biết cấu hình chi tiết, cách hiểu `Research`, `High/Max`, `Thinking`, `Auto`, Memory và quy trình benchmark.
