# Các Câu Lệnh (Prompts) Cho Kế Hoạch Kiểm Thử

## 1. Tạo Kế hoạch Kiểm thử Toàn diện

```text
Tạo một kế hoạch kiểm thử chi tiết cho:

Dự án: [TÊN_DỰ_ÁN]
Phiên bản Phát hành: [PHIÊN_BẢN]
Các Tính năng cần Kiểm thử: [DANH_SÁCH_TÍNH_NĂNG]
Thời gian Kiểm thử: [NGÀY_BẮT_ĐẦU đến NGÀY_KẾT_THÚC]
Đội ngũ: [SỐ_LƯỢNG_TESTER]
Môi trường: [CHI_TIẾT_MÔI_TRƯỜNG_KIỂM_THỬ]

Hãy tạo một kế hoạch kiểm thử bao gồm:
- Mục tiêu và phạm vi kiểm thử
- Các hạng mục kiểm thử (các tính năng cần kiểm thử)
- Các tính năng không nằm trong phạm vi kiểm thử
- Phương pháp và cách tiếp cận kiểm thử
- Tiêu chí đạt/không đạt (Pass/fail criteria)
- Các sản phẩm bàn giao (Test deliverables)
- Yêu cầu về tài nguyên
- Lịch trình và các cột mốc quan trọng
- Rủi ro và biện pháp giảm thiểu
```

## 2. Kế hoạch Kiểm thử Sprint

```text
Tạo một kế hoạch kiểm thử Sprint cho:

Sprint số: [SỐ_SPRINT]
Mục tiêu Sprint: [MỤC_TIÊU]
User Stories: [DANH_SÁCH_STORIES]
Thời lượng Sprint: [SỐ_TUẦN]
Năng suất Nhóm (Capacity): [SỐ_GIỜ/ĐIỂM]

Bao gồm:
- Các story cần kiểm thử
- Cách tiếp cận kiểm thử cho từng story
- Xác thực các tiêu chí chấp nhận (Acceptance criteria)
- Phạm vi kiểm thử hồi quy (Regression)
- Các tác vụ tự động hóa (Automation)
- Các hoạt động kiểm thử hàng ngày
- Định nghĩa Hoàn thành (Definition of Done)
- Mục tiêu kiểm thử của Sprint
```

## 3. Kế hoạch Kiểm thử Phát hành (Release)

```text
Tạo một kế hoạch kiểm thử phát hành cho:

Phiên bản Phát hành: [PHIÊN_BẢN]
Ngày Phát hành: [NGÀY]
Phạm vi Phát hành: [CÁC_TÍNH_NĂNG/CÁC_BẢN_VÁ_LỖI]
Phiên bản Trước đó: [PHIÊN_BẢN]
Loại hình Triển khai: [THEO_GIAI_ĐOẠN (PHASED) / ĐỒNG_LOẠT (BIG_BANG)]

Bao gồm các nội dung:
- Phạm vi kiểm thử bản phát hành
- Chiến lược kiểm thử hồi quy
- Danh sách kiểm tra Smoke Test (Kiểm thử luồng chính)
- Đánh giá hiệu năng
- Kiểm tra bảo mật
- Kiểm thử chuyển đổi dữ liệu (nếu có)
- Kiểm thử khôi phục (Rollback)
- Tiêu chí Quyết định triển khai (Go/No-Go criteria)
- Giám sát sau phát hành
```

## 4. Kế hoạch Kiểm thử Chuyên biệt cho Tính năng

```text
Tạo một kế hoạch kiểm thử cho một tính năng cụ thể:

Tên Tính năng: [TÊN_TÍNH_NĂNG]
Mô tả Tính năng: [MÔ_TẢ_TÍNH_NĂNG]
User Stories: [DANH_SÁCH_STORIES]
Các Phụ thuộc (Dependencies): [MÔ_TẢ_CÁC_PHỤ_THUỘC]
Tiêu chí Chấp nhận: [DANH_SÁCH_TIÊU_CHÍ]

Bao gồm:
- Phạm vi kiểm thử tính năng
- Các kịch bản và ca kiểm thử (Test scenarios & cases)
- Các điểm tích hợp cần kiểm thử
- Yêu cầu về dữ liệu kiểm thử
- Yêu cầu về môi trường
- Lịch trình kiểm thử
- Tiêu chí đầu vào và đầu ra (Entry and exit criteria)
- Đánh giá rủi ro cho tính năng này
```

