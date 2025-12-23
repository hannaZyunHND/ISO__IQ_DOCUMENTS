# SOP-03.1: ĐÁNH GIÁ RỦI RO AN NINH MẠNG

## 1. MỤC ĐÍCH
Quy định quy trình đánh giá rủi ro an ninh mạng, đảm bảo:
- Nhận diện đầy đủ các mối đe dọa
- Đánh giá chính xác rủi ro
- Ưu tiên xử lý hợp lý
- Thông tin cho quyết định đầu tư
- Cập nhật liên tục

## 2. QUY TRÌNH ĐÁNH GIÁ

### 2.1. Asset inventory (Kiểm kê tài sản)

#### 2.1.1. Identify assets
```
IT Assets:
├─ Hardware:
│   ├─ Servers (physical, virtual)
│   ├─ Network devices (routers, switches)
│   ├─ End-user devices (PCs, laptops, tablets)
│   ├─ Mobile devices
│   └─ IoT devices (cameras, sensors)
│
├─ Software:
│   ├─ Operating systems
│   ├─ Applications (SIS, LMS, ERP)
│   ├─ Databases
│   └─ Development tools
│
├─ Data:
│   ├─ Student data
│   ├─ Staff data
│   ├─ Financial data
│   └─ Operational data
│
├─ Networks:
│   ├─ LAN
│   ├─ WiFi
│   ├─ WAN/Internet
│   └─ VPN
│
└─ Services:
    ├─ Cloud services
    ├─ Email
    ├─ Hosting
    └─ SaaS applications
```

#### 2.1.2. Asset classification
```
For each asset:
- Criticality: [Critical/High/Medium/Low]
- Value: [Financial, operational, reputational]
- Owner: [Department/person]
- Location: [Physical/virtual]
- Dependencies: [Other assets]
```

### 2.2. Threat identification

#### 2.2.1. Threat categories
```
External threats:
├─ Cybercriminals (ransomware, phishing, malware)
├─ Hackers (attacks, breaches)
├─ Competitors (espionage)
├─ Nation-states (APT)
└─ Script kiddies (vandalism)

Internal threats:
├─ Malicious insiders (sabotage, theft)
├─ Negligent employees (accidents, errors)
└─ Contractors (unauthorized access)

Environmental:
├─ Natural disasters (flood, fire)
├─ Power failures
├─ Equipment failures
└─ Pandemics (business continuity)
```

#### 2.2.2. Threat intelligence
```
Sources:
- Security vendors
- CERT/CSIRT advisories
- Industry reports
- News và forums
- Government warnings
- Peer schools

Activities:
- Monitor threat landscape
- Identify trends
- Assess applicability
- Update defenses
```

### 2.3. Vulnerability assessment

#### 2.3.1. Technical vulnerabilities
```
Assessment methods:
1. Automated scanning:
   - Vulnerability scanners (Nessus, Qualys)
   - Frequency: Weekly (internal), Monthly (external)
   - Scope: All systems

2. Manual testing:
   - Configuration reviews
   - Code reviews
   - Architecture reviews
   - Frequency: Quarterly

3. Penetration testing:
   - Simulated attacks
   - External testers
   - Frequency: Annual
```

#### 2.3.2. Non-technical vulnerabilities
```
Assess:
- Policy gaps
- Process weaknesses
- Training inadequacies
- Physical security
- Third-party risks
```

### 2.4. Risk analysis

#### 2.4.1. Risk calculation
```
Risk = Threat × Vulnerability × Impact

Components:
1. Threat likelihood (1-5):
   5 = Almost certain (>80%)
   4 = Likely (60-80%)
   3 = Possible (40-60%)
   2 = Unlikely (20-40%)
   1 = Rare (<20%)

2. Vulnerability exploitability (1-5):
   5 = Very easy (no skill needed)
   4 = Easy (basic skill)
   3 = Medium (moderate skill)
   2 = Hard (advanced skill)
   1 = Very hard (expert only)

3. Impact (1-5):
   5 = Catastrophic (>500M VNĐ, national news)
   4 = Major (100-500M, serious disruption)
   3 = Moderate (20-100M, significant impact)
   2 = Minor (5-20M, limited impact)
   1 = Negligible (<5M, minimal impact)

Risk Score = Likelihood × Impact (1-25)
```

