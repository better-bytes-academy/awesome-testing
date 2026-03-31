# Các Câu lệnh (Prompts) Kiểm thử Trường hợp Ngoại lệ (Edge Case)
> Tiếng Anh bên dưới

## 1. Phân tích giá trị biên (Boundary Value Analysis)

```
Tạo các test case trường hợp ngoại lệ sử dụng phân tích giá trị biên cho:

Tính năng: [TÊN_TÍNH_NĂNG]
Các trường đầu vào:
- [TRƯỜNG_1]: Loại: [LOẠI], Phạm vi: [TỐI_THIỂU-TỐI_ĐA], Định dạng: [ĐỊNH_DẠNG]
- [TRƯỜNG_2]: Loại: [LOẠI], Phạm vi: [TỐI_THIỂU-TỐI_ĐA], Định dạng: [ĐỊNH_DẠNG]

Tạo test case cho:
- Các giá trị biên tối thiểu
- Các giá trị biên tối đa
- Ngay dưới mức tối thiểu (không hợp lệ)
- Ngay trên mức tối đa (không hợp lệ)
- Các giá trị biên chính xác
- Sự kết hợp các giá trị biên giữa các trường
```

## 2. Kiểm thử giá trị Null và Rỗng (Null and Empty Value Testing)

```
Tạo các test case trường hợp ngoại lệ cho việc xử lý giá trị null và rỗng:

Tính năng: [TÊN_TÍNH_NĂNG]
Các trường: [DANH_SÁCH_TẤT_CẢ_CÁC_TRƯỜNG]
Các trường bắt buộc: [DANH_SÁCH_CÁC_TRƯỜNG_BẮT_BUỘC]
Các trường tùy chọn: [DANH_SÁCH_CÁC_TRƯỜNG_TÙY_CHỌN]

Tạo test case cho:
- Giá trị null trong các trường bắt buộc
- Giá trị null trong các trường tùy chọn
- Chuỗi rỗng so với giá trị null
- Các giá trị chỉ chứa khoảng trắng
- Giá trị 0 cho các trường số
- Mảng/tập hợp rỗng
- Các tham chiếu đối tượng null
```

## 3. Xử lý ký tự đặc biệt (Special Character Handling)

```
Tạo các test case trường hợp ngoại lệ cho việc xử lý ký tự đặc biệt:

Các trường đầu vào: [DANH_SÁCH_CÁC_TRƯỜNG]
Ký tự được phép: [MÔ_TẢ_CÁC_KÝ_TỰ_ĐƯỢC_PHÉP]

Kiểm thử với:
- Các ký tự SQL injection (', --, ;)
- Các ký tự XSS (<, >, <script>)
- Các ký tự Unicode (emoji, biểu tượng đặc biệt)
- Các ký tự thoát (escape) (\n, \t, \r)
- Các ký tự duyệt thư mục (path traversal) (../, ..\)
- Các ký tự mã hóa URL (%20, %3C)
- Các ký tự điều khiển
- Các ký tự của ngôn ngữ khác nhau (tiếng Trung, tiếng Ả Rập, v.v.)
```

## 4. Đồng thời và Tình huống tranh chấp (Concurrency and Race Conditions)

```
Tạo các test case trường hợp ngoại lệ cho các hoạt động đồng thời:

Tính năng: [TÊN_TÍNH_NĂNG]
Tài nguyên dùng chung: [MÔ_TẢ_CÁC_TÀI_NGUYÊN]
Các thao tác: [DANH_SÁCH_CÁC_THAO_TÁC]

Tạo test case cho:
- Cập nhật đồng thời trên cùng một bản ghi
- Các thao tác đọc và ghi đồng thời
- Nhiều người dùng cùng thực hiện một hành động
- Các kịch bản bế tắc (Deadlock)
- Hành vi khóa tài nguyên
- Các vấn đề về mức độ cô lập giao dịch (Transaction isolation)
- Vô hiệu hóa bộ nhớ đệm (Cache invalidation) trong quá trình truy cập đồng thời
```

## 5. Kiểm thử khối lượng dữ liệu lớn (Large Data Volume Testing)