## 5. Kế hoạch Kiểm thử Tích hợp

```text
Phát triển một kế hoạch kiểm thử tích hợp cho:

Các Hệ thống cần Tích hợp: [HỆ_THỐNG_A] với [HỆ_THỐNG_B]
Loại Tích hợp: [API/DATABASE/FILE/MESSAGE]
Các Điểm Tích hợp: [DANH_SÁCH_ENDPOINT/GIAO_DIỆN]
Luồng Dữ liệu: [MÔ_TẢ_LUỒNG]

Bao gồm các nội dung:
- Phạm vi kiểm thử tích hợp
- Phương pháp kiểm thử giao diện
- Xác thực trao đổi dữ liệu
- Các kịch bản xử lý lỗi
- Kiểm thử hiệu năng
- Kiểm thử bảo mật
- Các luồng công việc End-to-end
- Thiết lập môi trường tích hợp
```

## 6. Kế hoạch Kiểm thử Hiệu năng

```text
Tạo một kế hoạch kiểm thử hiệu năng cho:

Ứng dụng: [TÊN_ỨNG_DỤNG]
Mục tiêu Hiệu năng: [THỜI_GIAN_PHẢN_HỒI/THÔNG_LƯỢNG]
Tải Dự kiến: [SỐ_USER/TPS]
Các Giao dịch Quan trọng: [DANH_SÁCH_GIAO_DỊCH]
Thời gian Kiểm thử: [THỜI_LƯỢNG]

Bao gồm:
- Mục tiêu kiểm thử hiệu năng
- Các loại kiểm thử (Load, Stress, Spike, Endurance)
- Các kịch bản kiểm thử và mô hình tải (Workload models)
- Các chỉ số và KPIs hiệu năng
- Khối lượng dữ liệu kiểm thử
- Thông số kỹ thuật của môi trường kiểm thử
- Chiến lược giám sát
- Tiêu chí thành công
- Đường cơ sở hiệu năng (Performance baseline)
```

## 7. Kế hoạch Kiểm thử Bảo mật

```text
Tạo một kế hoạch kiểm thử bảo mật cho:

Ứng dụng: [TÊN_ỨNG_DỤNG]
Yêu cầu Bảo mật: [CÁC_YÊU_CẦU]
Tiêu chuẩn Tuân thủ: [OWASP/GDPR/v.v.]
Các Loại Dữ liệu Nhạy cảm: [DANH_SÁCH_DỮ_LIỆU]
Các Vấn đề Bảo mật Trước đó: [NẾU_CÓ]

Bao gồm các nội dung:
- Phạm vi kiểm thử bảo mật
- Phương pháp đánh giá lỗ hổng
- Chiến lược kiểm thử thâm nhập (Penetration testing)
- Kiểm thử xác thực/phân quyền
- Kiểm thử bảo vệ dữ liệu
- Các công cụ bảo mật sẽ sử dụng
- Bảo mật môi trường kiểm thử
- Quy trình báo cáo và khắc phục
```

## 8. Kế hoạch Kiểm thử Hồi quy

```text
Tạo một kế hoạch kiểm thử hồi quy cho:

Ứng dụng: [TÊN_ỨNG_DỤNG]
Các Thay đổi trong Bản phát hành này: [MÔ_TẢ_THAY_ĐỔI]
Kích thước Bộ kiểm thử Hồi quy: [SỐ_LƯỢNG_TEST_CASE]
Thời gian Cho phép: [THỜI_LƯỢNG]
Mức độ Phủ Tự động hóa: [PHẦN_TRĂM]

Bao gồm:
- Phạm vi kiểm thử hồi quy
- Tiêu chí lựa chọn test case
- Chiến lược ưu tiên
- Phân chia tỷ lệ Tự động (Automated) vs Thủ công (Manual)
- Lịch trình thực thi
- Yêu cầu về môi trường
- Tiêu chí đạt/không đạt
- Quản lý lỗi (Defect management)
```

## 9. Kế hoạch Kiểm thử UAT

