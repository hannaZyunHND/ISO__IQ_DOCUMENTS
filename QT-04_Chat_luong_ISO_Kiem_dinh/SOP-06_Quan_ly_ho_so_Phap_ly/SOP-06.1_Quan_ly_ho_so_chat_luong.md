# SOP-06.1: QUẢN LÝ HỒ SƠ CHẤT LƯỢNG

## 1. THÔNG TIN QUY TRÌNH

| **Thuộc tính** | **Nội dung** |
|---|---|
| Mã SOP | SOP-06.1 |
| Tên quy trình | Quản lý hồ sơ chất lượng |
| Quy trình cha | SOP-06: Quản lý hồ sơ - Pháp lý |
| Phiên bản | 1.0 |
| Tần suất | Liên tục |

## 2. MỤC ĐÍCH

- **Bằng chứng hoạt động**: Hồ sơ chứng minh đã thực hiện theo quy trình
- **Truy vết được**: Tìm lại thông tin khi cần
- **Phục vụ audit/kiểm định**: Auditor yêu cầu xem hồ sơ → Cung cấp ngay
- **Tuân thủ ISO**: Yêu cầu Điều 7.5.3 ISO 9001

## 3. PHÂN LOẠI HỒ SƠ CHẤT LƯỢNG

### 3.1. Phân loại theo tính chất

| **Loại** | **Ví dụ** | **Người quản lý** |
|---|---|---|
| **Hồ sơ Chính sách, Mục tiêu** | Chính sách CL, Bảng KPI năm, Biên bản MR | Ban ISO |
| **Hồ sơ Audit** | Kế hoạch audit, BC audit, CAR, Chứng chỉ Auditor | Ban ISO |
| **Hồ sơ Đào tạo** | Danh sách đào tạo, Chứng chỉ, Bài thi | Phòng NS |
| **Hồ sơ Quy trình** | Biên bản họp, Checklist, Phiếu kiểm tra | BP liên quan |
| **Hồ sơ Khách hàng** | Khảo sát hài lòng, Khiếu nại, Xử lý | Ban ISO + BP |
| **Hồ sơ Nhà cung cấp** | Đánh giá NCC, Hợp đồng, Nghiệm thu | Phòng KT, Hành chính |
| **Hồ sơ Cải tiến** | Đề xuất CI, BC dự án, Đánh giá hiệu quả | Ban ISO |

### 3.2. Phân loại theo thời gian lưu

| **Loại** | **Thời gian lưu** | **Ví dụ** |
|---|---|---|
| **Vĩnh viễn** | Mãi mãi | BCTC năm, Chứng chỉ ISO, Giấy phép |
| **Dài hạn (10 năm)** | 10 năm | Hồ sơ audit, CAR, Hợp đồng |
| **Trung hạn (5 năm)** | 5 năm | BC tháng/quý, Đào tạo |
| **Ngắn hạn (2-3 năm)** | 2-3 năm | Checklist, Phiếu kiểm tra |

## 4. QUY TRÌNH QUẢN LÝ HỒ SƠ

### 4.1. Tạo hồ sơ

**Bước 1: Khi thực hiện quy trình → Tạo hồ sơ**

Ví dụ:
- Audit → Tạo: BC audit, Checklist, CAR
- Đào tạo → Tạo: Danh sách tham dự, Bài thi, Chứng chỉ
- Khiếu nại → Tạo: Đơn khiếu nại, BC xử lý, Biên bản

**Bước 2: Điền đầy đủ, Ký đúng quy định**

**Bước 3: Scan hoặc Lưu file gốc (Nếu đã điện tử)**

### 4.2. Lưu trữ

**Bước 4: Đặt tên file chuẩn**

**Format:** `[Loại]_[Ngày]_[Tên].[Đuôi]`

