# BM-349: LỊCH BACKUP DỮ LIỆU

## Mã biểu mẫu
QT-06-SOP-06-BM-349

## Phiên bản
1.0

## Ngày ban hành
30/10/2024

## Ngày hiệu lực
01/11/2024

## Mục đích
Theo dõi lịch backup dữ liệu hệ thống quản lý học sinh

## Hướng dẫn sử dụng
- Ghi chép đầy đủ thông tin backup
- Kiểm tra định kỳ theo lịch
- Báo cáo ngay nếu có sự cố

## Nội dung biểu mẫu

```
═══════════════════════════════════════════════════════
              LỊCH BACKUP DỮ LIỆU
═══════════════════════════════════════════════════════

Tháng: ____  Năm: ____

┌──────┬──────────┬──────────┬──────────┬──────────┬──────────┐
│ Ngày │   Giờ    │   Loại   │  Kích    │  Trạng   │  Ghi chú │
│      │          │ Backup   │  thước   │  thái    │          │
├──────┼──────────┼──────────┼──────────┼──────────┼──────────┤
│ 1    │ 01:00    │ Incremental│ 2.5GB  │ ✅ OK    │          │
│ 2    │ 01:00    │ Incremental│ 1.8GB  │ ✅ OK    │          │
│ 3    │ 01:00    │ Incremental│ 3.2GB  │ ✅ OK    │          │
│ 4    │ 01:00    │ Incremental│ 2.1GB  │ ✅ OK    │          │
│ 5    │ 01:00    │ Incremental│ 2.9GB  │ ✅ OK    │          │
│ 6    │ 01:00    │ Incremental│ 2.3GB  │ ✅ OK    │          │
│ 7    │ 01:00    │ Incremental│ 2.7GB  │ ✅ OK    │          │
│ 8    │ 01:00    │ Incremental│ 2.4GB  │ ✅ OK    │          │
│ 9    │ 01:00    │ Incremental│ 2.8GB  │ ✅ OK    │          │
│ 10   │ 01:00    │ Incremental│ 2.6GB  │ ✅ OK    │          │
│ 11   │ 01:00    │ Incremental│ 2.2GB  │ ✅ OK    │          │
│ 12   │ 01:00    │ Incremental│ 2.5GB  │ ✅ OK    │          │
│ 13   │ 01:00    │ Incremental│ 2.8GB  │ ✅ OK    │          │
│ 14   │ 01:00    │ Incremental│ 2.3GB  │ ✅ OK    │          │
│ 15   │ 01:00    │ Incremental│ 2.7GB  │ ✅ OK    │          │
│ 16   │ 01:00    │ Incremental│ 2.4GB  │ ✅ OK    │          │
│ 17   │ 01:00    │ Incremental│ 2.9GB  │ ✅ OK    │          │
│ 18   │ 01:00    │ Incremental│ 2.1GB  │ ✅ OK    │          │
│ 19   │ 01:00    │ Incremental│ 2.6GB  │ ✅ OK    │          │
│ 20   │ 01:00    │ Incremental│ 2.8GB  │ ✅ OK    │          │
│ 21   │ 01:00    │ Incremental│ 2.3GB  │ ✅ OK    │          │
│ 22   │ 01:00    │ Incremental│ 2.5GB  │ ✅ OK    │          │
│ 23   │ 01:00    │ Incremental│ 2.7GB  │ ✅ OK    │          │
│ 24   │ 01:00    │ Incremental│ 2.4GB  │ ✅ OK    │          │
│ 25   │ 01:00    │ Incremental│ 2.8GB  │ ✅ OK    │          │
│ 26   │ 01:00    │ Incremental│ 2.2GB  │ ✅ OK    │          │
│ 27   │ 01:00    │ Incremental│ 2.6GB  │ ✅ OK    │          │
│ 28   │ 01:00    │ Incremental│ 2.9GB  │ ✅ OK    │          │
│ 29   │ 01:00    │ Incremental│ 2.3GB  │ ✅ OK    │          │
│ 30   │ 01:00    │ Incremental│ 2.5GB  │ ✅ OK    │          │
│ 31   │ 01:00    │ Incremental│ 2.7GB  │ ✅ OK    │          │
└──────┴──────────┴──────────┴──────────┴──────────┴──────────┘

BACKUP TUẦN (Chủ nhật):
┌──────┬──────────┬──────────┬──────────┬──────────┬──────────┐
│ Tuần │   Ngày   │   Loại   │  Kích    │  Trạng   │  Ghi chú │
│      │          │ Backup   │  thước   │  thái    │          │
├──────┼──────────┼──────────┼──────────┼──────────┼──────────┤
│ 1    │ 07/__    │ Full     │ 15.2GB   │ ✅ OK    │          │
│ 2    │ 14/__    │ Full     │ 15.8GB   │ ✅ OK    │          │
│ 3    │ 21/__    │ Full     │ 16.1GB   │ ✅ OK    │          │
│ 4    │ 28/__    │ Full     │ 16.5GB   │ ✅ OK    │          │
└──────┴──────────┴──────────┴──────────┴──────────┴──────────┘

BACKUP THÁNG:
┌──────┬──────────┬──────────┬──────────┬──────────┬──────────┐
│ Tháng│   Ngày   │   Loại   │  Kích    │  Trạng   │  Ghi chú │
│      │          │ Backup   │  thước   │  thái    │          │
├──────┼──────────┼──────────┼──────────┼──────────┼──────────┤
│ __   │ 30/__    │ Full     │ 18.2GB   │ ✅ OK    │          │
└──────┴──────────┴──────────┴──────────┴──────────┴──────────┘

TỔNG KẾT:
- Backup hằng ngày: ✅ Thành công
- Backup hằng tuần: ✅ Thành công  
- Backup hằng tháng: ✅ Thành công
- Tổng dung lượng: ____ GB
- Số lần lỗi: ____

NGƯỜI THỰC HIỆN:
Họ tên: _______________  Chức vụ: _______
Ký tên: _______________  Ngày: __/__/____

NGƯỜI KIỂM TRA:
Họ tên: _______________  Chức vụ: _______
Ký tên: _______________  Ngày: __/__/____
═══════════════════════════════════════════════════════
```

## Lưu ý quan trọng
- Backup hằng ngày: 1h sáng (Incremental)
- Backup hằng tuần: Chủ nhật (Full)
- Backup hằng tháng: Ngày 30 (Full)
- Kiểm tra định kỳ: Mỗi tuần
- Test restore: Mỗi học kỳ