```text
Phát triển một kế hoạch kiểm thử UAT (Nghiệm thu Người dùng) cho:

Dự án: [TÊN_DỰ_ÁN]
Người dùng Nghiệp vụ: [PHÒNG_BAN/VAI_TRÒ]
Các Kịch bản Nghiệp vụ: [CÁC_KỊCH_BẢN_CHÍNH]
Thời gian UAT: [LỊCH_TRÌNH]
Địa điểm UAT: [TRỰC_TIẾP/TỪ_XA]

Bao gồm các nội dung:
- Mục tiêu và phạm vi UAT
- Tiêu chí lựa chọn người dùng tham gia
- Kế hoạch đào tạo người dùng
- Tạo kịch bản kiểm thử
- Thiết lập môi trường UAT
- Lịch trình và hậu cần
- Quy trình thu thập phản hồi
- Luồng công việc giải quyết vấn đề
- Quy trình nghiệm thu ký duyệt (Sign-off)
```

## 10. Kế hoạch Kiểm thử Ứng dụng Di động

```text
Tạo một kế hoạch kiểm thử ứng dụng di động cho:

Tên Ứng dụng: [TÊN_ỨNG_DỤNG]
Nền tảng: [iOS/ANDROID/CẢ_HAI]
Loại Ứng dụng: [NATIVE/HYBRID/WEB]
Thiết bị Mục tiêu: [DANH_SÁCH_THIẾT_BỊ]
Phiên bản Hệ điều hành: [CÁC_PHIÊN_BẢN_HỖ_TRỢ]

Bao gồm:
- Chiến lược bao phủ thiết bị
- Phạm vi kiểm thử chức năng
- Kiểm thử đặc thù theo nền tảng
- Kiểm thử chức năng ngoại tuyến (Offline)
- Kiểm thử hiệu năng
- Kiểm thử pin và tài nguyên
- Tuân thủ quy định của App Store/Play Store
- Kiểm thử bản cập nhật
- Chiến lược sử dụng thiết bị thật vs Trình giả lập (Simulator)
```

## 11. Kế hoạch Kiểm thử API

```text
Tạo một kế hoạch kiểm thử API cho:

Tên API: [TÊN_API]
Loại API: [REST/GRAPHQL/SOAP]
Số lượng Endpoint: [SỐ_LƯỢNG]
Phiên bản API: [PHIÊN_BẢN]
Xác thực: [LOẠI_XÁC_THỰC]

Bao gồm các nội dung:
- Phạm vi kiểm thử API
- Phương pháp kiểm thử chức năng
- Kiểm thử hợp đồng (Contract testing)
- Xác thực xử lý lỗi
- Kiểm thử hiệu năng
- Kiểm thử bảo mật
- Kiểm tra tài liệu API
- Khả năng tương thích ngược
- Chiến lược dữ liệu kiểm thử
```

## 12. Kế hoạch Kiểm thử Chuyển đổi Dữ liệu

```text
Tạo một kế hoạch kiểm thử chuyển đổi dữ liệu cho:

Hệ thống Nguồn: [TÊN_HỆ_THỐNG]
Hệ thống Đích: [TÊN_HỆ_THỐNG]
Khối lượng Dữ liệu: [KÍCH_THƯỚC]
Ngày Chuyển đổi: [NGÀY]
Loại Chuyển đổi: [BIG_BANG/THEO_GIAI_ĐOẠN]

Bao gồm:
- Các giai đoạn kiểm thử chuyển đổi
- Chiến lược xác thực dữ liệu
- Phương pháp đối chiếu (Reconciliation)
- Kiểm tra chất lượng dữ liệu
- Kiểm thử hiệu năng
- Kiểm thử khôi phục (Rollback)
- Kế hoạch chuyển đổi hệ thống (Cutover plan)
- Xác thực sau chuyển đổi
- Tiêu chí thành công
```

---

## Mẫu Kế Hoạch Kiểm Thử

