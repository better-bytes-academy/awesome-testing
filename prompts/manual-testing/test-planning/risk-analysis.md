# Các Prompt Về Phân Tích Rủi Ro (Risk Analysis Prompts)

## 1. Đánh Giá Rủi Ro Dự Án (Project Risk Assessment)

```text
Thực hiện phân tích rủi ro toàn diện cho:

Dự án: [TÊN_DỰ_ÁN]
Loại dự án: [WEB/MOBILE/API/v.v.]
Thời gian: [THỜI_LƯỢNG]
Kinh nghiệm của đội ngũ: [MÔ_TẢ_KINH_NGHIỆM]
Công nghệ sử dụng (Tech Stack): [LIỆT_KÊ_CÔNG_NGHỆ]
Độ phức tạp: [CAO/TRUNG_BÌNH/THẤP]

Nhận diện và phân tích:
- Rủi ro kỹ thuật (Technical risks)
- Rủi ro nguồn lực (Resource risks)
- Rủi ro tiến độ (Schedule risks)
- Rủi ro chất lượng (Quality risks)
- Rủi ro kinh doanh (Business risks)
- Chiến lược giảm thiểu cho từng rủi ro
- Ma trận ưu tiên rủi ro
```

## 2. Phân Tích Rủi Ro Của Tính Năng (Feature Risk Analysis)

```text
Phân tích rủi ro cho một tính năng cụ thể:

Tính năng: [TÊN_TÍNH_NĂNG]
Độ phức tạp: [CAO/TRUNG_BÌNH/THẤP]
Sự phụ thuộc (Dependencies): [LIỆT_KÊ_SỰ_PHỤ_THUỘC]
Sử dụng công nghệ mới: [CÓ/KHÔNG]
Tác động đến người dùng: [NGHIÊM_TRỌNG/CAO/TRUNG_BÌNH/THẤP]
Tiến độ: [CHẶT_CHẼ/ĐẦY_ĐỦ/LINH_HOẠT]

Đánh giá:
- Rủi ro trong quá trình triển khai kỹ thuật
- Rủi ro tích hợp
- Rủi ro hiệu năng
- Rủi ro bảo mật
- Rủi ro trong việc tiếp nhận từ người dùng (User adoption)
- Đề xuất về độ bao phủ kiểm thử
```

## 3. Đánh Giá Rủi Ro Phát Hành (Release Risk Assessment)

```text
Thực hiện phân tích rủi ro phát hành cho:

Phiên bản phát hành: [PHIÊN_BẢN]
Ngày phát hành: [NGÀY_THÁNG]
Các thay đổi đi kèm: [MAJOR(LỚN)/MINOR(NHỎ)/PATCH(BẢN_VÁ)]
Độ bao phủ kiểm thử: [PHẦN_TRĂM]
Các lỗi đã biết (Known Issues): [SỐ_LƯỢNG_VÀ_MỨC_ĐỘ_NGHIÊM_TRỌNG]
Hình thức triển khai: [PHASED(TỪNG_GIAI_ĐOẠN)/BIG_BANG(ĐỒNG_LOẠT)]

Đánh giá:
- Rủi ro triển khai (Deployment risks)
- Rủi ro hồi quy (Regression risks)
- Rủi ro suy giảm hiệu năng
- Các lỗ hổng bảo mật
- Độ phức tạp khi khôi phục (Rollback)
- Tác động đến người dùng
- Đề xuất Quyết định Tiếp tục/Dừng (Go/No-Go recommendation)
```

## 4. Phân Tích Rủi Ro Kỹ Thuật (Technical Risk Analysis)

```text
Phân tích rủi ro kỹ thuật cho:

Công nghệ: [TÊN_CÔNG_NGHỆ]
Mức độ quen thuộc của đội ngũ: [CAO/TRUNG_BÌNH/THẤP]
Độ trưởng thành của công nghệ: [ỔN_ĐỊNH/MỚI_NỔI/THỬ_NGHIỆM]
Độ phức tạp khi tích hợp: [MÔ_TẢ]
Yêu cầu hiệu năng: [CÁC_YÊU_CẦU]

Nhận diện:
- Rủi ro áp dụng công nghệ mới
- Rủi ro khả năng mở rộng (Scalability)
- Rủi ro về tính tương thích
- Rủi ro bảo trì
- Rủi ro từ nhà cung cấp/hỗ trợ
- Rủi ro chuyển đổi/di dời (Migration)
- Các chiến lược giảm thiểu
```

