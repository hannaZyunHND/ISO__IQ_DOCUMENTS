# BM-281: Form template Excel báo cáo điểm danh

## Thông tin biểu mẫu
- **Mã biểu mẫu**: QT-06-SOP-02-BM-17
- **Tên biểu mẫu**: Form template Excel báo cáo điểm danh
- **Phiên bản**: 1.0
- **Ngày ban hành**: 30/10/2025
- **Ngày hiệu lực**: 30/10/2025
- **SOP liên quan**: SOP-02.5

## Mục đích
Template Excel để hỗ trợ GVCN và BP HS tổng hợp, tính toán và báo cáo điểm danh.

## Nội dung biểu mẫu

```
═══════════════════════════════════════════════════════
        TEMPLATE EXCEL BÁO CÁO ĐIỂM DANH
═══════════════════════════════════════════════════════

CẤU TRÚC FILE EXCEL:

Sheet "Dữ liệu":
• Cột A: STT
• Cột B: Họ tên HS
• Cột C: Lớp
• Cột D: Ngày 1 (P/A/AP/L/E/I)
• Cột E: Ngày 2
• ... (Các ngày khác)
• Cột cuối: Tổng kết

Sheet "Báo cáo tuần":
• Tự động tính từ Sheet "Dữ liệu"
• Tỷ lệ đi học từng HS
• HS cần chú ý
• Thống kê tổng quan

Sheet "Báo cáo tháng":
• Tổng hợp từ các tuần
• Phân loại mức độ
• Biểu đồ trực quan
• Xu hướng

Sheet "Biểu đồ":
• Biểu đồ cột: Tỷ lệ theo tháng
• Biểu đồ tròn: Lý do vắng
• Biểu đồ đường: Xu hướng

CÔNG THỨC TÍNH TOÁN:

1. Tỷ lệ đi học:
   =COUNTIF(D2:Z2,"P")/COUNTA(D2:Z2)*100

2. Số lần vắng có phép:
   =COUNTIF(D2:Z2,"AP")

3. Số lần vắng không phép:
   =COUNTIF(D2:Z2,"A")

4. Số lần muộn:
   =COUNTIF(D2:Z2,"L")

5. Phân loại mức độ:
   =IF(B2>=90,"🟢",IF(B2>=80,"🟡",IF(B2>=70,"🟠","🔴")))

HƯỚNG DẪN SỬ DỤNG:

1. Nhập dữ liệu hàng ngày vào Sheet "Dữ liệu"
2. Các Sheet khác tự động cập nhật
3. In báo cáo từ Sheet tương ứng
4. Lưu file theo tên: "BaoCaoDiemDanh_[Lop]_[Thang].xlsx"

LƯU Ý:
• Backup file thường xuyên
• Kiểm tra công thức trước khi sử dụng
• Cập nhật template khi có thay đổi quy định
═══════════════════════════════════════════════════════
```

## Hướng dẫn sử dụng
1. Tải template về máy
2. Nhập dữ liệu điểm danh hàng ngày
3. Các báo cáo tự động cập nhật
4. In hoặc gửi file cho cấp trên

## Lưu ý
- Kiểm tra công thức trước khi sử dụng
- Backup file thường xuyên
- Cập nhật template khi cần thiết