#### 2.4.2. Risk matrix
```
Impact ↑
5 |  5  | 10  | 15  | 20  | 25  |
4 |  4  |  8  | 12  | 16  | 20  |
3 |  3  |  6  |  9  | 12  | 15  |
2 |  2  |  4  |  6  |  8  | 10  |
1 |  1  |  2  |  3  |  4  |  5  |
  +-----|-----|-----|-----|-----+
    1     2     3     4     5   → Likelihood

Risk levels:
🔴 20-25: Critical (immediate action)
🟠 15-19: High (urgent action)
🟡 10-14: Medium (planned action)
🟢 5-9: Low (accept or monitor)
🔵 1-4: Very low (accept)
```

### 2.5. Risk treatment

#### 2.5.1. Treatment options
```
For each risk:

Avoid (Tránh):
- Không thực hiện activity
- Eliminate vulnerability
- Example: Không cho BYOD

Reduce (Giảm):
- Implement controls
- Lower likelihood hoặc impact
- Example: Install firewall, train users

Transfer (Chuyển):
- Insurance
- Outsource
- Example: Cyber insurance

Accept (Chấp nhận):
- Acknowledge risk
- Monitor
- Example: Low-impact risks
```

#### 2.5.2. Treatment plan
```
Risk ID: [XXX]
Risk: [Description]
Current score: [XX]
Treatment: [Avoid/Reduce/Transfer/Accept]

Actions:
1. [Action 1] - [Owner] - [Deadline] - [Cost]
2. [Action 2] - [Owner] - [Deadline] - [Cost]

Target residual risk: [YY]
Review date: [Date]
```

## 6. RISK REGISTER

### 6.1. Cyber risk register template
```
RISK REGISTER - CYBER SECURITY

Risk ID | Threat | Vulnerability | Likelihood | Impact | Risk Score | Treatment | Status
--------|--------|---------------|------------|--------|------------|-----------|--------
CR001 | Ransomware | Unpatched systems | 4 | 5 | 20 | Reduce | Open
CR002 | Phishing | User awareness low | 4 | 4 | 16 | Reduce | In progress
CR003 | DDoS | No protection | 3 | 3 | 9 | Transfer | Planned
[...]
```

### 6.2. Maintenance
```
Updates:
- New risks: Add immediately
- Existing risks: Review quarterly
- Closed risks: Archive
- Trend analysis: Monthly
```

## 7. REPORTING

### 7.1. Risk reports
```
Monthly: Risk dashboard update
Quarterly: Risk review report
Annual: Comprehensive risk assessment
Ad-hoc: For incidents, Board requests
```

### 7.2. Risk dashboard
```
CYBER RISK DASHBOARD

Overall posture: [Score/100]
Trend: [↑ Improving / → Stable / ↓ Declining]

Risk distribution:
🔴 Critical: [X]
🟠 High: [Y]
🟡 Medium: [Z]
🟢 Low: [W]

Top risks:
1. [Risk name] - [Score] - [Status]
2. [Risk name] - [Score] - [Status]
3. [Risk name] - [Score] - [Status]

Recent changes:
- [Risk A]: ↑ Increased
- [Risk B]: ↓ Decreased
- [Risk C]: ✅ Closed

Actions needed: [X] open, [Y] overdue
```

## 8. CÔNG CỤ VÀ TEMPLATE

### 8.1. Assessment tools
```
- Vulnerability scanners (Nessus, OpenVAS)
- Asset discovery (Lansweeper, Spiceworks)
- Risk assessment software
- Threat intelligence platforms
```

### 8.2. Templates
```
- Asset inventory template
- Risk assessment template
- Risk register
- Treatment plan template
```

## 9. CHỈ SỐ ĐÁNH GIÁ

```
Coverage:
- Assets inventoried: 100%
- Risks assessed: 100%
- Assessments current: ≤ 90 days old

Quality:
- Critical risks identified: 100%
- Assessment accuracy: ≥ 90%
- Treatment plans: 100%

Effectiveness:
- Risks mitigated: ≥ 80%
- Residual risk: Acceptable
- Incidents from known risks: 0
```

---

**Ngày ban hành**: 01/01/2024  
**Người phê duyệt**: Ban Giám hiệu  
**Người soạn thảo**: Phòng IT Security  
**Ngày xem xét lại**: 01/01/2025






