# Project-Software---Testing

# Manual Testing – ParaBank

## 1. Giới thiệu dự án

Dự án thực hành kiểm thử phần mềm website **ParaBank**, một hệ thống mô phỏng dịch vụ ngân hàng trực tuyến được sử dụng cho mục đích học tập và thực hành kiểm thử phần mềm.

Mục tiêu của dự án là áp dụng **Manual Testing** và **Functional Testing** để kiểm tra các chức năng, xây dựng Test Case, thực thi kiểm thử, ghi nhận kết quả và quản lý Bug.

---

## 2. Thông tin ứng dụng

- **Tên ứng dụng:** ParaBank
- **Loại hệ thống:** Online Banking Demo
- **URL:** https://parabank.parasoft.com/parabank/

ParaBank mô phỏng các nghiệp vụ cơ bản của ngân hàng trực tuyến như đăng ký tài khoản, đăng nhập, mở tài khoản, chuyển tiền, thanh toán hóa đơn, tra cứu giao dịch và quản lý thông tin khách hàng.

### Phạm vi kiểm thử

Dự án tập trung kiểm thử 3 chức năng:

- Register
- Open New Account
- Bill Pay

---

## 3. Mục tiêu kiểm thử

- Kiểm tra hoạt động của các chức năng trong phạm vi dự án.
- Kiểm tra hệ thống xử lý dữ liệu hợp lệ và không hợp lệ.
- Kiểm tra việc Validate dữ liệu đầu vào.
- Phát hiện và ghi nhận các lỗi trong quá trình kiểm thử.
- Theo dõi và quản lý Bug.
- Tổng hợp và đánh giá kết quả kiểm thử.

---

## 4. Phạm vi kiểm thử

### 4.1. Register

Kiểm thử chức năng đăng ký tài khoản:

- Kiểm tra thông tin bắt buộc.
- Đăng ký với dữ liệu hợp lệ.
- Kiểm tra Username và Password.
- Kiểm tra Confirm Password.
- Kiểm tra Username đã tồn tại.
- Kiểm tra dữ liệu chứa khoảng trắng.
- Kiểm tra ký tự đặc biệt.
- Kiểm tra Phone Number và Zip Code.

**Số lượng: 20 Test Case**

### 4.2. Open New Account

Kiểm thử chức năng mở tài khoản mới:

- Mở tài khoản Checking.
- Mở tài khoản Savings.
- Kiểm tra danh sách loại tài khoản.
- Kiểm tra tài khoản nguồn.
- Kiểm tra tài khoản sau khi tạo.
- Kiểm tra loại tài khoản sau khi tạo.

**Số lượng: 6 Test Case**

### 4.3. Bill Pay

Kiểm thử chức năng thanh toán hóa đơn:

- Kiểm tra Payee Name.
- Kiểm tra Address, City, State, Zip Code.
- Kiểm tra Phone Number.
- Kiểm tra Account Number và Verify Account.
- Kiểm tra Amount.
- Kiểm tra số tiền bằng 0.
- Kiểm tra số tiền âm.
- Kiểm tra số tiền vượt quá số dư.
- Kiểm tra dữ liệu không hợp lệ.
- Kiểm tra dữ liệu chứa ký tự đặc biệt.

**Số lượng: 19 Test Case**

### 4.4. Ngoài phạm vi

- Login
- Transfer Funds
- Find Transactions
- Request Loan
- Update Contact Info

Không thực hiện:

- Performance Testing
- Security Testing
- Load Testing
- Compatibility Testing
- Source Code Testing
- Database Testing

---

## 5. Phương pháp kiểm thử

Dự án sử dụng **Manual Testing** kết hợp **Functional Testing**.

Quy trình thực hiện:

```text
Phân tích yêu cầu
       ↓
Xây dựng Test Case
       ↓
Chuẩn bị Test Data
       ↓
Thực thi Test Case
       ↓
Ghi nhận Actual Result
       ↓
Pass / Fail
       ↓
Ghi nhận Bug
       ↓
Theo dõi Bug trên GitHub Issues
## 6. Test Case

Tổng cộng **45 Test Case** được xây dựng và thực thi.

### Phân bổ Test Case

| Module | Số lượng |
|---|---:|
| Register | 20 |
| Open New Account | 6 |
| Bill Pay | 19 |
| **Tổng cộng** | **45** |

Các Test Case được xây dựng nhằm kiểm tra cả dữ liệu hợp lệ và không hợp lệ, tập trung vào chức năng và validation của hệ thống.

---

## 7. Quản lý Test Case

Test Case được xây dựng và quản lý trên **Testiny**.

Các nội dung thực hiện:

- Thiết lập Test Case ID.
- Mô tả điều kiện kiểm thử.
- Chuẩn bị Test Data.
- Xác định Expected Result.
- Thực thi Test Case.
- Ghi nhận Actual Result.
- Cập nhật trạng thái Pass/Fail.
- Tổng hợp kết quả Test Run.

---

## 8. Kết quả kiểm thử

| Kết quả | Số lượng | Tỷ lệ |
|---|---:|---:|
| Passed | 33 | 73,3% |
| Failed | 12 | 26,7% |
| **Tổng cộng** | **45** | **100%** |

Kết quả kiểm thử:

- **33 Test Case Passed**
- **12 Test Case Failed**

Các Test Case Failed được sử dụng để ghi nhận và quản lý Bug.

---

## 9. Quản lý Bug

Các Bug được phát hiện trong quá trình kiểm thử được ghi nhận và theo dõi bằng **GitHub Issues**.

Mỗi Bug Report bao gồm:

- Bug ID
- Summary
- Steps to Reproduce
- Expected Result
- Actual Result
- Severity
- Status

**Tổng cộng: 12 Bug**

---

## 10. Phân loại Bug

| Module | Số Bug |
|---|---:|
| Register | 3 |
| Bill Pay | 9 |
| **Tổng cộng** | **12** |

Các lỗi phát hiện chủ yếu liên quan đến việc hệ thống xử lý dữ liệu đầu vào không hợp lệ và chưa kiểm tra đầy đủ các trường thông tin.

---

## 11. Công cụ sử dụng

- **Testiny:** Quản lý và thực thi Test Case.
- **GitHub Issues:** Ghi nhận và theo dõi Bug.
- **Google Chrome:** Môi trường thực hiện kiểm thử.
- **Microsoft Word:** Tổng hợp và trình bày báo cáo.

---

## 12. Kỹ năng thực hành

Thông qua dự án, em đã thực hành:

- Phân tích yêu cầu và chức năng.
- Thiết kế Test Case.
- Manual Testing.
- Functional Testing.
- Kiểm thử dữ liệu hợp lệ và không hợp lệ.
- Thực thi Test Case.
- Phân tích kết quả kiểm thử.
- Viết Bug Report.
- Phân loại Severity và Status.
- Quản lý Bug bằng GitHub Issues.
- Sử dụng Testiny để quản lý Test Case và Test Run.

---

## 13. Minh chứng dự án

Repository bao gồm các minh chứng cho quá trình kiểm thử:

- Test Case trên Testiny.
- Test Run và kết quả kiểm thử.
- Kết quả Passed/Failed.
- Bug Report.
- GitHub Issues.
- Hình ảnh minh chứng quá trình thực hiện Test Case.

---

## 14. Tổng kết

Dự án giúp thực hành quy trình kiểm thử phần mềm từ:

**Phân tích yêu cầu → Xây dựng Test Case → Thực thi kiểm thử → Ghi nhận kết quả → Phát hiện Bug → Quản lý Bug**

### Kết quả dự án

- **45 Test Case**
- **33 Passed**
- **12 Failed**
- **12 Bug**

Dự án giúp em áp dụng kiến thức **Manual Testing** và **Functional Testing** vào một hệ thống thực tế, đồng thời rèn luyện kỹ năng xây dựng Test Case, thực thi kiểm thử và quản lý Bug.