## 5. Phân Tích Rủi Ro Tích Hợp (Integration Risk Analysis)

```text
Đánh giá rủi ro tích hợp cho:

Hệ thống: [HỆ_THỐNG_A] <-> [HỆ_THỐNG_B]
Loại hình tích hợp: [API/CƠ_SỞ_DỮ_LIỆU/FILE/TIN_NHẮN]
Khối lượng dữ liệu: [KHỐI_LƯỢNG]
Tần suất: [THỜI_GIAN_THỰC/BATCH/v.v.]
Sự phụ thuộc: [MÔ_TẢ_SỰ_PHỤ_THUỘC]

Phân tích:
- Lỗi tại các điểm tích hợp
- Rủi ro đồng bộ dữ liệu
- Nút thắt cổ chai về hiệu năng (Performance bottlenecks)
- Các lỗ hổng bảo mật
- Tính tương thích của phiên bản
- Lỗ hổng trong việc xử lý lỗi (Error handling)
- Nhu cầu về giám sát và cảnh báo
```

## 6. Phân Tích Rủi Ro Dữ Liệu (Data Risk Analysis)

```text
Thực hiện phân tích rủi ro dữ liệu cho:

Các loại dữ liệu: [LIỆT_KÊ_LOẠI_DỮ_LIỆU]
Khối lượng dữ liệu: [KÍCH_THƯỚC]
Độ nhạy cảm của dữ liệu: [CÔNG_KHAI/NỘI_BỘ/TUYỆT_MẬT]
Nguồn dữ liệu: [LIỆT_KÊ_NGUỒN]
Chất lượng dữ liệu: [TRẠNG_THÁI_HIỆN_TẠI]

Đánh giá:
- Rủi ro mất mát dữ liệu
- Rủi ro hỏng/lỗi dữ liệu (Data corruption)
- Rủi ro quyền riêng tư dữ liệu
- Rủi ro di chuyển dữ liệu (Data migration)
- Rủi ro chất lượng dữ liệu
- Rủi ro về sự tuân thủ
- Chiến lược sao lưu và phục hồi (Backup & Recovery)
```

## 7. Phân Tích Rủi Ro Hiệu Năng (Performance Risk Analysis)

```text
Phân tích rủi ro hiệu năng cho:

Ứng dụng: [TÊN_ỨNG_DỤNG]
Tải dự kiến: [SỐ_USER_ĐỒNG_THỜI/TPS]
Yêu cầu hiệu năng: [SLA]
Hiệu năng hiện tại: [MỨC_CƠ_SỞ(BASELINE)]
Nhu cầu mở rộng: [DỰ_BÁO_TĂNG_TRƯỞNG]

Nhận diện:
- Rủi ro nút thắt cổ chai hiệu năng
- Rủi ro khả năng mở rộng
- Rủi ro giới hạn tài nguyên
- Rủi ro phụ thuộc vào bên thứ ba
- Rủi ro khi xử lý tải đỉnh điểm (Peak load)
- Rủi ro suy giảm hiệu năng
- Nhu cầu giám sát và tối ưu hóa
```

## 8. Phân Tích Rủi Ro Bảo Mật (Security Risk Analysis)

```text
Thực hiện đánh giá rủi ro bảo mật cho:

Ứng dụng: [TÊN_ỨNG_DỤNG]
Độ nhạy cảm của dữ liệu: [MỨC_ĐỘ]
Cơ sở người dùng: [NỘI_BỘ/BÊN_NGOÀI/CẢ_HAI]
Yêu cầu tuân thủ: [CÁC_TIÊU_CHUẨN]
Các vấn đề bảo mật trước đây: [NẾU_CÓ]

Phân tích:
- Rủi ro xác thực/phân quyền (Authentication/authorization)
- Rủi ro rò rỉ dữ liệu (Data breach)
- Rủi ro tấn công tiêm nhiễm (Injection attacks)
- Rủi ro kiểm soát truy cập
- Rủi ro về mã hóa
- Rủi ro từ các thành phần bên thứ ba
- Đề xuất kiểm thử bảo mật
```

