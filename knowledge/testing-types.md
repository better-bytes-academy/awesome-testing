# Testing Types

> Phân loại các loại kiểm thử phần mềm — từ Functional đến Non-functional.

---

## 📌 Mục lục

- [Tổng quan phân loại](#tổng-quan-phân-loại)
- [Functional Testing](#functional-testing)
- [Non-Functional Testing](#non-functional-testing)
- [Maintenance Testing](#maintenance-testing)
- [Bảng so sánh](#bảng-so-sánh)

---

## Tổng quan phân loại

```
Software Testing
├── Functional Testing
│   ├── Unit Testing
│   ├── Integration Testing
│   ├── System Testing
│   ├── Acceptance Testing
│   ├── Smoke Testing
│   ├── Sanity Testing
│   ├── Regression Testing
│   ├── Exploratory Testing
│   └── Ad-hoc Testing
│
├── Non-Functional Testing
│   ├── Performance Testing
│   ├── Load Testing
│   ├── Stress Testing
│   ├── Security Testing
│   ├── Usability Testing
│   ├── Compatibility Testing
│   ├── Accessibility Testing
│   └── Reliability Testing
│
└── Maintenance Testing
    ├── Confirmation Testing (Re-testing)
    ├── Regression Testing
    └── Impact Analysis
```

---

## Functional Testing

### Unit Testing
- **Mô tả**: Kiểm thử từng đơn vị code nhỏ nhất (function, method)
- **Ai thực hiện**: Developer
- **Công cụ**: JUnit, NUnit, pytest, Jest

### Integration Testing
- **Mô tả**: Kiểm thử sự tương tác giữa các module/component
- **Phương pháp**:
  - **Big Bang**: Tích hợp tất cả cùng lúc
  - **Top-Down**: Từ module cao nhất xuống
  - **Bottom-Up**: Từ module thấp nhất lên
  - **Sandwich/Hybrid**: Kết hợp Top-Down và Bottom-Up

### System Testing
- **Mô tả**: Kiểm thử toàn bộ hệ thống hoàn chỉnh
- **Ai thực hiện**: QA Team
- **Bao gồm**: Functional + Non-functional testing

### Acceptance Testing
- **Mô tả**: Kiểm thử để xác nhận hệ thống đáp ứng yêu cầu business
- **Phân loại**:
  - **UAT (User Acceptance Testing)**: Người dùng cuối thực hiện
  - **Alpha Testing**: Tại môi trường dev
  - **Beta Testing**: Tại môi trường người dùng thực

### Smoke Testing
- **Mô tả**: Kiểm thử nhanh các chức năng cơ bản nhất
- **Mục đích**: Xác nhận build ổn định, đủ điều kiện test tiếp
- **Ví dụ**: Login được không? Trang chủ load được không?

### Sanity Testing
- **Mô tả**: Kiểm thử nhanh sau khi sửa lỗi hoặc thay đổi nhỏ
- **Mục đích**: Xác nhận sửa lỗi đúng, không ảnh hưởng xung quanh

### Regression Testing
- **Mô tả**: Kiểm thử lại các chức năng hiện có sau khi có thay đổi
- **Mục đích**: Đảm bảo thay đổi mới không gây ra lỗi mới
- **Công cụ**: Selenium, Playwright, Cypress

### Exploratory Testing
- **Mô tả**: Kiểm thử dựa trên kinh nghiệm, không theo script cố định
- **Khi nào dùng**: Khi cần khám phá nhanh, hiểu hệ thống
- **Kỹ thuật**: Session-based Testing, Charter-based Testing

### Ad-hoc Testing
- **Mô tả**: Kiểm thử không có kế hoạch, không có tài liệu
- **Khi nào dùng**: Khi muốn tìm lỗi bất ngờ
- **Khác biệt với Exploratory**: Không có cấu trúc hay mục tiêu cụ thể

---

## Non-Functional Testing

### Performance Testing
- **Mô tả**: Đánh giá hiệu suất hệ thống (tốc độ, thời gian phản hồi)
- **Công cụ**: JMeter, k6, Gatling, Locust

### Load Testing
- **Mô tả**: Kiểm tra hệ thống với số lượng người dùng tăng dần
- **Mục đích**: Xác định giới hạn tải của hệ thống

### Stress Testing
- **Mô tả**: Đẩy hệ thống vượt quá giới hạn để xem cách ứng xử
- **Mục đích**: Xác định breaking point và khả năng recovery

### Security Testing
- **Mô tả**: Tìm kiếm lỗ hổng bảo mật
- **Bao gồm**: SQL Injection, XSS, CSRF, Authentication, Authorization
- **Công cụ**: OWASP ZAP, Burp Suite, Nmap

### Usability Testing
- **Mô tả**: Đánh giá trải nghiệm người dùng (UX)
- **Tiêu chí**: Dễ dùng, trực quan, hiệu quả

### Compatibility Testing
- **Mô tả**: Kiểm tra tương thích trên nhiều môi trường
- **Bao gồm**: Browser, OS, Device, Resolution

### Accessibility Testing
- **Mô tả**: Kiểm tra khả năng tiếp cận cho người khuyết tật
- **Tiêu chuẩn**: WCAG 2.1/2.2, ADA, Section 508
- **Công cụ**: axe, WAVE, Lighthouse

### Reliability Testing
- **Mô tả**: Đánh giá độ tin cậy của hệ thống theo thời gian
- **Bao gồm**: MTBF (Mean Time Between Failures), MTTR (Mean Time To Repair)

---

## Maintenance Testing

### Confirmation Testing (Re-testing)
- **Mô tả**: Kiểm tra lại bug đã được sửa
- **Mục đích**: Xác nhận fix đúng

### Regression Testing
- **Mô tả**: Kiểm tra các chức năng liên quan sau khi sửa lỗi
- **Mục đích**: Đảm bảo không có side-effect

### Impact Analysis
- **Mô tả**: Phân tích tác động của thay đổi để xác định phạm vi test
- **Mục đích**: Tối ưu effort kiểm thử

---

## Bảng so sánh

### Smoke vs Sanity

| Tiêu chí | Smoke Testing | Sanity Testing |
|---------|--------------|---------------|
| **Phạm vi** | Rộng — toàn bộ chức năng cơ bản | Hẹp — chức năng cụ thể |
| **Mục đích** | Build có ổn định không? | Fix lỗi có đúng không? |
| **Thời điểm** | Sau mỗi build mới | Sau khi fix bug cụ thể |
| **Script** | Có thể scripted | Thường unscripted |

### Re-testing vs Regression

| Tiêu chí | Re-testing | Regression Testing |
|---------|-----------|-------------------|
| **Phạm vi** | Chỉ bug đã fix | Các chức năng liên quan |
| **Mục đích** | Xác nhận fix đúng | Đảm bảo không có lỗi mới |
| **Tự động hóa** | Ít khi | Nên tự động hóa |

---

## 📚 Tham khảo

- [ISTQB Foundation Level Syllabus](https://www.istqb.org/)
- [Software Testing Types - Guru99](https://www.guru99.com/types-of-software-testing.html)