```text
# Kế hoạch Kiểm thử cho [TÊN_DỰ_ÁN]

## 1. Thông tin Nhận dạng Kế hoạch Kiểm thử
- Mã Tài liệu: [ID]
- Phiên bản: [PHIÊN_BẢN]
- Ngày: [NGÀY]
- Tác giả: [TÊN]

## 2. Giới thiệu
- Mục đích của kế hoạch kiểm thử này
- Bối cảnh dự án
- Tham chiếu đến các tài liệu liên quan

## 3. Các Hạng mục Kiểm thử
Các tính năng/module cần được kiểm thử:
- [TÍNH_NĂNG_1] - [PHIÊN_BẢN]
- [TÍNH_NĂNG_2] - [PHIÊN_BẢN]

## 4. Các Tính năng Cần Kiểm thử
- [TÍNH_NĂNG_1]: [MÔ_TẢ]
- [TÍNH_NĂNG_2]: [MÔ_TẢ]

## 5. Các Tính năng Không nằm trong Phạm vi Kiểm thử
- [TÍNH_NĂNG_X]: [LÝ_DO]
- [TÍNH_NĂNG_Y]: [LÝ_DO]

## 6. Cách tiếp cận Kiểm thử
### Các Cấp độ Kiểm thử
- Kiểm thử Unit: [NGƯỜI_PHỤ_TRÁCH]
- Kiểm thử Tích hợp: [CÁCH_TIẾP_CẬN]
- Kiểm thử Hệ thống: [CÁCH_TIẾP_CẬN]
- UAT (Nghiệm thu Người dùng): [CÁCH_TIẾP_CẬN]

### Các Loại Kiểm thử
- Chức năng: [PHẠM_VI]
- Hiệu năng: [PHẠM_VI]
- Bảo mật: [PHẠM_VI]
- Tính khả dụng (Usability): [PHẠM_VI]

### Các Kỹ thuật Kiểm thử
- [KỸ_THUẬT_1]
- [KỸ_THUẬT_2]

## 7. Tiêu chí Đạt/Không đạt của Hạng mục
### Tiêu chí Đạt (Pass)
- Tất cả các test case nghiêm trọng (critical) đều pass
- Không có lỗi (defect) mức độ nghiêm trọng cao nào còn mở
- [CÁC_TIÊU_CHÍ_BỔ_SUNG]

### Tiêu chí Không đạt (Fail)
- Bất kỳ test case nghiêm trọng nào bị fail
- Các lỗi mức độ nghiêm trọng cao chưa được giải quyết
- [CÁC_TIÊU_CHÍ_BỔ_SUNG]

## 8. Tiêu chí Tạm dừng và Yêu cầu Tiếp tục lại
### Tạm dừng
- [TIÊU_CHÍ_1]
- [TIÊU_CHÍ_2]

### Tiếp tục lại
- [YÊU_CẦU_1]
- [YÊU_CẦU_2]

## 9. Các Sản phẩm Bàn giao (Test Deliverables)
### Trước khi Kiểm thử
- Kế hoạch kiểm thử
- Các ca kiểm thử (Test cases)
- Dữ liệu kiểm thử

### Trong khi Kiểm thử
- Báo cáo thực thi kiểm thử
- Báo cáo lỗi (Defect reports)

### Sau khi Kiểm thử
- Báo cáo tổng kết kiểm thử
- Các chỉ số và phân tích

## 10. Môi trường Kiểm thử
- Phần cứng: [THÔNG_SỐ_KỸ_THUẬT]
- Phần mềm: [HỆ_ĐIỀU_HÀNH, TRÌNH_DUYỆT, CÔNG_CỤ]
- Mạng: [CẤU_HÌNH]
- Dữ liệu Kiểm thử: [NGUỒN_VÀ_KHỐI_LƯỢNG]

## 11. Yêu cầu Nhân sự và Đào tạo
### Cấu trúc Nhóm
| Vai trò | Tên | Trách nhiệm |
|---------|-----|-------------|
| Trưởng nhóm Kiểm thử (Test Lead) | [TÊN] | [TRÁCH_NHIỆM] |
| Nhân viên Kiểm thử (Tester) | [TÊN] | [TRÁCH_NHIỆM] |

### Nhu cầu Đào tạo
- [ĐÀO_TẠO_1]
- [ĐÀO_TẠO_2]

## 12. Lịch trình
| Hoạt động | Ngày Bắt đầu | Ngày Kết thúc | Người Phụ trách |
|-----------|--------------|---------------|-----------------|
| Lập Kế hoạch Kiểm thử | [NGÀY] | [NGÀY] | [TÊN] |
| Thiết kế Kiểm thử | [NGÀY] | [NGÀY] | [TÊN] |
| Thực thi Kiểm thử | [NGÀY] | [NGÀY] | [TÊN] |
| Đóng Kiểm thử | [NGÀY] | [NGÀY] | [TÊN] |

## 13. Rủi ro và Biện pháp Giảm thiểu
| Rủi ro | Tác động | Xác suất | Biện pháp Giảm thiểu |
|--------|----------|----------|----------------------|
| [RỦI_RO_1] | [CAO/TB/THẤP] | [CAO/TB/THẤP] | [CHIẾN_LƯỢC] |
| [RỦI_RO_2] | [CAO/TB/THẤP] | [CAO/TB/THẤP] | [CHIẾN_LƯỢC] |

## 14. Phê duyệt
| Vai trò | Tên | Chữ ký | Ngày |
|---------|-----|--------|------|
| Quản lý Kiểm thử | [TÊN] | | |
| Quản lý Dự án | [TÊN] | | |
| Các Bên liên quan | [TÊN] | | |
```