## 9. Phân Tích Rủi Ro Nguồn Lực (Resource Risk Analysis)

```text
Đánh giá các rủi ro liên quan đến nguồn lực cho:

Dự án: [TÊN_DỰ_ÁN]
Quy mô đội ngũ: [SỐ_LƯỢNG]
Nhân sự chủ chốt: [CÁC_VAI_TRÒ]
Thời gian: [THỜI_LƯỢNG]
Ngân sách: [CÁC_RÀNG_BUỘC]

Nhận diện:
- Rủi ro về sự sẵn sàng của đội ngũ
- Rủi ro thiếu hụt kỹ năng (Skill gap)
- Rủi ro phụ thuộc vào nhân sự chủ chốt
- Rủi ro vượt ngân sách
- Rủi ro về công cụ/cơ sở hạ tầng
- Nhu cầu đào tạo
- Lập kế hoạch dự phòng
```

## 10. Phân Tích Rủi Ro Tiến Độ (Schedule Risk Analysis)

```text
Phân tích rủi ro tiến độ cho:

Dự án: [TÊN_DỰ_ÁN]
Hạn chót (Deadline): [NGÀY_THÁNG]
Tiến độ hiện tại: [PHẦN_TRĂM]
Sự phụ thuộc: [CÁC_PHỤ_THUỘC_BÊN_NGOÀI]
Thời gian dự trữ (Buffer Time): [THỜI_GIAN_DỰ_TRỮ_HIỆN_CÓ]

Đánh giá:
- Rủi ro trễ hạn (Deadline miss)
- Rủi ro chậm trễ do sự phụ thuộc
- Rủi ro phình to phạm vi (Scope creep)
- Rủi ro về mức độ sẵn sàng của nguồn lực
- Rủi ro bị ép/rút ngắn thời gian kiểm thử
- Rủi ro phải đánh đổi chất lượng
- Các giải pháp khôi phục tiến độ
```

## 11. Phân Tích Rủi Ro Bên Thứ Ba (Third-Party Risk Analysis)

```text
Đánh giá rủi ro tích hợp với bên thứ ba cho:

Dịch vụ bên thứ ba: [TÊN_DỊCH_VỤ]
Mức độ phụ thuộc: [NGHIÊM_TRỌNG/CAO/TRUNG_BÌNH/THẤP]
SLA (Cam kết chất lượng dịch vụ): [NỘI_DUNG_SLA]
Giải pháp thay thế sẵn có: [CÓ/KHÔNG]
Điều khoản hợp đồng: [MÔ_TẢ]

Phân tích:
- Rủi ro về mức độ sẵn sàng của dịch vụ
- Rủi ro suy giảm hiệu năng
- Rủi ro khi có thay đổi từ API
- Rủi ro bị trói buộc với một nhà cung cấp (Vendor lock-in)
- Rủi ro leo thang chi phí
- Rủi ro bảo mật dữ liệu
- Lập kế hoạch dự phòng
```

## 12. Phân Tích Rủi Ro Tuân Thủ (Compliance Risk Analysis)

```text
Đánh giá rủi ro tuân thủ cho:

Ứng dụng: [TÊN_ỨNG_DỤNG]
Quy định: [GDPR/HIPAA/PCI-DSS/v.v.]
Dữ liệu được xử lý: [CÁC_LOẠI_DỮ_LIỆU]
Phạm vi địa lý: [CÁC_KHU_VỰC]
Yêu cầu đánh giá/kiểm toán (Audit): [TẦN_SUẤT]

Nhận diện:
- Khoảng trống trong việc tuân thủ quy định
- Rủi ro về quyền riêng tư dữ liệu
- Rủi ro thất bại khi đánh giá/kiểm toán
- Rủi ro trách nhiệm pháp lý
- Thiếu sót về mặt tài liệu
- Rủi ro về tính tuân thủ quy trình
- Thứ tự ưu tiên để khắc phục
```

