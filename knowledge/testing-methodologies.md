# Testing Methodologies

> Các phương pháp luận và kỹ thuật thiết kế kiểm thử.

---

## 📌 Mục lục

- [Test Design Techniques](#test-design-techniques)
- [Black-box vs White-box vs Grey-box](#black-box-vs-white-box-vs-grey-box)
- [Static vs Dynamic Testing](#static-vs-dynamic-testing)
- [Agile Testing](#agile-testing)
- [Shift-Left Testing](#shift-left-testing)
- [TDD, BDD, ATDD](#tdd-bdd-atdd)

---

## Test Design Techniques

### Black-box Techniques

| Kỹ thuật | Mô tả | Ví dụ |
|---------|-------|-------|
| **Equivalence Partitioning** | Chia dữ liệu thành các nhóm tương đương | Tuổi: [1-17], [18-65], [66-120] |
| **Boundary Value Analysis** | Test tại biên của mỗi nhóm | Tuổi: 0, 1, 17, 18, 65, 66, 120, 121 |
| **Decision Table** | Test các tổ hợp điều kiện | Login: username đúng/sai × password đúng/sai |
| **State Transition** | Test các trạng thái và chuyển đổi | Account: Active → Locked → Suspended |
| **Use Case Testing** | Test theo kịch bản sử dụng | User flow: Register → Login → Purchase |

### White-box Techniques

| Kỹ thuật | Mô tả |
|---------|-------|
| **Statement Coverage** | Đảm bảo mỗi dòng code được thực thi ít nhất 1 lần |
| **Branch Coverage** | Đảm bảo mỗi nhánh (if/else) được thực thi |
| **Path Coverage** | Đảm bảo mỗi đường đi trong code được thực thi |
| **Condition Coverage** | Đảm bảo mỗi điều kiện boolean được test cả true/false |

### Experience-based Techniques

| Kỹ thuật | Mô tả |
|---------|-------|
| **Error Guessing** | Dựa trên kinh nghiệm để đoán lỗi có thể xảy ra |
| **Exploratory Testing** | Khám phá và test đồng thời |
| **Checklist-based Testing** | Test dựa trên danh sách kiểm tra |

---

## Black-box vs White-box vs Grey-box

| Tiêu chí | Black-box | White-box | Grey-box |
|---------|----------|----------|---------|
| **Kiến thức code** | Không cần | Cần | Một phần |
| **Ai thực hiện** | QA | Developer | QA/Dev |
| **Tập trung vào** | Chức năng | Cấu trúc code | Cả hai |
| **Ví dụ** | Functional Testing | Unit Testing | Integration Testing |

---

## Static vs Dynamic Testing

| Tiêu chí | Static Testing | Dynamic Testing |
|---------|---------------|----------------|
| **Thực thi code** | Không | Có |
| **Phương pháp** | Review, Inspection, Walkthrough | Test execution |
| **Tìm lỗi** | Lỗi thiết kế, logic, coding standards | Lỗi runtime, functional |
| **Chi phí** | Thấp hơn | Cao hơn |
| **Thời điểm** | Sớm trong SDLC | Sau khi có code chạy được |

---

## Agile Testing

### Nguyên tắc Agile Testing

1. **Testing là hoạt động liên tục** — không phải giai đoạn riêng biệt
2. **Whole team approach** — cả team chịu trách nhiệm chất lượng
3. **Fast feedback** — phản hồi nhanh qua CI/CD
4. **Customer collaboration** — hợp tác chặt chẽ với khách hàng

### Agile Testing Quadrants

```
         Business-Facing
              │
   Q2         │         Q3
 Automated    │    Manual
 Functional   │    Exploratory
 Tests        │    Usability
              │    UAT
──────────────┼──────────────
   Q1         │         Q4
 Automated    │    Tools
 Unit Tests   │    Performance
 Component    │    Security
 Tests        │    Load
              │
        Technology-Facing
```

---

## Shift-Left Testing

> Đưa hoạt động kiểm thử về sớm hơn trong vòng đời phát triển.

### Lợi ích
- Phát hiện lỗi sớm → giảm chi phí sửa
- Cải thiện chất lượng code
- Tăng tốc delivery

### Thực hành
- Code review từ đầu
- Unit test bắt buộc
- Static analysis tự động
- Test trong CI/CD pipeline
- QA tham gia từ giai đoạn requirement

---

## TDD, BDD, ATDD

### TDD (Test-Driven Development)

```
Red → Green → Refactor
 │       │        │
 │       │        └─ Cải thiện code
 │       └─ Viết code đủ để pass test
 └─ Viết test fail trước
```

### BDD (Behavior-Driven Development)

- Mở rộng từ TDD, tập trung vào hành vi
- Sử dụng ngôn ngữ tự nhiên (Gherkin)

```gherkin
Feature: Login
  Scenario: Successful login
    Given user is on login page
    When user enters valid credentials
    Then user should see dashboard
```

### ATDD (Acceptance Test-Driven Development)

- Test được viết dựa trên acceptance criteria
- Collaboration giữa Dev, QA, PO
- Test case = specification

### So sánh

| Tiêu chí | TDD | BDD | ATDD |
|---------|-----|-----|------|
| **Focus** | Code | Behavior | Requirements |
| **Người viết test** | Developer | Dev + QA + PO | Dev + QA + PO |
| **Ngôn ngữ** | Code | Gherkin/Natural | Natural language |
| **Công cụ** | JUnit, pytest | Cucumber, SpecFlow | FitNesse, Robot Framework |

---

## 📚 Tham khảo

- [ISTQB Foundation Level Syllabus - Test Design Techniques](https://www.istqb.org/)
- [Agile Testing Quadrants - Lisa Crispin](https://lisacrispin.com/2011/11/08/using-the-agile-testing-quadrants/)
- [Shift Left Testing - SmartBear](https://smartbear.com/learn/automated-testing/shift-left-testing/)
