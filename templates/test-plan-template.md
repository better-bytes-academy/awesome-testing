# Test Plan Template

> Mẫu kế hoạch kiểm thử tiêu chuẩn.

---

## 1. Thông tin chung

| Thông tin | Chi tiết |
|----------|---------|
| **Project name** | [Tên dự án] |
| **Module** | [Tên module] |
| **Version** | [Phiên bản] |
| **Author** | [Tên người viết] |
| **Created date** | [DD/MM/YYYY] |
| **Last updated** | [DD/MM/YYYY] |
| **Reviewer** | [Tên người review] |
| **Status** | Draft / In Review / Approved |

---

## 2. Phạm vi kiểm thử (Test Scope)

### 2.1. In Scope
- [ ] Feature / Module 1
- [ ] Feature / Module 2
- [ ] Feature / Module 3

### 2.2. Out of Scope
- [ ] Feature / Module A (lý do)
- [ ] Feature / Module B (lý do)

---

## 3. Phương pháp kiểm thử (Test Approach)

### 3.1. Loại kiểm thử

| Loại kiểm thử | Status | Công cụ |
|---------------|--------|---------|
| Functional Testing | ✅ | Manual |
| Regression Testing | ✅ | Playwright |
| API Testing | ✅ | Postman / Playwright |
| Performance Testing | ❌ | - |
| Security Testing | ❌ | - |
| Accessibility Testing | ❌ | - |

### 3.2. Test Design Techniques
- Equivalence Partitioning
- Boundary Value Analysis
- Decision Table
- Exploratory Testing

---

## 4. Môi trường kiểm thử (Test Environment)

| Môi trường | URL | Database | Ghi chú |
|-----------|-----|----------|---------|
| DEV | [URL] | [DB name] | |
| QA/Staging | [URL] | [DB name] | |
| Production | [URL] | [DB name] | Read-only |

### 4.1. Browsers / Devices

| Browser/Device | Version |
|---------------|---------|
| Chrome | Latest |
| Firefox | Latest |
| Safari | Latest |
| Mobile (iOS) | iPhone 14+ |
| Mobile (Android) | Pixel 7+ |

---

## 5. Test Data

| Loại data | Mô tả | Nguồn |
|----------|-------|-------|
| User accounts | Test users với các roles | Tạo thủ công |
| Sample data | Product, order data | Seed script |
| Edge case data | Boundary values | Định nghĩa trong test case |

---

## 6. Entry & Exit Criteria

### 6.1. Entry Criteria
- [ ] Requirements đã được review và approve
- [ ] Test environment sẵn sàng
- [ ] Build deploy thành công
- [ ] Test data chuẩn bị xong
- [ ] Smoke test pass

### 6.2. Exit Criteria
- [ ] 100% test cases đã thực thi
- [ ] ≥ 95% test cases pass
- [ ] 0 Critical/Blocker bugs open
- [ ] ≤ 2 Major bugs open (có workaround)
- [ ] Test report đã được review

---

## 7. Lịch trình (Schedule)

| Giai đoạn | Ngày bắt đầu | Ngày kết thúc | Người phụ trách |
|----------|-------------|-------------|----------------|
| Test Planning | DD/MM | DD/MM | [Tên] |
| Test Case Design | DD/MM | DD/MM | [Tên] |
| Test Execution - Round 1 | DD/MM | DD/MM | [Tên] |
| Bug Fix & Retest | DD/MM | DD/MM | [Tên] |
| Test Execution - Round 2 | DD/MM | DD/MM | [Tên] |
| Regression Testing | DD/MM | DD/MM | [Tên] |
| Test Closure | DD/MM | DD/MM | [Tên] |

---

## 8. Risks & Mitigation

| Risk | Probability | Impact | Mitigation |
|------|-----------|--------|-----------|
| Requirements thay đổi | High | High | Agile approach, frequent sync |
| Environment không ổn định | Medium | High | Backup environment |
| Thiếu test data | Low | Medium | Chuẩn bị sớm, seed scripts |
| Thiếu nhân lực | Medium | Medium | Cross-training, prioritization |

---

## 9. Deliverables

- [ ] Test Plan (document này)
- [ ] Test Cases
- [ ] Test Execution Report
- [ ] Bug Report
- [ ] Test Summary Report

---

## 10. Approval

| Role | Tên | Ngày | Chữ ký |
|------|-----|------|--------|
| QA Lead | | | |
| Project Manager | | | |
| Product Owner | | | |