## Các Thực Hành Tốt Nhất (Best Practices)

1. **Rõ Ràng, Cụ Thể**: Xác định rõ ràng phạm vi và mục tiêu.
2. **Lịch Trình Thực Tế**: Tính toán đến các yếu tố phụ thuộc và rủi ro.
3. **Sự Đồng Thuận của Các Bên Liên Quan**: Nhận được sự phê duyệt từ tất cả các bên liên quan.
4. **Tài Liệu Sống (Living Document)**: Cập nhật liên tục khi dự án tiến triển.
5. **Khả Năng Truy Xuất Nguồn Gốc (Traceability)**: Liên kết chặt chẽ với các yêu cầu và test case.
6. **Quản Lý Rủi Ro**: Nhận diện và lập kế hoạch cho các rủi ro.
7. **Tiêu Chí Rõ Ràng**: Định nghĩa các tiêu chí đạt/không đạt có thể đo lường được.
8. **Hoạch Định Tài Nguyên**: Đảm bảo đủ nguồn lực thực hiện.

## Danh Sách Kiểm Tra Các Phần Chung (Checklist)

- [ ] Các mục tiêu kiểm thử được nêu rõ ràng
- [ ] Định nghĩa rõ phạm vi (trong và ngoài phạm vi)
- [ ] Phương pháp tiếp cận kiểm thử được ghi chép lại
- [ ] Tiêu chí đầu vào và đầu ra được chỉ định rõ
- [ ] Các tài nguyên đã được xác định
- [ ] Lịch trình cùng các cột mốc quan trọng
- [ ] Các rủi ro và chiến lược giảm thiểu rủi ro
- [ ] Liệt kê các sản phẩm bàn giao (deliverables)
- [ ] Các yêu cầu về môi trường
- [ ] Chữ ký phê duyệt đầy đủ
---
# Test Plan Prompts

## 1. Comprehensive Test Plan Creation

```
Create a detailed test plan for:

Project: [PROJECT_NAME]
Release Version: [VERSION]
Features to Test: [LIST_FEATURES]
Testing Timeline: [START_DATE to END_DATE]
Team: [NUMBER_OF_TESTERS]
Environment: [TEST_ENVIRONMENT_DETAILS]

Generate a test plan including:
- Test objectives and scope
- Test items (features to be tested)
- Features not to be tested
- Test approach and methodology
- Pass/fail criteria
- Test deliverables
- Resource requirements
- Schedule and milestones
- Risks and mitigation
```

## 2. Sprint Test Plan

```
Create a sprint test plan for:

Sprint Number: [SPRINT_#]
Sprint Goal: [GOAL]
User Stories: [LIST_STORIES]
Sprint Duration: [WEEKS]
Team Capacity: [HOURS/POINTS]

Include:
- Stories to be tested
- Test approach per story
- Acceptance criteria validation
- Regression scope
- Automation tasks
- Daily testing activities
- Definition of Done
- Sprint testing goals
```

## 3. Release Test Plan

```
Generate a release test plan for:

Release Version: [VERSION]
Release Date: [DATE]
Release Scope: [FEATURES/FIXES]
Previous Version: [VERSION]
Deployment Type: [PHASED/BIG_BANG]

Cover:
- Release testing scope
- Regression testing strategy
- Smoke testing checklist
- Performance validation
- Security checks
- Data migration testing (if applicable)
- Rollback testing
- Go/No-Go criteria
- Post-release monitoring
```

## 4. Feature-Specific Test Plan

