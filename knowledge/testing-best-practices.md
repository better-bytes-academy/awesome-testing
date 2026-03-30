# Testing Best Practices

> Các thực hành tốt nhất trong kiểm thử phần mềm.

---

## 📌 Mục lục

- [Viết Test Case hiệu quả](#viết-test-case-hiệu-quả)
- [Bug Report chất lượng](#bug-report-chất-lượng)
- [Test Automation Best Practices](#test-automation-best-practices)
- [CI/CD Testing](#cicd-testing)
- [Test Environment Management](#test-environment-management)
- [Communication & Collaboration](#communication--collaboration)

---

## Viết Test Case hiệu quả

### Nguyên tắc

1. **Rõ ràng & cụ thể** — Mỗi test case chỉ kiểm tra một điều
2. **Độc lập** — Không phụ thuộc vào test case khác
3. **Có thể lặp lại** — Chạy nhiều lần cho cùng kết quả
4. **Có test data cụ thể** — Không dùng "enter valid data"
5. **Expected result rõ ràng** — Mô tả chính xác kết quả mong đợi

### Ví dụ tốt vs xấu

❌ **Xấu:**
> Test login feature

✅ **Tốt:**
> **TC-001**: Verify user can login with valid email "test@email.com" and password "Test@123"
> - Precondition: User account exists and is active
> - Steps: Navigate to login page → Enter email → Enter password → Click Login
> - Expected: User is redirected to Dashboard, welcome message displays username

---

## Bug Report chất lượng

### Template chuẩn

```
Title: [Module] - Mô tả ngắn gọn bug
Severity: Critical / Major / Minor / Trivial
Priority: High / Medium / Low
Environment: Browser, OS, Device
Precondition: Điều kiện tiên quyết

Steps to Reproduce:
1. Step 1
2. Step 2
3. Step 3

Actual Result: Kết quả thực tế
Expected Result: Kết quả mong đợi
Attachments: Screenshot / Video / Log
```

### Mẹo viết bug report

- **Title**: Ngắn gọn nhưng đủ thông tin — `[Login] - Error 500 when submitting empty email`
- **Steps**: Đủ chi tiết để developer reproduce được
- **Evidence**: Luôn đính kèm screenshot hoặc video
- **Severity vs Priority**: Hiểu rõ sự khác biệt và đánh đúng mức

---

## Test Automation Best Practices

### Khi nào nên tự động hóa?

✅ **Nên tự động**:
- Regression test — chạy lặp đi lặp lại
- Smoke test — cần chạy nhanh sau mỗi build
- Data-driven test — cùng logic, nhiều data
- Cross-browser / Cross-device test

❌ **Không nên tự động**:
- Test chạy một lần duy nhất
- Exploratory testing
- UI thay đổi liên tục
- Usability testing

### Design Patterns

| Pattern | Mô tả |
|---------|-------|
| **Page Object Model (POM)** | Tách logic test và UI elements |
| **Screenplay Pattern** | Actor-based, task-oriented |
| **Factory Pattern** | Tạo test data linh hoạt |
| **Builder Pattern** | Xây dựng complex test objects |

### Nguyên tắc viết automation test

1. **DRY** — Don't Repeat Yourself
2. **KISS** — Keep It Simple, Stupid
3. **AAA** — Arrange, Act, Assert
4. **Independent** — Test không phụ thuộc nhau
5. **Fast** — Chạy nhanh, feedback nhanh
6. **Reliable** — Không flaky, kết quả ổn định

---

## CI/CD Testing

### Testing trong Pipeline

```
Code Push → Build → Unit Tests → Integration Tests → Deploy to Staging → E2E Tests → Deploy to Production
```

### Checklist CI/CD Testing

- [ ] Unit tests chạy trên mỗi commit
- [ ] Integration tests chạy trên mỗi PR
- [ ] E2E tests chạy trước deploy staging
- [ ] Smoke tests chạy sau deploy production
- [ ] Performance tests chạy scheduled (weekly)
- [ ] Security scan tự động trong pipeline

---

## Test Environment Management

### Best Practices

1. **Tách biệt môi trường**: Dev → QA → Staging → Production
2. **Data riêng biệt**: Không dùng production data để test
3. **Configuration management**: Dùng env variables, không hardcode
4. **Reset capability**: Có khả năng reset environment nhanh
5. **Monitoring**: Theo dõi health của test environment

### Test Data Strategy

| Phương pháp | Ưu điểm | Nhược điểm |
|------------|---------|-----------|
| **Manual creation** | Kiểm soát cao | Tốn thời gian |
| **Data generation** | Nhanh, đa dạng | Có thể không realistic |
| **Production copy** | Realistic | Rủi ro bảo mật |
| **Synthetic data** | An toàn, đa dạng | Cần công cụ |

---

## Communication & Collaboration

### Với Developer

- Báo bug rõ ràng, có evidence
- Discuss trước khi log bug nếu không chắc
- Không blame, tập trung vào giải pháp

### Với Product Owner

- Clarify requirement sớm
- Đề xuất edge cases khi review story
- Report tiến độ testing rõ ràng

### Trong Team

- Daily standup: chia sẻ blockers
- Sprint retrospective: cải thiện process
- Knowledge sharing sessions

---

## 📚 Tham khảo

- [Google Testing Blog](https://testing.googleblog.com/)
- [Ministry of Testing](https://www.ministryoftesting.com/)
- [Test Automation University](https://testautomationu.applitools.com/)