---

## Mẫu Phân Tích Rủi Ro (Risk Analysis Template)

```text
# Phân Tích Rủi Ro cho [TÊN_DỰ_ÁN/TÍNH_NĂNG]

## Nhận Diện Rủi Ro

| Mã Rủi Ro | Mô Tả Rủi Ro | Danh Mục | Xác Suất | Tác Động | Điểm Rủi Ro |
|-----------|--------------|----------|----------|----------|-------------|
| R001 | [MÔ_TẢ] | [KỸ_THUẬT/NGUỒN_LỰC/v.v.] | [CAO/TB/THẤP] | [CAO/TB/THẤP] | [ĐIỂM_SỐ] |
| R002 | [MÔ_TẢ] | [DANH_MỤC] | [CAO/TB/THẤP] | [CAO/TB/THẤP] | [ĐIỂM_SỐ] |

## Ma Trận Ưu Tiên Rủi Ro

         Tác động (Impact)
         Cao  | R001, R003 | R002, R005 |
Xác suất TB   | R004       | R006       |
         Thấp | R007       | R008       |
              |------------|------------|
                Cao          Trung bình   Thấp

http://googleusercontent.com/immersive_entry_chip/0

## Hướng Dẫn Tính Điểm Rủi Ro (Risk Scoring Guide)

### Xác Suất (Likelihood)
- **Cao (3)**: Rất có khả năng xảy ra (xác suất >60%)
- **Trung bình (2)**: Có thể xảy ra (xác suất 30-60%)
- **Thấp (1)**: Không chắc sẽ xảy ra (xác suất <30%)

### Tác Động (Impact)
- **Cao (3)**: Tác động nghiêm trọng đến sự thành công của dự án
- **Trung bình (2)**: Tác động vừa phải, có thể kiểm soát được
- **Thấp (1)**: Tác động nhỏ, dễ dàng xử lý

### Điểm Rủi Ro (Risk Score)
- **Điểm Rủi Ro = Xác Suất × Tác Động**
- **Rủi Ro Cao**: Điểm 6-9 (Cần hành động ngay lập tức)
- **Rủi Ro Trung Bình**: Điểm 3-4 (Lên kế hoạch giảm thiểu)
- **Rủi Ro Thấp**: Điểm 1-2 (Theo dõi/Giám sát)

## Các Phương Pháp Thực Hành Tốt Nhất (Best Practices)

1. **Nhận diện sớm**: Phát hiện các rủi ro càng sớm càng tốt.
2. **Giám sát liên tục**: Thường xuyên xem xét và cập nhật trạng thái rủi ro.
3. **Sự tham gia của các bên liên quan**: Nhận ý kiến đóng góp từ tất cả các bên liên quan.
4. **Giảm thiểu chủ động**: Đừng đợi đến khi rủi ro xảy ra mới hành động.
5. **Ghi chép mọi thứ**: Lưu giữ nhật ký rủi ro (Risk Logs) một cách chi tiết.
6. **Học hỏi từ quá khứ**: Xem xét lại rủi ro từ các dự án trước đây.
7. **Định lượng khi có thể**: Sử dụng số liệu/dữ liệu để hỗ trợ đánh giá.
8. **Cân bằng giữa Rủi ro và Lợi ích**: Xem xét các giá trị mang lại cho doanh nghiệp.

## Các Chiến Lược Giảm Thiểu Rủi Ro (Risk Mitigation Strategies)

### Tránh né (Avoidance)
- Thay đổi phương pháp tiếp cận để loại bỏ hoàn toàn rủi ro.
- Loại bỏ các tính năng hoặc các thành phần phụ thuộc có rủi ro cao.

### Giảm thiểu (Reduction)
- Áp dụng các biện pháp kiểm soát để giảm xác suất hoặc tác động.
- Bổ sung thêm các bước kiểm thử, đánh giá (review) hoặc xác thực (validation).

### Chuyển giao (Transfer)
- Thuê ngoài (Outsource) các thành phần có rủi ro cao.
- Sử dụng bảo hiểm hoặc các điều khoản bảo hành.

### Chấp nhận (Acceptance)
- Nhận biết rủi ro và chuẩn bị phương án dự phòng.
- Theo dõi chặt chẽ và luôn sẵn sàng với kế hoạch ứng phó.

## Danh Sách Kiểm Tra Các Danh Mục Rủi Ro Phổ Biến (Common Risk Categories Checklist)

- [ ] Rủi ro Kỹ thuật/Công nghệ (Technical/Technology risks)
- [ ] Rủi ro Tích hợp (Integration risks)
- [ ] Rủi ro Hiệu năng (Performance risks)
- [ ] Rủi ro Bảo mật (Security risks)
- [ ] Rủi ro Dữ liệu (Data risks)
- [ ] Rủi ro Nguồn lực/Nhân sự (Resource/Staffing risks)
- [ ] Rủi ro Tiến độ/Lịch trình (Schedule/Timeline risks)
- [ ] Rủi ro Ngân sách/Chi phí (Budget/Cost risks)
- [ ] Rủi ro từ Bên thứ ba/Nhà cung cấp (Third-party/Vendor risks)
- [ ] Rủi ro về Tuân thủ/Pháp lý (Compliance/Regulatory risks)
- [ ] Rủi ro Chất lượng (Quality risks)
- [ ] Rủi ro Kinh doanh/Thị trường (Business/Market risks)

---
# Risk Analysis Prompts

## 1. Project Risk Assessment

```
Perform a comprehensive risk analysis for:

