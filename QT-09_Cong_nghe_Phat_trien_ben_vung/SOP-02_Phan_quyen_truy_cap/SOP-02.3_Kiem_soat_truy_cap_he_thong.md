# SOP-02.3: KIỂM SOÁT TRUY CẬP HỆ THỐNG

## 1. MỤC ĐÍCH
Quy định các biện pháp kiểm soát truy cập hệ thống, đảm bảo:
- Xác thực người dùng chính xác
- Phân quyền đúng vai trò
- Bảo vệ khỏi truy cập trái phép
- Giám sát hoạt động truy cập
- Phát hiện và ngăn chặn vi phạm

## 2. AUTHENTICATION (XÁC THỰC)

### 2.1. Authentication factors
```
Factor 1 - Something you know:
- Password
- PIN
- Security questions

Factor 2 - Something you have:
- Phone (SMS, app)
- Hardware token
- Smart card

Factor 3 - Something you are:
- Fingerprint
- Face recognition
- Iris scan
```

### 2.2. Multi-Factor Authentication (MFA)

#### 2.2.1. MFA requirements
```
Mandatory MFA for:
✅ Admin accounts (all systems)
✅ Remote access (VPN)
✅ Financial systems
✅ HR systems
✅ Email (executives)
✅ Cloud services admin

Optional MFA for:
⚠️ Standard email
⚠️ LMS/SIS (teachers)
⚠️ Student accounts

Not required:
❌ Student portal (low risk)
❌ Public website
```

#### 2.2.2. MFA methods
```
Preferred order:
1. Authenticator app (Google, Microsoft)
2. SMS OTP
3. Email OTP
4. Hardware token

Setup process:
1. User enables MFA
2. Register device/method
3. Backup codes generated
4. Test authentication
5. Enforce on next login
```

### 2.3. Single Sign-On (SSO)

#### 2.3.1. Benefits
```
For users:
- One login cho multiple systems
- Fewer passwords to remember
- Faster access

For IT:
- Centralized management
- Better security
- Easier auditing
- Reduced help desk calls
```

#### 2.3.2. Implementation
```
Architecture:
[Identity Provider (IdP)]
    ↓ SAML/OAuth
[Applications]
├─ SIS
├─ LMS
├─ Email
├─ File storage
└─ Other apps

IdP options:
- Azure AD
- Google Workspace
- Okta
- On-premise (AD FS)
```

## 3. AUTHORIZATION (PHÂN QUYỀN)

### 3.1. Access control models

#### 3.1.1. Role-Based Access Control (RBAC)
```
Concept: Permissions gán cho roles, users gán vào roles

Structure:
User → Role → Permissions → Resources

Example:
Nguyen Van A → Teacher → Read/Write → Own classes
```

#### 3.1.2. Attribute-Based Access Control (ABAC)
```
Concept: Permissions based on attributes

Attributes:
- User: Department, level, location
- Resource: Classification, owner
- Environment: Time, location, device
- Action: Read, write, delete

Rule example:
IF user.department = "Finance" 
AND resource.type = "Financial" 
AND time.hour BETWEEN 8 AND 18
THEN allow access
```

### 3.2. Permission levels
```
Level | Description | Examples
------|-------------|----------
None | No access | -
Read | View only | Reports, dashboards
Write | Create/edit | Data entry, updates
Delete | Remove | Admin functions
Admin | Full control | System configuration
```

### 3.3. Data-level security

#### 3.3.1. Row-level security
```
Concept: Users chỉ thấy rows họ có quyền

Examples:
- Teachers: Chỉ own classes
- Managers: Chỉ own department
- Finance: Chỉ assigned accounts
```

#### 3.3.2. Column-level security
```
Concept: Hide sensitive columns

Examples:
- Salary: Chỉ HR và individual
- Health info: Chỉ nurse và parents
- Grades: Chỉ teachers và students
```

#### 3.3.3. Dynamic data masking
```
Concept: Mask data based on user role

Examples:
- Phone: 098****789 (for non-authorized)
- Email: n***@gmail.com
- ID number: ****5678
```

## 4. SESSION MANAGEMENT

### 4.1. Session controls
```
Settings:
- Timeout: 30 phút idle (standard)
- Timeout: 15 phút (sensitive systems)
- Max duration: 8 giờ
- Concurrent sessions: 2 (warning), 3 (block)
- Device binding: Optional
```

### 4.2. Logout procedures
```
Automatic logout:
- After timeout
- After max duration
- On suspicious activity

Manual logout:
- User clicks logout
- Clear session
- Redirect to login
```

## 5. REMOTE ACCESS

### 5.1. VPN access

#### 5.1.1. Requirements
```
Who needs:
- Staff working from home
- Admins for after-hours support
- Contractors (temporary)

Requirements:
- Approved request
- Company device (preferred)
- MFA enabled
- VPN client installed
- Security training completed
```

#### 5.1.2. VPN policy
```
Allowed:
✅ Work-related activities only
✅ Approved applications
✅ Secure networks

Not allowed:
❌ Personal use
❌ Torrenting, streaming
❌ Public WiFi (without additional security)
❌ Sharing credentials
```

### 5.2. Remote desktop

#### 5.2.1. Access controls
```
- Restricted to IT staff và approved users
- MFA required
- Session recording (for admin)
- Timeout: 15 phút
- Approval for each session (high-privilege)
```

## 6. PRIVILEGED ACCESS MANAGEMENT

### 6.1. Admin accounts

#### 6.1.1. Separation
```
Principle: Admin accounts tách biệt personal accounts

Structure:
- Personal: nguyen.van.a@school.edu.vn
- Admin: nguyen.van.a-admin@school.edu.vn

Usage:
- Personal: Email, daily work
- Admin: System administration only
```

#### 6.1.2. Just-in-Time (JIT) access
```
Concept: Cấp admin access chỉ khi cần, limited time

Process:
1. Request admin access
2. Justify need
3. Approve (CIO)
4. Grant for X hours
5. Auto-revoke after time
6. Audit usage
```

### 6.2. Privileged Session Management
```
Controls:
- Session recording
- Real-time monitoring
- Approval workflow
- Time limits
- Activity logging
```

## 7. CÔNG CỤ VÀ TEMPLATE

### 7.1. Technical tools
```
- Identity Provider (Azure AD, Okta)
- MFA solution
- VPN (Cisco, Fortinet)
- Privileged Access Management (CyberArk, BeyondTrust)
- Session monitoring
```

### 7.2. Templates
```
- Access control policy
- Remote access policy
- VPN request form
- Admin access request
```

## 8. CHỈ SỐ ĐÁNH GIÁ

```
Authentication:
- MFA adoption (required accounts): 100%
- Password policy compliance: 100%
- SSO coverage: ≥ 80% of applications

Authorization:
- Role assignments correct: ≥ 98%
- Excessive permissions: 0
- Separation of duties violations: 0

Remote access:
- VPN usage: Monitored 100%
- Unauthorized access: 0
- Security incidents: ≤ 2/năm

Privileged access:
- Admin account separation: 100%
- JIT usage: ≥ 80%
- Session recordings: 100%
```

---

**Ngày ban hành**: 01/01/2024  
**Người phê duyệt**: Ban Giám hiệu  
**Người soạn thảo**: Phòng IT  
**Ngày xem xét lại**: 01/01/2025






