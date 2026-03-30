# Manual Testing Interview Questions

> Câu hỏi phỏng vấn Manual Testing — từ cơ bản đến nâng cao.

---

## 🟢 Cơ bản (Fresher)

### 1. Kiểm thử phần mềm là gì?
**Trả lời**: Kiểm thử phần mềm là quá trình đánh giá và xác minh rằng sản phẩm phần mềm hoạt động đúng như mong đợi, phát hiện lỗi, và đảm bảo chất lượng trước khi phát hành.

### 2. Sự khác biệt giữa Verification và Validation?
**Trả lời**:
- **Verification**: "Are we building the product right?" — Kiểm tra quá trình phát triển (review, inspection)
- **Validation**: "Are we building the right product?" — Kiểm tra sản phẩm cuối (testing, UAT)

### 3. Liệt kê 7 nguyên tắc kiểm thử (ISTQB)?
**Trả lời**:
1. Testing shows presence of defects
2. Exhaustive testing is impossible
3. Early testing saves time and money
4. Defects cluster together
5. Pesticide paradox
6. Testing is context dependent
7. Absence-of-errors fallacy

### 4. Sự khác biệt giữa Severity và Priority?
**Trả lời**:
- **Severity**: Mức độ ảnh hưởng kỹ thuật (Critical, Major, Minor, Trivial)
- **Priority**: Mức độ ưu tiên sửa lỗi từ góc nhìn business (High, Medium, Low)
- Ví dụ: Logo sai → Severity: Minor, Priority: High (ảnh hưởng brand)

### 5. Smoke Testing vs Sanity Testing?
**Trả lời**:
| Smoke | Sanity |
|-------|--------|
| Kiểm tra tổng thể build | Kiểm tra chức năng cụ thể |
| Phạm vi rộng | Phạm vi hẹp |
| Sau mỗi build mới | Sau khi fix bug |

### 6. STLC (Software Testing Life Cycle) gồm những giai đoạn nào?
**Trả lời**: Requirement Analysis → Test Planning → Test Case Design → Environment Setup → Test Execution → Test Closure

### 7. Test Case gồm những thành phần nào?
**Trả lời**: Test Case ID, Title, Description, Preconditions, Test Steps, Test Data, Expected Result, Actual Result, Status, Priority, Module.

### 8. Regression Testing là gì? Khi nào cần thực hiện?
**Trả lời**: Regression Testing là kiểm tra lại các chức năng hiện có sau khi có code thay đổi. Cần thực hiện khi: fix bug, thêm feature mới, refactor code, thay đổi configuration.

---

## 🟡 Trung cấp (Junior - Mid)

### 9. Phân biệt các loại Integration Testing?
**Trả lời**:
- **Big Bang**: Tích hợp tất cả modules cùng lúc, test một lần
- **Top-Down**: Tích hợp từ module cao nhất xuống, dùng Stubs
- **Bottom-Up**: Tích hợp từ module thấp nhất lên, dùng Drivers
- **Sandwich**: Kết hợp Top-Down và Bottom-Up

### 10. Equivalence Partitioning và Boundary Value Analysis khác nhau thế nào?
**Trả lời**:
- **EP**: Chia input thành nhóm tương đương, chọn 1 giá trị đại diện mỗi nhóm
- **BVA**: Test tại các giá trị biên của mỗi nhóm
- Ví dụ: Age field [18-65] → EP: 10, 30, 80 | BVA: 17, 18, 65, 66

### 11. Kể tên các loại Test Documentation?
**Trả lời**: Test Strategy, Test Plan, Test Scenario, Test Case, Test Suite, Test Report, Traceability Matrix, Bug Report.

### 12. RTM (Requirement Traceability Matrix) là gì?
**Trả lời**: RTM là ma trận liên kết requirements với test cases, đảm bảo mỗi requirement đều có test case tương ứng. Giúp đánh giá test coverage.

### 13. Defect Life Cycle gồm những trạng thái nào?
**Trả lời**:
```
New → Assigned → Open → Fixed → Retest → Verified → Closed
                    ↓                  ↓
                 Rejected          Reopened
                    ↓
                 Deferred
```

### 14. Entry Criteria và Exit Criteria là gì?
**Trả lời**:
- **Entry Criteria**: Điều kiện cần đáp ứng trước khi bắt đầu test (test environment ready, test data prepared, build deployed)
- **Exit Criteria**: Điều kiện để kết thúc test (95% test cases passed, no critical bugs open, sign-off từ stakeholders)

---

## 🔴 Nâng cao (Senior)

### 15. Làm thế nào để ước lượng effort cho testing?
**Trả lời**: Có nhiều phương pháp:
- **Work Breakdown Structure (WBS)**: Phân chia task nhỏ, ước lượng từng task
- **Three-point estimation**: (Optimistic + 4×Most Likely + Pessimistic) / 6
- **Function Point Analysis**: Dựa trên complexity của features
- **Historical data**: Dựa trên dữ liệu từ dự án trước

### 16. Khi nào nên dừng test?
**Trả lời**: Dựa trên:
- Exit criteria đã đạt
- Budget/deadline hết
- Coverage đạt target
- Risk acceptable
- Defect rate giảm (defect convergence)

### 17. Làm thế nào để quản lý test khi requirements thay đổi liên tục?
**Trả lời**:
- Agile approach: chấp nhận thay đổi
- Modular test design: dễ cập nhật
- Risk-based testing: ưu tiên test quan trọng
- Automation cho regression
- Communication chặt chẽ với PO/BA

### 18. Giải thích Risk-based Testing?
**Trả lời**: Ưu tiên testing dựa trên risk assessment:
- **Risk = Probability × Impact**
- Xác định areas có risk cao nhất
- Phân bổ effort testing nhiều hơn cho high-risk areas
- Giảm effort cho low-risk areas

---

## 📚 Tham khảo

- [ISTQB Foundation Level Syllabus](https://www.istqb.org/)
- [Guru99 Testing Interview Questions](https://www.guru99.com/qa-interview-questions-answers.html)