Project: [PROJECT_NAME]
Project Type: [WEB/MOBILE/API/etc.]
Timeline: [DURATION]
Team Experience: [DESCRIBE_EXPERIENCE]
Technology Stack: [LIST_TECHNOLOGIES]
Complexity: [HIGH/MEDIUM/LOW]

Identify and analyze:
- Technical risks
- Resource risks
- Schedule risks
- Quality risks
- Business risks
- Mitigation strategies for each
- Risk prioritization matrix
```

## 2. Feature Risk Analysis

```
Analyze risks for a specific feature:

Feature: [FEATURE_NAME]
Complexity: [HIGH/MEDIUM/LOW]
Dependencies: [LIST_DEPENDENCIES]
New Technology: [YES/NO]
User Impact: [CRITICAL/HIGH/MEDIUM/LOW]
Timeline: [TIGHT/ADEQUATE/FLEXIBLE]

Assess:
- Technical implementation risks
- Integration risks
- Performance risks
- Security risks
- User adoption risks
- Testing coverage recommendations
```

## 3. Release Risk Assessment

```
Perform a release risk analysis for:

Release Version: [VERSION]
Release Date: [DATE]
Changes Included: [MAJOR/MINOR/PATCH]
Testing Coverage: [PERCENTAGE]
Known Issues: [NUMBER_AND_SEVERITY]
Deployment Type: [PHASED/BIG_BANG]

Evaluate:
- Deployment risks
- Regression risks
- Performance degradation risks
- Security vulnerabilities
- Rollback complexity
- User impact
- Go/No-Go recommendation
```

## 4. Technical Risk Analysis

```
Analyze technical risks for:

Technology: [TECHNOLOGY_NAME]
Team Familiarity: [HIGH/MEDIUM/LOW]
Maturity: [STABLE/EMERGING/EXPERIMENTAL]
Integration Complexity: [DESCRIBE]
Performance Requirements: [REQUIREMENTS]

Identify:
- Technology adoption risks
- Scalability risks
- Compatibility risks
- Maintenance risks
- Vendor/support risks
- Migration risks
- Mitigation strategies
```

## 5. Integration Risk Analysis

```
Assess integration risks for:

Systems: [SYSTEM_A] <-> [SYSTEM_B]
Integration Type: [API/DATABASE/FILE/MESSAGE]
Data Volume: [VOLUME]
Frequency: [REAL_TIME/BATCH/etc.]
Dependencies: [DESCRIBE_DEPENDENCIES]