Ví dụ:
- `BC_Audit_20241112_Phong_Hoc_thuat.pdf`
- `CAR_20241115_001_Hoc_thuat.docx`
- `Checklist_Audit_20241112.xlsx`

**Bước 5: Lưu vào đúng thư mục**

**Cấu trúc thư mục Server:**

```
\\Server\ISO\
├─ 01_Chinh_sach_Muc_tieu\
│  ├─ 2024\
│  │  ├─ Chinh_sach_CL_Ver1.0.pdf
│  │  └─ Bang_KPI_2024.xlsx
│  └─ 2025\
├─ 02_Audit\
│  ├─ 2024\
│  │  ├─ Dot_1_T11\
│  │  │  ├─ Ke_hoach_audit.pdf
│  │  │  ├─ BC_Audit_Hoc_thuat.pdf
│  │  │  └─ CAR_001.docx
│  │  └─ Dot_2_T5\
│  └─ 2025\
├─ 03_Dao_tao\
├─ 04_Khach_hang\
│  ├─ Khao_sat\
│  ├─ Khieu_nai\
│  └─ Xu_ly\
├─ 05_Cai_tien\
├─ 06_Phap_ly\
└─ 07_Khac\
```

**Bước 6: Quyền truy cập**

| **Thư mục** | **Quyền đọc** | **Quyền ghi** |
|---|---|---|
| Chính sách, Mục tiêu | Tất cả | Ban ISO |
| Audit | BGH, Ban ISO, Auditor | Ban ISO |
| Đào tạo | BGH, NS, Ban ISO | NS |
| Khách hàng | BGH, Ban ISO | Ban ISO |

### 4.3. Tra cứu

**Bước 7: Khi cần tra cứu**

**Phương pháp:**
- Tìm kiếm trên server (Ctrl+F)
- Hoặc tra Danh mục hồ sơ (QT04-S08 - Excel)

**Danh mục hồ sơ:**

| **STT** | **Loại HS** | **Tên file** | **Ngày** | **Vị trí** | **Thời hạn lưu** | **Ngày hủy** |
|---|---|---|---|---|---|---|
| 1 | BC Audit | BC_Audit_Hoc_thuat_T11_2024 | 12/11/24 | \\Server\ISO\02_Audit\2024\Dot_1 | 10 năm | 12/11/2034 |

**Bước 8: Cung cấp hồ sơ khi được yêu cầu**

### 4.4. Bảo quản

**Bước 9: Backup định kỳ**

| **Tần suất** | **Phương pháp** | **Vị trí** |
|---|---|---|
| Hàng ngày | Tự động backup | Server phụ |
| Hàng tuần | Backup incremental | Cloud (Google Drive) |
| Hàng tháng | Backup full | Ổ cứng ngoài |

**Bước 10: Kiểm tra định kỳ (6 tháng)**

- Backup có hoạt động không?
- File có mở được không?
- Có virus không?

### 4.5. Thanh lý

**Bước 11: Hết thời hạn lưu → Thanh lý**

**Quy trình thanh lý:**
- Lập Danh sách hồ sơ hết hạn (QT04-D16)
- BGH ký duyệt thanh lý
- Xóa trên server
- Cập nhật Danh mục

**LƯU Ý:** Hồ sơ vĩnh viễn KHÔNG thanh lý!

## 5. LƯU ĐỒ QUY TRÌNH

