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
- Các bổ sung Claude chỉ nhằm hai việc đã thấy lặp qua benchmark: **ưu tiên đóng nguồn trực tiếp cho mệnh đề trụ cột** và **không để câu kết luận mạnh hơn phạm vi chứng cứ thực sự đã kiểm**.
- Không thêm quota nguồn, không ép trả lời ngắn, không làm yếu ưu thế nghiên cứu rộng và sâu của Claude.

## Cài nhanh

1. Tạo Claude Project mới.
2. Tải 5 tệp trong `sources/` vào Project Knowledge/Context.
3. Dán toàn bộ `HUONG_DAN_DU_AN_CLAUDE_PHAT_HOC_v3.2.2.txt` vào Project Instructions.
4. Để Project memory hoạt động bình thường; đặt **Use account memory = OFF**.
5. Bật Research/Web search khi làm câu hỏi nghiên cứu mở nếu tài khoản có hỗ trợ.

Xem `HUONG_DAN_CAI_DAT_CLAUDE_PROJECT.md` để cài chi tiết và benchmark.