Analyze:
- Integration point failures
- Data synchronization risks
- Performance bottlenecks
- Security vulnerabilities
- Version compatibility
- Error handling gaps
- Monitoring and alerting needs
```

## 6. Data Risk Analysis

```
Perform a data risk analysis for:

Data Types: [LIST_DATA_TYPES]
Data Volume: [SIZE]
Data Sensitivity: [PUBLIC/INTERNAL/CONFIDENTIAL]
Data Sources: [LIST_SOURCES]
Data Quality: [CURRENT_STATE]

Assess:
- Data loss risks
- Data corruption risks
- Data privacy risks
- Data migration risks
- Data quality risks
- Compliance risks
- Backup and recovery strategy
```

## 7. Performance Risk Analysis

```
Analyze performance risks for:

Application: [APP_NAME]
Expected Load: [USERS/TPS]
Performance Requirements: [SLA]
Current Performance: [BASELINE]
Scalability Needs: [GROWTH_PROJECTION]

Identify:
- Performance bottleneck risks
- Scalability risks
- Resource constraint risks
- Third-party dependency risks
- Peak load handling risks
- Performance degradation risks
- Monitoring and optimization needs
```

## 8. Security Risk Analysis

```
Perform a security risk assessment for:

Application: [APP_NAME]
Data Sensitivity: [LEVEL]
User Base: [INTERNAL/EXTERNAL/BOTH]
Compliance Requirements: [STANDARDS]
Previous Security Issues: [IF_ANY]

Analyze:
- Authentication/authorization risks
- Data breach risks
- Injection attack risks
- Access control risks
- Encryption risks
- Third-party component risks
- Security testing recommendations
```

## 9. Resource Risk Analysis

```
Assess resource-related risks for:

Project: [PROJECT_NAME]
Team Size: [NUMBER]
Key Personnel: [ROLES]
Timeline: [DURATION]
Budget: [CONSTRAINTS]

Identify:
- Team availability risks
- Skill gap risks
- Key person dependency risks
- Budget overrun risks
- Tool/infrastructure risks
- Training needs
- Contingency planning
```

## 10. Schedule Risk Analysis

```
Analyze schedule risks for:

Project: [PROJECT_NAME]
Deadline: [DATE]
Current Progress: [PERCENTAGE]
Dependencies: [EXTERNAL_DEPENDENCIES]
Buffer Time: [AVAILABLE_BUFFER]

Assess:
- Deadline miss risks
- Dependency delay risks
- Scope creep risks
- Resource availability risks
- Testing time compression risks
- Quality compromise risks
- Schedule recovery options
```

## 11. Third-Party Risk Analysis

```
Evaluate third-party integration risks for:

Third-Party Service: [SERVICE_NAME]
Dependency Level: [CRITICAL/HIGH/MEDIUM/LOW]
SLA: [SERVICE_LEVEL_AGREEMENT]
Alternatives Available: [YES/NO]
Contract Terms: [DESCRIBE]

Analyze:
- Service availability risks
- Performance degradation risks
- API changes risks
- Vendor lock-in risks
- Cost escalation risks
- Data security risks
- Contingency planning
```

## 12. Compliance Risk Analysis

```
Assess compliance risks for:

Application: [APP_NAME]
Regulations: [GDPR/HIPAA/PCI-DSS/etc.]
Data Handled: [TYPES_OF_DATA]
Geographic Scope: [REGIONS]
Audit Requirements: [FREQUENCY]

Identify:
- Regulatory compliance gaps
- Data privacy risks
- Audit failure risks
- Legal liability risks
- Documentation gaps
- Process compliance risks
- Remediation priorities
```

## Risk Analysis Template

```
# Risk Analysis for [PROJECT/FEATURE_NAME]

## Risk Identification

| Risk ID | Risk Description | Category | Likelihood | Impact | Risk Score |
|---------|-----------------|----------|------------|--------|------------|
| R001 | [DESCRIPTION] | [TECHNICAL/RESOURCE/etc.] | [H/M/L] | [H/M/L] | [SCORE] |
| R002 | [DESCRIPTION] | [CATEGORY] | [H/M/L] | [H/M/L] | [SCORE] |

## Risk Prioritization Matrix

