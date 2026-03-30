# Automation Testing Interview Questions

> Câu hỏi phỏng vấn Automation Testing — từ cơ bản đến nâng cao.

---

## 🟢 Cơ bản

### 1. Automation Testing là gì? Khi nào nên tự động hóa?
**Trả lời**: Automation Testing là sử dụng công cụ/script để thực thi test cases tự động. Nên tự động hóa khi:
- Test cần chạy lặp đi lặp lại (regression)
- Test cần chạy trên nhiều browser/device
- Test có data-driven requirements
- Test cần chạy trong CI/CD pipeline

### 2. Page Object Model (POM) là gì?
**Trả lời**: POM là design pattern tách biệt UI elements và test logic:
- Mỗi page có 1 class riêng chứa locators và actions
- Test class sử dụng page objects thay vì tương tác trực tiếp với UI
- Dễ maintain khi UI thay đổi

### 3. Locator strategies trong Selenium/Playwright?
**Trả lời**: ID, Name, Class Name, CSS Selector, XPath, Link Text, Tag Name, Data-testid.
- **Best practice**: Ưu tiên ID/data-testid > CSS Selector > XPath

### 4. Explicit wait vs Implicit wait?
**Trả lời**:
- **Implicit**: Đợi global, áp dụng cho mọi element
- **Explicit**: Đợi có điều kiện, áp dụng cho element cụ thể
- **Best practice**: Dùng Explicit wait

### 5. Framework automation testing gồm những thành phần nào?
**Trả lời**: Test Runner, Page Objects, Test Data, Configuration, Reporting, Utilities, CI/CD Integration.

---

## 🟡 Trung cấp

### 6. Giải thích Data-driven Testing?
**Trả lời**: Tách test data ra khỏi test script, chạy cùng test logic với nhiều bộ data khác nhau.
- Source: CSV, Excel, JSON, Database
- Ví dụ: Test login với 50 cặp username/password khác nhau

### 7. Keyword-driven Testing là gì?
**Trả lời**: Actions được định nghĩa bằng keywords (Click, Type, Verify...). Non-technical users có thể viết test bằng cách kết hợp keywords. Robot Framework là ví dụ điển hình.

### 8. Làm thế nào xử lý Flaky Tests?
**Trả lời**:
- Dùng explicit waits thay vì sleep
- Retry mechanism cho flaky tests
- Isolate test data — mỗi test có data riêng
- Check race conditions
- Review test design, giảm dependencies
- Monitor và track flaky tests

### 9. Parallel Testing là gì? Lợi ích?
**Trả lời**: Chạy nhiều tests đồng thời. Lợi ích:
- Giảm thời gian chạy test suite
- Tận dụng tối đa resources
- Faster feedback trong CI/CD

### 10. Giải thích AAA Pattern?
**Trả lời**:
- **Arrange**: Setup test data và preconditions
- **Act**: Thực hiện action cần test
- **Assert**: Verify kết quả

---

## 🔴 Nâng cao

### 11. Thiết kế automation framework từ đầu gồm những bước nào?
**Trả lời**:
1. Chọn tech stack (language, framework, reporting)
2. Setup project structure (POM pattern)
3. Configure CI/CD integration
4. Implement base classes (BasePage, BaseTest)
5. Create utility functions
6. Setup test data management
7. Configure reporting
8. Define coding standards
9. Documentation

### 12. So sánh Selenium vs Playwright vs Cypress?
**Trả lời**:

| Tiêu chí | Selenium | Playwright | Cypress |
|---------|---------|-----------|---------|
| Browser | Chrome, Firefox, Safari, Edge | Chromium, Firefox, WebKit | Chrome, Firefox, Edge |
| Language | Multi | Multi | JS/TS only |
| Speed | Medium | Fast | Fast |
| Auto-wait | No | Yes | Yes |
| Network interception | Hard | Easy | Easy |
| Mobile | Via Appium | Emulation | Limited |
| Community | Largest | Growing fast | Large |

### 13. Làm thế nào để giảm maintenance cost cho test suite?
**Trả lời**:
- Solid POM architecture
- Reusable components & utilities
- Data-driven approach
- Self-healing locators
- Regular refactoring
- Code review cho test code
- CI/CD integration sớm

### 14. Integration testing trong CI/CD pipeline?
**Trả lời**:
- Unit tests: chạy trên mỗi commit
- Integration/API tests: chạy trên mỗi PR
- E2E tests: chạy trước deploy staging
- Smoke tests: chạy sau deploy production
- Performance tests: scheduled runs

---

## 📚 Tham khảo

- [Test Automation University](https://testautomationu.applitools.com/)
- [Playwright Documentation](https://playwright.dev/docs/intro)