```
Tạo các test case trường hợp ngoại lệ cho khối lượng dữ liệu lớn:

Tính năng: [TÊN_TÍNH_NĂNG]
Khối lượng dữ liệu dự kiến: [KHỐI_LƯỢNG_THÔNG_THƯỜNG]

Kiểm thử với:
- Số lượng bản ghi tối đa được phép
- Vượt quá giới hạn tối đa
- Tải lên tệp lớn (giới hạn kích thước)
- Chuỗi văn bản dài (độ dài tối đa + 1)
- Số lượng lớn người dùng đồng thời
- Các thao tác hàng loạt (bulk operations) ở quy mô lớn
- Hiệu suất truy vấn cơ sở dữ liệu với tập dữ liệu lớn
- Mức tiêu thụ bộ nhớ với dữ liệu lớn
```

## 6. Các trường hợp ngoại lệ về Thời gian và Ngày tháng (Time and Date Edge Cases)

```
Tạo các test case trường hợp ngoại lệ cho việc xử lý ngày/giờ:

Tính năng: [TÊN_TÍNH_NĂNG]
Các trường Ngày/Giờ: [DANH_SÁCH_CÁC_TRƯỜNG]
Xử lý múi giờ: [CÓ/KHÔNG]

Tạo test case cho:
- Ngày của năm nhuận (29 tháng 2)
- Các ngày cuối tháng (28, 29, 30, 31)
- Chuyển đổi giờ tiết kiệm ánh sáng ban ngày (Daylight saving time)
- Chuyển đổi múi giờ
- Các ngày trong quá khứ (lịch sử)
- Các ngày trong tương lai (tương lai xa)
- Các ngày không hợp lệ (30 tháng 2, Tháng 13)
- Các biến thể về định dạng ngày tháng
- Thời điểm nửa đêm và cuối ngày
- Các hệ thống lịch khác nhau
```

## 7. Các trường hợp ngoại lệ về Mạng và Kết nối (Network and Connectivity Edge Cases)

```
Tạo các test case trường hợp ngoại lệ cho các kịch bản về mạng:

Loại ứng dụng: [WEB/DI_ĐỘNG/DESKTOP]
Phụ thuộc mạng: [DANH_SÁCH_CÁC_PHỤ_THUỘC]

Các kịch bản kiểm thử:
- Kết nối mạng chậm
- Kết nối mạng chập chờn
- Mất mạng hoàn toàn trong quá trình thao tác
- Các kịch bản hết thời gian chờ (Timeout)
- Truyền dữ liệu một phần
- Chuyển đổi mạng (từ WiFi sang mạng di động)
- Các hạn chế do proxy/tường lửa
- Lỗi phân giải tên miền (DNS)
```

## 8. Các trường hợp ngoại lệ về Chuyển đổi trạng thái (State Transition Edge Cases)

```
Tạo các test case trường hợp ngoại lệ cho việc chuyển đổi trạng thái:

Thực thể: [TÊN_THỰC_THỂ]
Các trạng thái: [DANH_SÁCH_CÁC_TRẠNG_THÁI]
Các chuyển đổi: [MÔ_TẢ_CÁC_CHUYỂN_ĐỔI_ĐƯỢC_PHÉP]

Tạo test case cho:
- Sự thay đổi trạng thái liên tục/nhanh chóng
- Các chuyển đổi trạng thái không hợp lệ
- Các kịch bản khôi phục (rollback) trạng thái
- Sửa đổi trạng thái đồng thời
- Lỗi lưu giữ (persistence) trạng thái
- Các trạng thái mồ côi (không có liên kết)
- Nỗ lực chuyển đổi vòng tròn (Circular transition)
- Các trường hợp ngoại lệ về xác thực trạng thái
```

## 9. Các trường hợp ngoại lệ về Quyền và Truy cập (Permission and Access Edge Cases)

```
Tạo các test case trường hợp ngoại lệ về ủy quyền:

Các vai trò: [DANH_SÁCH_CÁC_VAI_TRÒ]
Các tài nguyên: [DANH_SÁCH_CÁC_TÀI_NGUYÊN]
Mô hình phân quyền: [MÔ_TẢ_MÔ_HÌNH]

Các kịch bản kiểm thử:
- Các phiên (session) đã hết hạn
- Bị thu hồi quyền trong khi phiên đang hoạt động
- Bị thay đổi vai trò trong khi phiên đang hoạt động
- Cố truy cập tài nguyên sau khi đã bị xóa
- Các nỗ lực leo thang đặc quyền (Privilege escalation)
- Truy cập dữ liệu chéo giữa các tổ chức (Cross-tenant)
- Xung đột tài nguyên dùng chung
- Các trường hợp ngoại lệ về tính kế thừa quyền hạn
```

