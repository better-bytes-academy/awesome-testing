# Senior QA Interview Questions

> Câu hỏi phỏng vấn cho vị trí Senior QA / QA Lead / QA Manager.

---

## 📌 Mục lục

- [Test Strategy & Planning](#test-strategy--planning)
- [Leadership & Process](#leadership--process)
- [Technical Depth](#technical-depth)
- [Behavioral Questions](#behavioral-questions)

---

## Test Strategy & Planning

### 1. Bạn xây dựng Test Strategy như thế nào cho một dự án mới?
**Trả lời**:
1. Hiểu requirements và business context
2. Identify risks và priority areas
3. Chọn test approach (manual vs automation ratio)
4. Define test levels (unit, integration, E2E)
5. Chọn tools và frameworks
6. Define metrics và reporting
7. Estimate effort và timeline
8. Define entry/exit criteria
9. Plan test environment và test data
10. Communicate với team

### 2. Làm thế nào để đo lường chất lượng testing?
**Trả lời**: Sử dụng các metrics:
- **Defect Density**: Số bugs / size of module
- **Defect Leakage**: Bugs found in production / total bugs
- **Test Coverage**: Test cases / requirements
- **Defect Removal Efficiency**: Bugs found before release / total bugs
- **Automation Coverage**: Automated tests / total tests
- **MTTR**: Mean Time To Repair

### 3. Risk-based Testing approach thực hiện như thế nào?
**Trả lời**:
1. Identify risks (technical, business, operational)
2. Assess probability và impact (High/Medium/Low)
3. Calculate risk level = Probability × Impact
4. Prioritize testing effort theo risk level
5. Allocate more effort cho high-risk areas
6. Regular re-assessment risks trong sprint

---

## Leadership & Process

### 4. Làm thế nào để cải thiện quy trình QA trong team?
**Trả lời**:
- Analyze current process, tìm bottlenecks
- Implement shift-left: QA tham gia sớm từ requirement
- Đưa automation vào CI/CD
- Establish coding standards cho test code
- Knowledge sharing sessions
- Retrospective và continuous improvement
- Measure và track QA metrics

### 5. Khi developer không đồng ý về bug bạn report, bạn xử lý thế nào?
**Trả lời**:
- Provide evidence rõ ràng (screenshots, logs, steps)
- Tham chiếu requirements/acceptance criteria
- Discuss cùng team, không biến thành confrontation
- Escalate lên PO/PM nếu cần quyết định business
- Document decision cho future reference

### 6. Làm thế nào để balance giữa quality và speed of delivery?
**Trả lời**:
- Risk-based testing: focus vào critical areas
- Automation cho regression → giảm manual effort
- Shift-left: phát hiện lỗi sớm → ít rework
- Define "good enough" quality với stakeholders
- Parallel testing khi có thể
- Feature flags để test in production safely

### 7. Bạn quản lý test automation debt như thế nào?
**Trả lời**:
- Track flaky tests và fix ngay
- Regular refactoring sessions
- Code review cho test code
- Delete tests không còn relevant
- Keep framework up-to-date
- Allocate 20% sprint capacity cho tech debt

---

## Technical Depth

### 8. Thiết kế test architecture cho microservices?
**Trả lời**:
- **Unit tests**: Mỗi service có unit tests riêng
- **Contract tests**: Verify API contracts giữa services (Pact)
- **Integration tests**: Test service interactions
- **E2E tests**: Test critical user journeys
- **Chaos testing**: Simulate failures
- Challenge: test data management, environment setup

### 9. Performance testing strategy cho production?
**Trả lời**:
- Baseline performance metrics
- Load testing: expected traffic
- Stress testing: peak hours simulation
- Soak testing: long-running stability
- Spike testing: sudden traffic increase
- Production monitoring: real-time alerts
- Capacity planning dựa trên growth projections

### 10. Testing trong DevOps/CI-CD pipeline?
**Trả lời**:
```
Commit → Build → Unit Tests → Static Analysis → Integration Tests
→ Deploy to QA → E2E Tests → Security Scan → Deploy to Staging
→ Smoke Tests → Performance Tests → Deploy to Production
→ Smoke Tests → Monitoring
```

---

## Behavioral Questions

### 11. Kể về một lần bạn phát hiện critical bug trước deadline?
> Mô tả tình huống cụ thể, cách bạn communicate, và kết quả

### 12. Kể về lần bạn cải thiện quy trình testing mang lại kết quả rõ rệt?
> Metrics trước/sau, approach đã dùng

### 13. Bạn handle thế nào khi bị áp lực release mà vẫn còn bugs?
> Risk assessment, communication, decision making process

### 14. Kinh nghiệm mentoring junior QA?
> Approach, challenges, results

---

## 📚 Tham khảo

- [Ministry of Testing](https://www.ministryoftesting.com/)
- [QA Lead Interview Guide](https://www.guru99.com/qa-interview-questions-answers.html)
