# API Testing Interview Questions

> Câu hỏi phỏng vấn API Testing — từ cơ bản đến nâng cao.

---

## 🟢 Cơ bản

### 1. API là gì?
**Trả lời**: API (Application Programming Interface) là giao diện cho phép các phần mềm giao tiếp với nhau. Trong web, API thường là REST API hoặc GraphQL.

### 2. REST API là gì? Các HTTP Methods chính?
**Trả lời**: REST (Representational State Transfer) là architectural style cho web APIs.

| Method | Mục đích | Idempotent |
|--------|---------|-----------|
| GET | Lấy dữ liệu | ✅ |
| POST | Tạo mới | ❌ |
| PUT | Cập nhật toàn bộ | ✅ |
| PATCH | Cập nhật một phần | ❌ |
| DELETE | Xóa | ✅ |

### 3. HTTP Status Codes quan trọng?
**Trả lời**:
- **2xx**: Success (200 OK, 201 Created, 204 No Content)
- **3xx**: Redirection (301 Moved, 302 Found)
- **4xx**: Client Error (400 Bad Request, 401 Unauthorized, 403 Forbidden, 404 Not Found)
- **5xx**: Server Error (500 Internal Server Error, 502 Bad Gateway, 503 Service Unavailable)

### 4. Authentication vs Authorization?
**Trả lời**:
- **Authentication**: Xác minh "bạn là ai?" (Login)
- **Authorization**: Xác minh "bạn có quyền gì?" (Phân quyền)

### 5. Các phương thức Authentication phổ biến?
**Trả lời**: Basic Auth, API Key, Bearer Token (JWT), OAuth 2.0, Session/Cookie.

---

## 🟡 Trung cấp

### 6. API Testing cần verify những gì?
**Trả lời**:
- **Status Code**: Đúng với expected
- **Response Body**: Data đúng format và giá trị
- **Headers**: Content-Type, Authorization
- **Response Time**: Trong giới hạn chấp nhận
- **Error Handling**: Response lỗi có ý nghĩa
- **Schema Validation**: Response đúng schema

### 7. PUT vs PATCH khác nhau thế nào?
**Trả lời**:
- **PUT**: Cập nhật toàn bộ resource, cần gửi tất cả fields
- **PATCH**: Cập nhật một phần, chỉ gửi fields cần thay đổi

### 8. Idempotent nghĩa là gì? Tại sao quan trọng?
**Trả lời**: Idempotent = gọi nhiều lần cho cùng kết quả. GET, PUT, DELETE là idempotent. POST không phải. Quan trọng vì: retry mechanism, network failures.

### 9. REST vs GraphQL?
**Trả lời**:

| Tiêu chí | REST | GraphQL |
|---------|------|---------|
| Endpoint | Nhiều endpoints | Single endpoint |
| Data fetching | Fixed response | Client chọn fields |
| Over-fetching | Có thể xảy ra | Không |
| Caching | Dễ (HTTP caching) | Phức tạp hơn |
| Learning curve | Thấp | Trung bình |

### 10. Contract Testing là gì?
**Trả lời**: Kiểm tra rằng API provider và consumer tuân thủ một "hợp đồng" (contract) đã thống nhất. Công cụ: Pact, JSON Schema. Quan trọng trong microservices.

---

## 🔴 Nâng cao

### 11. Thiết kế test strategy cho API testing?
**Trả lời**:
1. **Positive testing**: Happy path với valid data
2. **Negative testing**: Invalid data, missing fields
3. **Boundary testing**: Min/max values
4. **Authentication/Authorization**: Token expired, wrong role
5. **Performance**: Response time, concurrent requests
6. **Security**: SQL injection, XSS qua API
7. **Integration**: Dependencies giữa các APIs
8. **Error handling**: Error messages, error codes

### 12. Rate Limiting testing?
**Trả lời**: Verify API xử lý đúng khi:
- Vượt quá rate limit → trả 429 Too Many Requests
- Headers: X-RateLimit-Limit, X-RateLimit-Remaining, Retry-After
- Reset time chính xác

### 13. API Versioning strategies?
**Trả lời**:
- **URI**: `/api/v1/users`, `/api/v2/users`
- **Header**: `Accept: application/vnd.api.v1+json`
- **Query Param**: `/api/users?version=1`

### 14. Pagination testing cần verify gì?
**Trả lời**:
- Total count chính xác
- Page size đúng
- Next/Previous links hoạt động
- Last page có đúng số items
- Boundary: page=0, page=-1, page=999999
- Sort order consistent across pages

---

## 📚 Tham khảo

- [REST API Tutorial](https://restfulapi.net/)
- [Postman Learning Center](https://learning.postman.com/)