## 10. Các trường hợp ngoại lệ về Tải lên/Tải xuống tệp (File Upload/Download Edge Cases)

```
Tạo các test case trường hợp ngoại lệ cho các thao tác với tệp:

Tính năng: [TẢI_LÊN/TẢI_XUỐNG/CẢ_HAI]
Loại tệp được phép: [DANH_SÁCH_CÁC_LOẠI]
Giới hạn kích thước: [CHỈ_ĐỊNH_GIỚI_HẠN]

Tạo test case cho:
- Các tệp có kích thước 0 byte
- Các tệp có kích thước tối đa
- Các loại tệp không được hỗ trợ
- Các tệp bị hỏng (Corrupted files)
- Các tệp không có phần mở rộng
- Các tệp có nhiều phần mở rộng
- Ký tự đặc biệt trong tên tệp
- Tên tệp rất dài
- Tên tệp bị trùng lặp
- Các tệp bị nhiễm virus (nếu có bật tính năng quét)
- Tải lên không hoàn tất
- Tải lên đồng thời nhiều tệp
```

## 11. Các trường hợp ngoại lệ về Tính toán và Công thức (Calculation and Formula Edge Cases)

```
Tạo các test case trường hợp ngoại lệ cho các phép tính:

Loại tính toán: [MÔ_TẢ_PHÉP_TÍNH]
Biến đầu vào: [DANH_SÁCH_CÁC_BIẾN_VÀ_PHẠM_VI]
Đầu ra dự kiến: [MÔ_TẢ_ĐẦU_RA]

Kiểm thử với:
- Phép chia cho số 0
- Các số rất lớn (tràn số - overflow)
- Các số rất nhỏ (tràn số dưới - underflow)
- Số âm trong trường hợp mong đợi số dương
- Giới hạn về độ chính xác thập phân
- Các trường hợp ngoại lệ về làm tròn
- Các giá trị Vô cực (Infinity) và NaN (Không phải là số)
- Tính toán phần trăm ở các mức cực đoan
- Tính toán phức hợp với các giá trị biên
```

## 12. Các trường hợp ngoại lệ về Bản địa hóa và Quốc tế hóa (Localization and Internationalization Edge Cases)

```
Tạo các test case trường hợp ngoại lệ cho i18n/l10n:

Các ngôn ngữ được hỗ trợ: [DANH_SÁCH_NGÔN_NGỮ]
Các khu vực được hỗ trợ: [DANH_SÁCH_KHU_VỰC]
Các tính năng bị ảnh hưởng: [DANH_SÁCH_TÍNH_NĂNG]

Tạo test case cho:
- Các ngôn ngữ viết từ phải sang trái (tiếng Ả Rập, tiếng Do Thái)
- Các ngôn ngữ có ký tự đặc biệt
- Các trường hợp ngoại lệ về định dạng tiền tệ
- Các biến thể về định dạng số
- Sự khác biệt về định dạng ngày tháng
- Sự giãn ra/co lại của văn bản trên giao diện người dùng (UI)
- Các vấn đề về mã hóa ký tự
- Quy tắc sắp xếp theo ngôn ngữ cụ thể (Locale-specific sorting)
- Các kịch bản thiếu bản dịch
```

## 13. Các trường hợp ngoại lệ về Trình duyệt và Thiết bị (Browser and Device Edge Cases)

```
Tạo các test case trường hợp ngoại lệ về khả năng tương thích của trình duyệt/thiết bị:

Ứng dụng: [TÊN_ỨNG_DỤNG]
Nền tảng được hỗ trợ: [DANH_SÁCH_NỀN_TẢNG]

Các kịch bản kiểm thử:
- Phiên bản trình duyệt cũ nhất được hỗ trợ
- Trình duyệt bị tắt JavaScript
- Trình duyệt bị tắt Cookie
- Độ phân giải màn hình rất nhỏ
- Độ phân giải màn hình rất lớn
- Tương tác cảm ứng so với chuột
- Các mức thu phóng (zoom) của trình duyệt (50%, 200%)
- Hành vi của nút quay lại/tiến tới (back/forward) trên trình duyệt
- Mở nhiều tab/cửa sổ
- Chế độ Riêng tư/Ẩn danh
```