```
Create a test plan for a specific feature:

Feature Name: [FEATURE_NAME]
Feature Description: [DESCRIBE_FEATURE]
User Stories: [LIST_STORIES]
Dependencies: [DESCRIBE_DEPENDENCIES]
Acceptance Criteria: [LIST_CRITERIA]

Include:
- Feature testing scope
- Test scenarios and cases
- Integration points to test
- Test data requirements
- Environment needs
- Testing timeline
- Entry and exit criteria
- Risk assessment for this feature
```

## 5. Integration Test Plan

```
Develop an integration test plan for:

Systems to Integrate: [SYSTEM_A] with [SYSTEM_B]
Integration Type: [API/DATABASE/FILE/MESSAGE]
Integration Points: [LIST_ENDPOINTS/INTERFACES]
Data Flow: [DESCRIBE_FLOW]

Cover:
- Integration testing scope
- Interface testing approach
- Data exchange validation
- Error handling scenarios
- Performance testing
- Security testing
- End-to-end workflows
- Integration environment setup
```

## 6. Performance Test Plan

```
Create a performance test plan for:

Application: [APP_NAME]
Performance Goals: [RESPONSE_TIME/THROUGHPUT]
Expected Load: [USERS/TPS]
Critical Transactions: [LIST_TRANSACTIONS]
Test Duration: [DURATION]

Include:
- Performance test objectives
- Test types (load, stress, spike, endurance)
- Test scenarios and workload models
- Performance metrics and KPIs
- Test data volume
- Test environment specifications
- Monitoring strategy
- Success criteria
- Performance baseline
```

## 7. Security Test Plan

```
Generate a security test plan for:

Application: [APP_NAME]
Security Requirements: [REQUIREMENTS]
Compliance Standards: [OWASP/GDPR/etc.]
Sensitive Data Types: [LIST_DATA]
Previous Security Issues: [IF_ANY]

Cover:
- Security testing scope
- Vulnerability assessment approach
- Penetration testing strategy
- Authentication/authorization testing
- Data protection testing
- Security tools to use
- Test environment security
- Reporting and remediation process
```

## 8. Regression Test Plan

```
Create a regression test plan for:

Application: [APP_NAME]
Changes in This Release: [DESCRIBE_CHANGES]
Regression Suite Size: [NUMBER_OF_TESTS]
Time Available: [DURATION]
Automation Coverage: [PERCENTAGE]

Include:
- Regression testing scope
- Test selection criteria
- Prioritization strategy
- Automated vs manual split
- Execution schedule
- Environment requirements
- Pass/fail criteria
- Defect management
```

## 9. UAT Test Plan

```
Develop a UAT test plan for:

Project: [PROJECT_NAME]
Business Users: [DEPARTMENTS/ROLES]
Business Scenarios: [KEY_SCENARIOS]
UAT Duration: [TIMELINE]
UAT Location: [ONSITE/REMOTE]

Cover:
- UAT objectives and scope
- User selection criteria
- User training plan
- Test scenario creation
- UAT environment setup
- Schedule and logistics
- Feedback collection process
- Issue resolution workflow
- Sign-off process
```

## 10. Mobile App Test Plan

```
Create a mobile app test plan for:

App Name: [APP_NAME]
Platform: [iOS/ANDROID/BOTH]
App Type: [NATIVE/HYBRID/WEB]
Target Devices: [LIST_DEVICES]
OS Versions: [SUPPORTED_VERSIONS]

Include:
- Device coverage strategy
- Functional testing scope
- Platform-specific testing
- Offline functionality testing
- Performance testing
- Battery and resource testing
- App store compliance
- Update testing
- Real device vs simulator strategy
```

## 11. API Test Plan

```
Generate an API test plan for:

API Name: [API_NAME]
API Type: [REST/GRAPHQL/SOAP]
Number of Endpoints: [COUNT]
API Version: [VERSION]
Authentication: [TYPE]

Cover:
- API testing scope
- Functional testing approach
- Contract testing
- Error handling validation
- Performance testing
- Security testing
- Documentation validation
- Backward compatibility
- Test data strategy
```

## 12. Data Migration Test Plan

```
Create a data migration test plan for:

Source System: [SYSTEM_NAME]
Target System: [SYSTEM_NAME]
Data Volume: [SIZE]
Migration Date: [DATE]
Migration Type: [BIG_BANG/PHASED]

Include:
- Migration testing phases
- Data validation strategy
- Reconciliation approach
- Data quality checks
- Performance testing
- Rollback testing
- Cutover plan
- Post-migration validation
- Success criteria
```

