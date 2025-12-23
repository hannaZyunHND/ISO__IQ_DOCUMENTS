# BM-379: Form đăng ký tư vấn (Online)

**Mã biểu mẫu:** QT-07-SOP-01-BM-379  
**Phiên bản:** 1.0  
**Ngày ban hành:** 01/01/2024  
**Ngày hiệu lực:** 01/01/2024  

## 1. THÔNG TIN CHUNG

| **Thuộc tính** | **Nội dung** |
|---|---|
| Tên biểu mẫu | Form đăng ký tư vấn (Online) |
| Mục đích | Thu thập thông tin PH quan tâm tuyển sinh |
| Đối tượng sử dụng | PH, Tư vấn viên |
| Tần suất sử dụng | Liên tục (Tháng 3-8) |

## 2. NỘI DUNG BIỂU MẪU

### 2.1. Form Facebook Ads

```
┌─────────────────────────────────────┐
│  ĐĂNG KÝ TƯ VẤN TUYỂN SINH          │
├─────────────────────────────────────┤
│ Họ tên PH: [____________]           │
│ SĐT: [____________]                 │
│ Email: [____________]               │
│ Con học lớp: [Chọn: MN/1/2...]      │
│ Khu vực: [Chọn: Quận X/Y...]        │
│                                     │
│ [Nút: GỬI ĐĂNG KÝ]                  │
└─────────────────────────────────────┘
```

### 2.2. Form Website (Chi tiết hơn)

| **Trường** | **Loại** | **Bắt buộc** | **Ghi chú** |
|---|---|---|---|
| Họ tên PH | Text | ✅ | |
| SĐT | Phone | ✅ | |
| Email | Email | ✅ | |
| Con tên | Text | ✅ | |
| Con năm nay lên lớp | Select | ✅ | MN, 1, 2, 3, 4, 5, 6, 7, 8, 9 |
| Khu vực | Select | ✅ | Quận X, Y, Z... |
| Nguồn biết đến | Select | ❌ | Facebook, Google, Bạn bè, Khác |
| Mong muốn | Textarea | ❌ | PH quan tâm điểm gì? |
| Thời gian liên hệ | Select | ❌ | Sáng, Chiều, Tối |

### 2.3. Form Landing Page