## 14. Các trường hợp ngoại lệ về Tích hợp (Integration Edge Cases)

```
Tạo các test case trường hợp ngoại lệ cho việc tích hợp hệ thống:

Loại tích hợp: [API/CƠ_SỞ_DỮ_LIỆU/TỆP/MESSAGE_QUEUE]
Hệ thống bên ngoài: [TÊN_HỆ_THỐNG]
Trao đổi dữ liệu: [MÔ_TẢ_LUỒNG_DỮ_LIỆU]

Tạo test case cho:
- Hệ thống bên ngoài không khả dụng
- Các phản hồi không đúng định dạng (malformed) từ hệ thống bên ngoài
- Các kiểu dữ liệu không mong muốn
- Thiếu các trường bắt buộc trong phản hồi
- Hết thời gian chờ (Timeout) trong quá trình gọi tích hợp
- Các kịch bản thành công một phần
- Các trường hợp ngoại lệ về logic thử lại (Retry logic)
- Kích hoạt cơ chế ngắt mạch (Circuit breaker)
- Lỗi không khớp phiên bản giữa các hệ thống
```

## 15. Các trường hợp ngoại lệ về Tìm kiếm và Lọc (Search and Filter Edge Cases)

```
Tạo các test case trường hợp ngoại lệ cho tính năng tìm kiếm:

Loại tìm kiếm: [CƠ_BẢN/NÂNG_CAO/TOÀN_VĂN_BẢN]
Các trường có thể tìm kiếm: [DANH_SÁCH_CÁC_TRƯỜNG]

Các kịch bản kiểm thử:
- Truy vấn tìm kiếm trống
- Tìm kiếm bằng một ký tự duy nhất
- Truy vấn tìm kiếm rất dài
- Ký tự đặc biệt trong từ khóa tìm kiếm
- Tìm kiếm chỉ với các khoảng trắng
- Các trường hợp ngoại lệ về phân biệt chữ hoa/chữ thường
- Xử lý các ký tự đại diện (wildcard)
- Các trường hợp ngoại lệ của toán tử Boolean (AND, OR, NOT)
- Phân trang kết quả tìm kiếm ở các mốc biên
- Kịch bản không tìm thấy kết quả nào
- Kịch bản tất cả các kết quả đều khớp
```

---

## Mẹo Kiểm thử các Trường hợp Ngoại lệ

1. **Suy nghĩ Tiêu cực (Think Negatively)**: Luôn tự hỏi điều gì có thể xảy ra sai sót.
2. **Kết hợp các Điều kiện (Combine Conditions)**: Thử nghiệm nhiều trường hợp ngoại lệ cùng một lúc.
3. **Dữ liệu Thực tế (Real-World Data)**: Sử dụng các dữ liệu ngoại lệ thực tế tương tự như môi trường production.
4. **Tự động hóa (Automate)**: Các trường hợp ngoại lệ là đối tượng hoàn hảo cho kiểm thử tự động.
5. **Lập Tài liệu (Document)**: Ghi chép lại những trường hợp ngoại lệ được phát hiện trong môi trường production.
6. **Tập trung vào Bảo mật (Security Focus)**: Nhiều trường hợp ngoại lệ tiềm ẩn những nguy cơ về bảo mật.
7. **Hiệu suất (Performance)**: Các trường hợp biên thường làm bộc lộ các vấn đề về hiệu năng.

## Danh sách Kiểm tra (Checklist) Các Danh mục Ngoại lệ Phổ biến

- [ ] Các giá trị biên (tối thiểu, tối đa, ngay ngoài giới hạn)
- [ ] Dữ liệu Null, rỗng và bị thiếu
- [ ] Ký tự đặc biệt và các vấn đề mã hóa
- [ ] Xử lý đồng thời và thời gian (timing)
- [ ] Khối lượng dữ liệu lớn và các giới hạn
- [ ] Các trường hợp ngoại lệ về Ngày/Giờ
- [ ] Mạng lưới và kết nối
- [ ] Chuyển đổi trạng thái
- [ ] Quyền hạn và truy cập
- [ ] Thao tác với tệp
- [ ] Tính toán và công thức
- [ ] Bản địa hóa (Localization)
- [ ] Tương thích trình duyệt/thiết bị
- [ ] Các điểm tích hợp
- [ ] Tìm kiếm và bộ lọc
----
# Edge Case Testing Prompts