```mermaid
graph TD
    A[Thực hiện quy trình] --> B[Tạo hồ sơ: BC, Biên bản, Checklist...]
    B --> C[Điền đầy đủ, Ký đúng]
    C --> D[Scan hoặc Lưu file gốc]
    D --> E[Đặt tên file chuẩn]
    E --> F[Lưu vào đúng thư mục Server]
    F --> G[Phân quyền truy cập]
    G --> H[Nhập Danh mục hồ sơ]
    
    H --> I[Backup tự động hàng ngày]
    I --> J[Backup tuần lên Cloud]
    J --> K[Backup tháng ra ổ cứng]
    
    L[Khi cần tra cứu] --> M[Tìm trên Server hoặc Danh mục]
    M --> N[Mở file xem]
    N --> O{Cần in/Gửi?}
    O -->|Có| P[In/Gửi email]
    O -->|Không| Q[Chỉ xem]
    
    R[6 tháng: Kiểm tra] --> S[Backup OK?]
    S --> T[File mở được?]
    T --> U[Có virus?}
    U --> V{Có vấn đề?}
    V -->|Có| W[Khắc phục ngay]
    V -->|Không| X[OK]
    
    Y[Hết hạn lưu] --> Z{Loại HS?}
    Z -->|Vĩnh viễn| AA[KHÔNG thanh lý]
    Z -->|10 năm, 5 năm...| AB[Lập danh sách thanh lý]
    AB --> AC[BGH duyệt]
    AC --> AD[Xóa khỏi server]
    AD --> AE[Cập nhật Danh mục]
```

## 6. BIỂU MẪU LIÊN QUAN

| **Mã** | **Tên** |
|---|---|
| QT04-S08 | Danh mục hồ sơ chất lượng |
| QT04-D16 | Danh sách hồ sơ thanh lý |
| QT04-F18 | Form đề nghị tra cứu hồ sơ |

## 7. TIÊU CHUẨN VÀ CHỈ TIÊU

| **Chỉ tiêu** | **Mục tiêu** |
|---|---|
| Hồ sơ được tạo đầy đủ | 100% |
| Tìm được hồ sơ khi cần | ≤ 5 phút |
| Mất mát hồ sơ | 0% |
| Backup thành công | 100% |

## 8. TRÁCH NHIỆM CỤ THỂ

| **Vai trò** | **Trách nhiệm** |
|---|---|
| **BP thực hiện quy trình** | Tạo hồ sơ, Điền đầy đủ, Lưu đúng chỗ |
| **Ban ISO** | Quản lý hồ sơ ISO, Danh mục, Hướng dẫn |
| **IT** | Quản lý server, Backup, Phân quyền, Bảo mật |

## 9. LƯU Ý QUAN TRỌNG

- ⚠️ **Hồ sơ = Bằng chứng**: "Không có hồ sơ = Không làm" (Theo ISO)
- ✅ **Lưu đầy đủ**: Auditor hỏi gì cũng phải có
- ✅ **Dễ tìm**: Cấu trúc thư mục logic, Đặt tên chuẩn
- ✅ **Bảo mật**: Hồ sơ nhạy cảm (Lương, Khiếu nại...) phân quyền chặt
- 🔥 **Backup quan trọng**: Server hỏng = Mất tất cả → Tai họa!

## 10. PHỤ LỤC

### 10.1. Danh sách hồ sơ chất lượng chính

**A. Hồ sơ Chính sách & Mục tiêu:**
- Chính sách CL (Tất cả phiên bản)
- Bảng KPI hàng năm
- Biên bản Management Review (2 lần/năm)

**B. Hồ sơ Audit:**
- Kế hoạch audit năm
- Chứng chỉ Auditor
- Checklist audit
- Báo cáo audit (Mỗi lần)
- CAR/PAR (Tất cả)
- Biên bản đóng CAR

**C. Hồ sơ Đào tạo:**
- Kế hoạch đào tạo năm
- Danh sách tham dự (Mỗi khóa)
- Tài liệu đào tạo
- Bài thi, Kết quả
- Chứng chỉ hoàn thành
- Đánh giá hiệu quả đào tạo

**D. Hồ sơ Khách hàng:**
- Khảo sát hài lòng (2 lần/năm)
- Phân tích kết quả khảo sát
- Đơn khiếu nại
- Báo cáo xử lý khiếu nại
- Biên bản đóng khiếu nại