## Test Plan Template

```
# Test Plan for [PROJECT_NAME]

## 1. Test Plan Identifier
- Document ID: [ID]
- Version: [VERSION]
- Date: [DATE]
- Author: [NAME]

## 2. Introduction
- Purpose of this test plan
- Project background
- References to related documents

## 3. Test Items
Features/modules to be tested:
- [FEATURE_1] - [VERSION]
- [FEATURE_2] - [VERSION]

## 4. Features to be Tested
- [FEATURE_1]: [DESCRIPTION]
- [FEATURE_2]: [DESCRIPTION]

## 5. Features Not to be Tested
- [FEATURE_X]: [REASON]
- [FEATURE_Y]: [REASON]

## 6. Test Approach
### Test Levels
- Unit Testing: [RESPONSIBILITY]
- Integration Testing: [APPROACH]
- System Testing: [APPROACH]
- UAT: [APPROACH]

### Test Types
- Functional: [SCOPE]
- Performance: [SCOPE]
- Security: [SCOPE]
- Usability: [SCOPE]

### Test Techniques
- [TECHNIQUE_1]
- [TECHNIQUE_2]

## 7. Item Pass/Fail Criteria
### Pass Criteria
- All critical test cases passed
- No open high-severity defects
- [ADDITIONAL_CRITERIA]

### Fail Criteria
- Any critical test case failed
- High-severity defects unresolved
- [ADDITIONAL_CRITERIA]

## 8. Suspension Criteria and Resumption Requirements
### Suspension
- [CRITERION_1]
- [CRITERION_2]

### Resumption
- [REQUIREMENT_1]
- [REQUIREMENT_2]

## 9. Test Deliverables
### Before Testing
- Test plan
- Test cases
- Test data

### During Testing
- Test execution reports
- Defect reports

### After Testing
- Test summary report
- Metrics and analysis

## 10. Test Environment
- Hardware: [SPECIFICATIONS]
- Software: [OS, BROWSERS, TOOLS]
- Network: [CONFIGURATION]
- Test Data: [SOURCE_AND_VOLUME]

## 11. Staffing and Training Needs
### Team Structure
| Role | Name | Responsibility |
|------|------|----------------|
| Test Lead | [NAME] | [RESPONSIBILITY] |
| Tester | [NAME] | [RESPONSIBILITY] |

### Training Needs
- [TRAINING_1]
- [TRAINING_2]

## 12. Schedule
| Activity | Start Date | End Date | Owner |
|----------|-----------|----------|-------|
| Test Planning | [DATE] | [DATE] | [NAME] |
| Test Design | [DATE] | [DATE] | [NAME] |
| Test Execution | [DATE] | [DATE] | [NAME] |
| Test Closure | [DATE] | [DATE] | [NAME] |

## 13. Risks and Mitigation
| Risk | Impact | Probability | Mitigation |
|------|--------|-------------|------------|
| [RISK_1] | [H/M/L] | [H/M/L] | [STRATEGY] |
| [RISK_2] | [H/M/L] | [H/M/L] | [STRATEGY] |

## 14. Approvals
| Role | Name | Signature | Date |
|------|------|-----------|------|
| Test Manager | [NAME] | | |
| Project Manager | [NAME] | | |
| Stakeholder | [NAME] | | |
```

## Best Practices

1. **Be Specific**: Clearly define scope and objectives
2. **Realistic Timelines**: Account for dependencies and risks
3. **Stakeholder Buy-in**: Get approval from all stakeholders
4. **Living Document**: Update as project evolves
5. **Traceability**: Link to requirements and test cases
6. **Risk Management**: Identify and plan for risks
7. **Clear Criteria**: Define measurable pass/fail criteria
8. **Resource Planning**: Ensure adequate resources

## Common Sections Checklist

- [ ] Test objectives clearly stated
- [ ] Scope (in and out) defined
- [ ] Test approach documented
- [ ] Entry and exit criteria specified
- [ ] Resources identified
- [ ] Schedule with milestones
- [ ] Risks and mitigation strategies
- [ ] Deliverables listed
- [ ] Environment requirements
- [ ] Approval signatures

--
- Tham khảo: [link](https://github.com/tayyabakmal1/qa-prompt-library/blob/main/manual-qa/test-planning/test-plan-prompts.md)