## 1. Boundary Value Analysis

```
Generate edge case test cases using boundary value analysis for:

Feature: [FEATURE_NAME]
Input Fields:
- [FIELD_1]: Type: [TYPE], Range: [MIN-MAX], Format: [FORMAT]
- [FIELD_2]: Type: [TYPE], Range: [MIN-MAX], Format: [FORMAT]

Create test cases for:
- Minimum boundary values
- Maximum boundary values
- Just below minimum (invalid)
- Just above maximum (invalid)
- Exact boundary values
- Combination of boundary values across fields
```

## 2. Null and Empty Value Testing

```
Generate edge case test cases for null and empty value handling:

Feature: [FEATURE_NAME]
Fields: [LIST_ALL_FIELDS]
Required Fields: [LIST_REQUIRED_FIELDS]
Optional Fields: [LIST_OPTIONAL_FIELDS]

Create test cases for:
- Null values in required fields
- Null values in optional fields
- Empty strings vs null
- Whitespace-only values
- Zero values for numeric fields
- Empty arrays/collections
- Null object references
```

## 3. Special Character Handling

```
Create edge case test cases for special character handling:

Input Fields: [LIST_FIELDS]
Allowed Characters: [DESCRIBE_ALLOWED_CHARS]

Test with:
- SQL injection characters (', --, ;)
- XSS characters (<, >, <script>)
- Unicode characters (emoji, special symbols)
- Escape characters (\n, \t, \r)
- Path traversal characters (../, ..\)
- URL encoding characters (%20, %3C)
- Control characters
- Different language characters (Chinese, Arabic, etc.)
```

## 4. Concurrency and Race Conditions

```
Generate edge case test cases for concurrent operations:

Feature: [FEATURE_NAME]
Shared Resources: [DESCRIBE_RESOURCES]
Operations: [LIST_OPERATIONS]

Create test cases for:
- Simultaneous updates to same record
- Concurrent read and write operations
- Multiple users performing same action
- Deadlock scenarios
- Resource locking behavior
- Transaction isolation issues
- Cache invalidation during concurrent access
```

## 5. Large Data Volume Testing

```
Create edge case test cases for large data volumes:

Feature: [FEATURE_NAME]
Expected Data Volume: [NORMAL_VOLUME]

Test with:
- Maximum allowed records
- Beyond maximum limit
- Large file uploads (size limits)
- Long text strings (max length + 1)
- Large number of concurrent users
- Bulk operations at scale
- Database query performance with large datasets
- Memory consumption with large data
```

## 6. Time and Date Edge Cases

```
Generate edge case test cases for date/time handling:

Feature: [FEATURE_NAME]
Date/Time Fields: [LIST_FIELDS]
Timezone Handling: [YES/NO]

Create test cases for:
- Leap year dates (Feb 29)
- End of month dates (28, 29, 30, 31)
- Daylight saving time transitions
- Timezone conversions
- Past dates (historical)
- Future dates (far future)
- Invalid dates (Feb 30, Month 13)
- Date format variations
- Midnight and end-of-day times
- Different calendar systems
```

## 7. Network and Connectivity Edge Cases

```
Create edge case test cases for network scenarios:

Application Type: [WEB/MOBILE/DESKTOP]
Network Dependencies: [LIST_DEPENDENCIES]

Test scenarios:
- Slow network connection
- Intermittent connectivity
- Complete network loss during operation
- Timeout scenarios
- Partial data transmission
- Network switch (WiFi to cellular)
- Proxy/firewall restrictions
- DNS resolution failures
```

## 8. State Transition Edge Cases

```
Generate edge case test cases for state transitions:

Entity: [ENTITY_NAME]
States: [LIST_STATES]
Transitions: [DESCRIBE_ALLOWED_TRANSITIONS]

Create test cases for:
- Rapid state changes
- Invalid state transitions
- State rollback scenarios
- Concurrent state modifications
- State persistence failures
- Orphaned states
- Circular transition attempts
- State validation edge cases
```

## 9. Permission and Access Edge Cases

```
Create edge case test cases for authorization:

Roles: [LIST_ROLES]
Resources: [LIST_RESOURCES]
Permission Model: [DESCRIBE_MODEL]

Test scenarios:
- Expired sessions
- Revoked permissions during active session
- Role changes during active session
- Accessing resources after deletion
- Privilege escalation attempts
- Cross-tenant data access
- Shared resource conflicts
- Permission inheritance edge cases
```

