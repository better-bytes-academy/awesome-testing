# Test Case Template

> Mẫu test case tiêu chuẩn.

---

## Test Case Format

### Single Test Case

| Field | Value |
|-------|-------|
| **Test Case ID** | TC-[Module]-[Number] |
| **Module** | [Tên module] |
| **Title** | [Mô tả ngắn gọn] |
| **Priority** | High / Medium / Low |
| **Type** | Positive / Negative / Boundary |
| **Preconditions** | [Điều kiện tiên quyết] |
| **Test Data** | [Dữ liệu cụ thể] |

**Steps:**

| # | Action | Expected Result |
|---|--------|----------------|
| 1 | [Bước 1] | [Kết quả mong đợi 1] |
| 2 | [Bước 2] | [Kết quả mong đợi 2] |
| 3 | [Bước 3] | [Kết quả mong đợi 3] |

**Actual Result:** [Kết quả thực tế khi thực thi]

**Status:** Pass / Fail / Blocked / Not Executed

---

## Ví dụ Test Cases

### Module: Login

#### TC-LOGIN-001: Login thành công với email và password hợp lệ

| Field | Value |
|-------|-------|
| **Priority** | High |
| **Type** | Positive |
| **Preconditions** | User account `test@email.com` / `Test@123` đã tồn tại và active |

| # | Action | Expected Result |
|---|--------|----------------|
| 1 | Navigate to login page | Login form hiển thị với email, password fields và Login button |
| 2 | Enter email: `test@email.com` | Email field hiển thị giá trị đã nhập |
| 3 | Enter password: `Test@123` | Password field hiển thị dạng masked (•••) |
| 4 | Click Login button | Redirect đến Dashboard, hiển thị welcome message |

---

#### TC-LOGIN-002: Login thất bại với password sai

| Field | Value |
|-------|-------|
| **Priority** | High |
| **Type** | Negative |
| **Preconditions** | User account `test@email.com` đã tồn tại |

| # | Action | Expected Result |
|---|--------|----------------|
| 1 | Navigate to login page | Login form hiển thị |
| 2 | Enter email: `test@email.com` | Email field hiển thị giá trị đã nhập |
| 3 | Enter password: `WrongPass` | Password field hiển thị dạng masked |
| 4 | Click Login button | Error message: "Invalid email or password" |

---

#### TC-LOGIN-003: Login với email trống

| Field | Value |
|-------|-------|
| **Priority** | Medium |
| **Type** | Negative |
| **Preconditions** | None |

| # | Action | Expected Result |
|---|--------|----------------|
| 1 | Navigate to login page | Login form hiển thị |
| 2 | Leave email field empty | |
| 3 | Enter password: `Test@123` | |
| 4 | Click Login button | Validation error: "Email is required" |

---

## Test Case Checklist Table

> Format bảng cho nhiều test cases cùng lúc:

| ID | Title | Priority | Precondition | Steps | Expected Result | Status |
|----|-------|----------|-------------|-------|----------------|--------|
| TC-001 | Login with valid credentials | High | Active account | Enter email, password → Click Login | Redirect to Dashboard | |
| TC-002 | Login with wrong password | High | Active account | Enter email, wrong password → Click Login | Error message displayed | |
| TC-003 | Login with empty email | Medium | None | Leave email empty → Click Login | "Email is required" error | |
| TC-004 | Login with invalid email format | Medium | None | Enter "invalid-email" → Click Login | "Invalid email format" error | |
| TC-005 | Login with locked account | High | Locked account | Enter credentials → Click Login | "Account is locked" message | |