```html
<!DOCTYPE html>
<html>
<head>
    <title>Đăng ký tư vấn tuyển sinh - IQ School</title>
</head>
<body>
    <div class="form-container">
        <h2>🎓 ĐĂNG KÝ TƯ VẤN TUYỂN SINH</h2>
        <p>Nhận tư vấn MIỄN PHÍ về chương trình học!</p>
        
        <form action="/submit" method="POST">
            <div class="form-group">
                <label>Họ tên PH *</label>
                <input type="text" name="parent_name" required>
            </div>
            
            <div class="form-group">
                <label>Số điện thoại *</label>
                <input type="tel" name="phone" required>
            </div>
            
            <div class="form-group">
                <label>Email *</label>
                <input type="email" name="email" required>
            </div>
            
            <div class="form-group">
                <label>Tên con *</label>
                <input type="text" name="child_name" required>
            </div>
            
            <div class="form-group">
                <label>Con năm nay lên lớp *</label>
                <select name="grade" required>
                    <option value="">Chọn lớp</option>
                    <option value="MN">Mầm non</option>
                    <option value="1">Lớp 1</option>
                    <option value="2">Lớp 2</option>
                    <option value="3">Lớp 3</option>
                    <option value="4">Lớp 4</option>
                    <option value="5">Lớp 5</option>
                    <option value="6">Lớp 6</option>
                    <option value="7">Lớp 7</option>
                    <option value="8">Lớp 8</option>
                    <option value="9">Lớp 9</option>
                </select>
            </div>
            
            <div class="form-group">
                <label>Khu vực *</label>
                <select name="area" required>
                    <option value="">Chọn quận/huyện</option>
                    <option value="quan-x">Quận X</option>
                    <option value="quan-y">Quận Y</option>
                    <option value="quan-z">Quận Z</option>
                    <option value="khac">Khác</option>
                </select>
            </div>
            
            <div class="form-group">
                <label>Nguồn biết đến</label>
                <select name="source">
                    <option value="">Chọn nguồn</option>
                    <option value="facebook">Facebook</option>
                    <option value="google">Google</option>
                    <option value="ban-be">Bạn bè giới thiệu</option>
                    <option value="poster">Poster/Banner</option>
                    <option value="bao-chi">Báo chí</option>
                    <option value="khac">Khác</option>
                </select>
            </div>
            
            <div class="form-group">
                <label>Mong muốn của PH</label>
                <textarea name="expectation" placeholder="PH quan tâm điểm gì? (Chất lượng, Học phí, Cơ sở...)" rows="3"></textarea>
            </div>
            
            <div class="form-group">
                <label>Thời gian thuận tiện liên hệ</label>
                <select name="contact_time">
                    <option value="">Chọn thời gian</option>
                    <option value="sang">Sáng (8h-12h)</option>
                    <option value="chieu">Chiều (13h-17h)</option>
                    <option value="toi">Tối (18h-20h)</option>
                    <option value="linh-hoat">Linh hoạt</option>
                </select>
            </div>
            
            <div class="form-group checkbox">
                <input type="checkbox" name="agree" required>
                <label>Tôi đồng ý nhận thông tin tư vấn từ IQ School</label>
            </div>
            
            <button type="submit" class="btn-submit">
                🎯 ĐĂNG KÝ TƯ VẤN MIỄN PHÍ
            </button>
        </form>
        
        <div class="benefits">
            <h3>🎁 ƯU ĐÃI ĐẶC BIỆT:</h3>
            <ul>
                <li>✅ Giảm 10% học phí (Đăng ký trước 31/3)</li>
                <li>✅ Tặng Balo + Đồ dùng (Trị giá 500K)</li>
                <li>✅ Tư vấn MIỄN PHÍ 1-1</li>
                <li>✅ Tham quan trường MIỄN PHÍ</li>
            </ul>
        </div>
    </div>
</body>
</html>
```

### 2.4. Validation Rules

| **Trường** | **Rule** | **Thông báo lỗi** |
|---|---|---|
| Họ tên PH | Min 2 ký tự, Max 50 ký tự | "Vui lòng nhập họ tên (2-50 ký tự)" |
| SĐT | 10-11 số, bắt đầu bằng 0 | "Vui lòng nhập SĐT hợp lệ" |
| Email | Format email hợp lệ | "Vui lòng nhập email hợp lệ" |
| Tên con | Min 2 ký tự, Max 30 ký tự | "Vui lòng nhập tên con (2-30 ký tự)" |
| Lớp | Bắt buộc chọn | "Vui lòng chọn lớp" |
| Khu vực | Bắt buộc chọn | "Vui lòng chọn khu vực" |
| Đồng ý | Bắt buộc tick | "Vui lòng đồng ý nhận thông tin" |

### 2.5. Auto Response

#### A. SMS (Ngay sau khi submit)
```
"Chào quý PH,
Cảm ơn quý vị đã đăng ký tư vấn IQ School!
Chúng tôi sẽ liên hệ trong 24h.
Hotline: 1900-xxxx
IQ School"
```

#### B. Email (Ngay sau khi submit)
```
Subject: Cảm ơn quý vị đã quan tâm IQ School!

Kính gửi quý PH [Tên],

Cảm ơn quý vị đã đăng ký tư vấn tuyển sinh!

Chúng tôi sẽ liên hệ quý vị trong 24h để:
• Tư vấn chi tiết về chương trình học
• Hẹn lịch tham quan trường
• Giải đáp mọi thắc mắc

Thông tin đã nhận:
• Con: [Tên con] - Lớp [X]
• Khu vực: [Quận X]
• Mong muốn: [Nội dung]

Mọi thắc mắc: 1900-xxxx

Trân trọng,
Ban Tuyển sinh - IQ School
```

## 3. PHÊ DUYỆT

| **Vị trí** | **Họ tên** | **Chữ ký** | **Ngày** |
|---|---|---|---|
| IT | | | |
| BP Tuyển sinh | | | |

---
*Biểu mẫu này được sử dụng trong SOP-01.3: Tiếp nhận và xử lý hồ sơ tuyển sinh*