## 10. File Upload/Download Edge Cases

```
Generate edge case test cases for file operations:

Feature: [UPLOAD/DOWNLOAD/BOTH]
Allowed File Types: [LIST_TYPES]
Size Limits: [SPECIFY_LIMITS]

Create test cases for:
- Zero-byte files
- Maximum size files
- Unsupported file types
- Corrupted files
- Files with no extension
- Files with multiple extensions
- Special characters in filename
- Very long filenames
- Duplicate filenames
- Virus-infected files (if scanning enabled)
- Incomplete uploads
- Simultaneous uploads
```

## 11. Calculation and Formula Edge Cases

```
Create edge case test cases for calculations:

Calculation Type: [DESCRIBE_CALCULATION]
Input Variables: [LIST_VARIABLES_AND_RANGES]
Expected Output: [DESCRIBE_OUTPUT]

Test with:
- Division by zero
- Very large numbers (overflow)
- Very small numbers (underflow)
- Negative numbers where positive expected
- Decimal precision limits
- Rounding edge cases
- Infinity and NaN values
- Percentage calculations at extremes
- Compound calculations with edge values
```

## 12. Localization and Internationalization Edge Cases

```
Generate edge case test cases for i18n/l10n:

Supported Languages: [LIST_LANGUAGES]
Supported Regions: [LIST_REGIONS]
Features Affected: [LIST_FEATURES]

Create test cases for:
- Right-to-left languages (Arabic, Hebrew)
- Languages with special characters
- Currency formatting edge cases
- Number formatting variations
- Date format differences
- Text expansion/contraction in UI
- Character encoding issues
- Locale-specific sorting
- Translation missing scenarios
```

## 13. Browser and Device Edge Cases

```
Create edge case test cases for browser/device compatibility:

Application: [APP_NAME]
Supported Platforms: [LIST_PLATFORMS]

Test scenarios:
- Oldest supported browser version
- Browser with JavaScript disabled
- Browser with cookies disabled
- Very small screen resolutions
- Very large screen resolutions
- Touch vs mouse interactions
- Browser zoom levels (50%, 200%)
- Browser back/forward button behavior
- Multiple tabs/windows
- Private/incognito mode
```

## 14. Integration Edge Cases

```
Generate edge case test cases for system integration:

Integration Type: [API/DATABASE/FILE/MESSAGE_QUEUE]
External System: [SYSTEM_NAME]
Data Exchange: [DESCRIBE_DATA_FLOW]

Create test cases for:
- External system unavailable
- Malformed responses from external system
- Unexpected data types
- Missing required fields in response
- Timeout during integration call
- Partial success scenarios
- Retry logic edge cases
- Circuit breaker activation
- Version mismatch between systems
```

## 15. Search and Filter Edge Cases

```
Create edge case test cases for search functionality:

Search Type: [BASIC/ADVANCED/FULL_TEXT]
Searchable Fields: [LIST_FIELDS]

Test scenarios:
- Empty search query
- Single character search
- Very long search query
- Special characters in search
- Search with only spaces
- Case sensitivity edge cases
- Wildcard character handling
- Boolean operator edge cases
- Search result pagination at boundaries
- No results found scenarios
- All results match scenarios
```

## Tips for Edge Case Testing

1. **Think Negatively**: Consider what could go wrong
2. **Combine Conditions**: Test multiple edge cases together
3. **Real-World Data**: Use actual production-like edge data
4. **Automate**: Edge cases are perfect for automated testing
5. **Document**: Record edge cases found in production
6. **Security Focus**: Many edge cases have security implications
7. **Performance**: Edge cases often reveal performance issues

## Common Edge Case Categories Checklist

- [ ] Boundary values (min, max, just outside)
- [ ] Null, empty, and missing data
- [ ] Special characters and encoding
- [ ] Concurrency and timing
- [ ] Large volumes and limits
- [ ] Date/time edge cases
- [ ] Network and connectivity
- [ ] State transitions
- [ ] Permissions and access
- [ ] File operations
- [ ] Calculations and formulas
- [ ] Localization
- [ ] Browser/device compatibility
- [ ] Integration points
- [ ] Search and filtering

> Tham khảo [link](https://github.com/tayyabakmal1/qa-prompt-library/blob/main/manual-qa/test-case-creation/edge-case-prompts.md)