**E. Hồ sơ Nhà cung cấp:**
- Danh sách NCC
- Đánh giá NCC hàng năm
- Hợp đồng
- Biên bản nghiệm thu

**F. Hồ sơ Cải tiến:**
- Sổ ý tưởng CI
- Project Charter
- Báo cáo dự án
- Đánh giá hiệu quả

**G. Hồ sơ Kiểm định:**
- Hồ sơ tự đánh giá
- Báo cáo kiểm định
- Chứng nhận kiểm định
- Kế hoạch khắc phục (Nếu có)

### 10.2. Checklist kiểm tra hồ sơ

**TRƯỚC KHI LƯU TRỮ:**
- [ ] Hồ sơ đã hoàn chỉnh (Không thiếu trang)
- [ ] Đủ chữ ký yêu cầu
- [ ] Ngày tháng rõ ràng
- [ ] Scan rõ nét (Nếu từ giấy)
- [ ] Đặt tên file chuẩn
- [ ] Lưu đúng thư mục
- [ ] Đã nhập Danh mục
- [ ] Đã phân quyền

**KHI AUDITOR YÊU CẦU:**
- [ ] Tìm được trong ≤ 5 phút
- [ ] File mở được, Không lỗi
- [ ] Nội dung đầy đủ
- [ ] Là phiên bản mới nhất

### 10.3. Ví dụ yêu cầu Auditor

**Auditor:** "Cho tôi xem Báo cáo Audit Phòng Học thuật lần gần nhất."

**BP:** [Vào server] → `\\ISO\02_Audit\2024\Dot_1\BC_Audit_Hoc_thuat_T11_2024.pdf` → Mở trong 2 phút

**Auditor:** "Có bao nhiêu NC?"

**BP:** "3 NC nhỏ. Đây ạ [Chỉ vào BC]"

**Auditor:** "Cho tôi xem CAR của 3 NC đó."

**BP:** [Mở thư mục CAR] → `CAR_001.docx`, `CAR_002.docx`, `CAR_003.docx`

**Auditor:** "Các CAR này đã đóng chưa?"

**BP:** "CAR-001 và 002 đã đóng. CAR-003 đang xử lý, hạn 15/12."

**Auditor:** "OK. Cho tôi xem bằng chứng đóng CAR-001."

**BP:** [Mở CAR-001] → Phần 4 có chữ ký Auditor xác nhận đóng

→ **NẾU BP TÌM KHÔNG RA TRONG 5 PHÚT = NC!**

## 5. LƯU ĐỒ (Đã có ở phần 5)

## 6. BIỂU MẪU (Đã liệt kê)

## 7. TIÊU CHUẨN (Đã liệt kê)

## 8. TRÁCH NHIỆM (Đã liệt kê)

## 9. LƯU Ý (Đã liệt kê)

## 10. PHỤ LỤC (Đã có)

## 11. FAQ

**Q1: Hồ sơ giấy có cần scan không?**  
A: NÊN scan để backup. Nhưng giấy gốc vẫn phải lưu (Một số hồ sơ pháp lý yêu cầu bản gốc).

**Q2: Nếu file bị hỏng, không mở được?**  
A: Rất nghiêm trọng! Khôi phục từ backup. Nếu không có backup → NC lớn.

**Q3: Có thể lưu hồ sơ trên Google Drive cá nhân không?**  
A: KHÔNG! Phải lưu server chính thức. Google Drive chỉ dùng để backup, không phải lưu trữ chính.

**Q4: Auditor yêu cầu xem hồ sơ 5 năm trước?**  
A: Nếu còn trong thời hạn lưu (VD: Hồ sơ 10 năm) → Phải cung cấp. Nếu đã thanh lý hợp lệ → Giải thích đã thanh lý.

---

**PHÊ DUYỆT**

| Trưởng Ban ISO | Trưởng IT | Phó Hiệu trưởng |
|---|---|---|
| [Họ tên] | [Họ tên] | [Họ tên] |