```
         Impact
         High  | R001, R003 | R002, R005 |
Likelihood Med   | R004       | R006       |
         Low   | R007       | R008       |
               |------------|------------|
                 High         Medium       Low
```

## Detailed Risk Analysis

### Risk R001: [RISK_NAME]
- **Description**: [DETAILED_DESCRIPTION]
- **Category**: [CATEGORY]
- **Likelihood**: [HIGH/MEDIUM/LOW] - [JUSTIFICATION]
- **Impact**: [HIGH/MEDIUM/LOW] - [JUSTIFICATION]
- **Risk Score**: [CALCULATED_SCORE]
- **Triggers**: [WHAT_WOULD_CAUSE_THIS]
- **Indicators**: [EARLY_WARNING_SIGNS]

**Mitigation Strategy**:
- Preventive Actions: [ACTIONS_TO_PREVENT]
- Contingency Plan: [IF_IT_OCCURS]
- Owner: [RESPONSIBLE_PERSON]
- Timeline: [WHEN_TO_IMPLEMENT]

**Monitoring**:
- Metrics: [HOW_TO_MEASURE]
- Frequency: [HOW_OFTEN_TO_CHECK]
- Escalation: [WHEN_TO_ESCALATE]

## Risk Categories

### Technical Risks
- [RISK_1]
- [RISK_2]

### Resource Risks
- [RISK_1]
- [RISK_2]

### Schedule Risks
- [RISK_1]
- [RISK_2]

### Quality Risks
- [RISK_1]
- [RISK_2]

### Business Risks
- [RISK_1]
- [RISK_2]

## Overall Risk Assessment

**Overall Risk Level**: [HIGH/MEDIUM/LOW]

**Key Concerns**:
1. [CONCERN_1]
2. [CONCERN_2]

**Recommendations**:
1. [RECOMMENDATION_1]
2. [RECOMMENDATION_2]

**Go/No-Go Recommendation**: [GO/NO-GO/CONDITIONAL]
- Conditions (if conditional): [CONDITIONS]
```

## Risk Scoring Guide

### Likelihood
- **High (3)**: Very likely to occur (>60% probability)
- **Medium (2)**: May occur (30-60% probability)
- **Low (1)**: Unlikely to occur (<30% probability)

### Impact
- **High (3)**: Severe impact on project success
- **Medium (2)**: Moderate impact, manageable
- **Low (1)**: Minor impact, easily handled

### Risk Score
- **Risk Score = Likelihood × Impact**
- **High Risk**: Score 6-9 (Immediate action required)
- **Medium Risk**: Score 3-4 (Plan mitigation)
- **Low Risk**: Score 1-2 (Monitor)

## Best Practices

1. **Early Identification**: Identify risks as early as possible
2. **Continuous Monitoring**: Regularly review and update risk status
3. **Stakeholder Involvement**: Get input from all stakeholders
4. **Proactive Mitigation**: Don't wait for risks to materialize
5. **Document Everything**: Keep detailed risk logs
6. **Learn from History**: Review past project risks
7. **Quantify When Possible**: Use data to support assessments
8. **Balance Risk and Reward**: Consider business value

## Risk Mitigation Strategies

### Avoidance
- Change approach to eliminate the risk
- Remove risky features or dependencies

### Reduction
- Implement controls to reduce likelihood or impact
- Add testing, reviews, or validation steps

### Transfer
- Outsource risky components
- Use insurance or warranties

### Acceptance
- Acknowledge the risk and prepare contingency
- Monitor closely and have response plan ready

## Common Risk Categories Checklist

- [ ] Technical/Technology risks
- [ ] Integration risks
- [ ] Performance risks
- [ ] Security risks
- [ ] Data risks
- [ ] Resource/Staffing risks
- [ ] Schedule/Timeline risks
- [ ] Budget/Cost risks
- [ ] Third-party/Vendor risks
- [ ] Compliance/Regulatory risks
- [ ] Quality risks
- [ ] Business/Market risks

---
- Tham khảo: [Link](https://github.com/tayyabakmal1/qa-prompt-library/blob/main/manual-qa/test-planning/risk-analysis-prompts.md)