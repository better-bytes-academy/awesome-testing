# Bug Report Template

> Mẫu báo cáo lỗi tiêu chuẩn.

---

## Bug Report Format

### [BUG-ID] [Module] - Mô tả ngắn gọn

| Field | Value |
|-------|-------|
| **Bug ID** | BUG-[Number] |
| **Title** | [Module] - Mô tả ngắn gọn về bug |
| **Reporter** | [Tên người report] |
| **Date** | [DD/MM/YYYY] |
| **Severity** | Critical / Major / Minor / Trivial |
| **Priority** | High / Medium / Low |
| **Status** | New / Assigned / Open / Fixed / Verified / Closed / Reopened |
| **Assignee** | [Tên developer] |
| **Environment** | [Browser, OS, Device] |
| **Build/Version** | [v1.0.0 / Sprint 5 / Build #123] |
| **Module** | [Tên module] |

### Preconditions
[Điều kiện tiên quyết để reproduce bug]

### Steps to Reproduce
1. Step 1
2. Step 2
3. Step 3

### Actual Result
[Mô tả kết quả thực tế — bug xảy ra như thế nào]

### Expected Result
[Mô tả kết quả mong đợi — hệ thống nên hoạt động thế nào]

### Attachments
- Screenshot/Video: [link]
- Console log: [link]
- Network log: [link]

### Additional Info
[Thông tin bổ sung: frequency, workaround, related bugs]

---

## Hướng dẫn đánh Severity

| Severity | Mô tả | Ví dụ |
|----------|-------|-------|
| **Critical** | Hệ thống crash, mất dữ liệu, block hoàn toàn | App crash khi login, payment bị charge 2 lần |
| **Major** | Chức năng chính không hoạt động | Không thể thêm sản phẩm vào giỏ hàng |
| **Minor** | Chức năng phụ lỗi, có workaround | Sort không đúng thứ tự trên danh sách |
| **Trivial** | UI/cosmetic, không ảnh hưởng chức năng | Typo trong text, alignment lệch 2px |

---

## Hướng dẫn đánh Priority

| Priority | Mô tả | Action |
|----------|-------|--------|
| **High** | Cần fix ngay trong sprint hiện tại | Fix immediately |
| **Medium** | Fix trong sprint tiếp theo | Plan for next sprint |
| **Low** | Fix khi có thời gian | Backlog |

---

## Ví dụ Bug Report

### BUG-042: [Login] - Error 500 khi submit form với email chứa ký tự đặc biệt

| Field | Value |
|-------|-------|
| **Reporter** | QA Tester |
| **Date** | 30/03/2026 |
| **Severity** | Major |
| **Priority** | High |
| **Environment** | Chrome 130, macOS 15.3 |
| **Build** | v2.1.0 - Sprint 12 |
| **Module** | Authentication |

**Preconditions:**
- User đang ở trang login

**Steps to Reproduce:**
1. Navigate to `https://app.example.com/login`
2. Enter email: `user+test@email.com`
3. Enter password: `ValidPass@123`
4. Click "Login" button

**Actual Result:**
- Trang hiển thị "500 Internal Server Error"
- Console log: `Uncaught TypeError: Cannot read property 'email' of undefined`

**Expected Result:**
- Nếu email/password đúng → redirect đến Dashboard
- Nếu sai → hiển thị error message "Invalid credentials"

**Attachments:**
- [Screenshot error page]
- [Console log]
- [Network response 500]

**Additional Info:**
- Bug xảy ra 100% khi email chứa ký tự `+`
- Workaround: Dùng email không có ký tự đặc biệt
- Related: BUG-039 (email validation issue)
