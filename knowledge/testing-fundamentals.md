# Testing Fundamentals

> Các khái niệm cơ bản trong kiểm thử phần mềm mà mọi QA Engineer cần nắm vững.

---

## 📌 Mục lục

- [Kiểm thử phần mềm là gì?](#kiểm-thử-phần-mềm-là-gì)
- [Tại sao cần kiểm thử?](#tại-sao-cần-kiểm-thử)
- [Các nguyên tắc kiểm thử (7 Principles)](#các-nguyên-tắc-kiểm-thử)
- [Quy trình kiểm thử (Test Process)](#quy-trình-kiểm-thử)
- [Các cấp độ kiểm thử (Test Levels)](#các-cấp-độ-kiểm-thử)
- [Verification vs Validation](#verification-vs-validation)
- [Testing Pyramid](#testing-pyramid)
- [Thuật ngữ quan trọng](#thuật-ngữ-quan-trọng)

---

## Kiểm thử phần mềm là gì?

Kiểm thử phần mềm (Software Testing) là quá trình đánh giá và xác minh rằng một sản phẩm phần mềm hoạt động đúng như mong đợi. Mục tiêu chính:

- Tìm ra lỗi (defects/bugs)
- Đảm bảo chất lượng sản phẩm
- Xác nhận yêu cầu được đáp ứng
- Giảm rủi ro khi phát hành

---

## Tại sao cần kiểm thử?

| Lý do | Giải thích |
|-------|-----------|
| **Tiết kiệm chi phí** | Phát hiện lỗi sớm giúp giảm chi phí sửa chữa |
| **Đảm bảo chất lượng** | Sản phẩm đáp ứng yêu cầu người dùng |
| **Bảo mật** | Phát hiện lỗ hổng bảo mật trước khi bị khai thác |
| **Sự hài lòng** | Người dùng nhận được trải nghiệm tốt |
| **Tuân thủ** | Đáp ứng các tiêu chuẩn và quy định |

---

## Các nguyên tắc kiểm thử

### 7 nguyên tắc kiểm thử theo ISTQB:

1. **Testing shows the presence of defects, not their absence** — Kiểm thử chỉ cho thấy lỗi tồn tại, không chứng minh phần mềm không có lỗi
2. **Exhaustive testing is impossible** — Kiểm thử toàn diện là không thể
3. **Early testing saves time and money** — Kiểm thử sớm tiết kiệm thời gian và chi phí
4. **Defects cluster together** — Lỗi có xu hướng tập trung
5. **Beware of the pesticide paradox** — Cẩn thận với nghịch lý thuốc trừ sâu
6. **Testing is context dependent** — Kiểm thử phụ thuộc vào ngữ cảnh
7. **Absence-of-errors is a fallacy** — Không có lỗi không có nghĩa là phần mềm tốt

---

## Quy trình kiểm thử

```
Test Planning → Test Analysis → Test Design → Test Implementation → Test Execution → Test Completion
```

| Giai đoạn | Hoạt động chính |
|-----------|----------------|
| **Test Planning** | Xác định phạm vi, mục tiêu, chiến lược |
| **Test Analysis** | Phân tích yêu cầu, xác định điều kiện test |
| **Test Design** | Thiết kế test case, test data |
| **Test Implementation** | Chuẩn bị môi trường, test scripts |
| **Test Execution** | Thực thi test, ghi nhận kết quả |
| **Test Completion** | Tổng kết, báo cáo, đánh giá |

---

## Các cấp độ kiểm thử

| Cấp độ | Mô tả | Ai thực hiện |
|--------|-------|-------------|
| **Unit Testing** | Kiểm thử từng đơn vị code riêng lẻ | Developer |
| **Integration Testing** | Kiểm thử tích hợp giữa các module | Developer / QA |
| **System Testing** | Kiểm thử toàn bộ hệ thống | QA Team |
| **Acceptance Testing** | Kiểm thử chấp nhận bởi người dùng | End User / PO |

---

## Verification vs Validation

| Tiêu chí | Verification | Validation |
|---------|-------------|-----------|
| **Câu hỏi** | "Are we building the product right?" | "Are we building the right product?" |
| **Mục đích** | Kiểm tra sản phẩm đúng spec | Kiểm tra sản phẩm đáp ứng nhu cầu |
| **Phương pháp** | Review, Inspection, Walkthrough | Testing, Demo, UAT |
| **Thời điểm** | Trong quá trình phát triển | Sau khi phát triển |

---

## Testing Pyramid

```
        /‾‾‾‾‾‾‾‾‾\
       /   E2E     \        ← Ít test, chi phí cao
      /   Tests     \
     /‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾\
    /  Integration     \     ← Vừa phải
   /    Tests           \
  /‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾\
 /     Unit Tests          \  ← Nhiều test, chi phí thấp
/___________________________\
```

- **Unit Tests**: Nhanh, rẻ, chạy nhiều — chiếm đa số
- **Integration Tests**: Kiểm tra tương tác giữa các thành phần
- **E2E Tests**: Mô phỏng hành vi người dùng thực tế — ít nhưng quan trọng

---

## Thuật ngữ quan trọng

| Thuật ngữ | Định nghĩa |
|-----------|-----------|
| **Bug / Defect** | Lỗi trong phần mềm |
| **Test Case** | Một tập hợp điều kiện để kiểm tra một chức năng |
| **Test Suite** | Tập hợp các test case |
| **Test Plan** | Tài liệu mô tả phạm vi và cách tiếp cận kiểm thử |
| **Test Data** | Dữ liệu dùng để thực thi test |
| **Test Environment** | Môi trường thực thi kiểm thử |
| **Regression Testing** | Kiểm thử lại để đảm bảo thay đổi không gây lỗi mới |
| **Smoke Testing** | Kiểm thử nhanh các chức năng cơ bản |
| **Sanity Testing** | Kiểm thử nhanh sau khi sửa lỗi cụ thể |
| **Severity** | Mức độ nghiêm trọng của lỗi |
| **Priority** | Mức độ ưu tiên sửa lỗi |
| **SLA** | Service Level Agreement — cam kết mức dịch vụ |

---

## 📚 Tham khảo

- [ISTQB Foundation Level Syllabus](https://www.istqb.org/)
- [Software Testing Help](https://www.softwaretestinghelp.com/)
- [Guru99 - Software Testing](https://www.guru99.com/software-testing.html)
