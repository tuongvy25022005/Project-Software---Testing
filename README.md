# Project-Software---Testing
# Manual Testing – ParaBank

## 1. Giới thiệu dự án

Dự án thực hành kiểm thử phần mềm website **ParaBank**, một hệ thống mô phỏng dịch vụ ngân hàng trực tuyến được sử dụng cho mục đích học tập và thực hành kiểm thử phần mềm.

Mục tiêu của dự án là áp dụng quy trình **Manual Testing** và **Functional Testing** để kiểm tra các chức năng của hệ thống, xây dựng Test Case, thực thi kiểm thử, ghi nhận kết quả và quản lý các lỗi phát hiện được.

---

## 2. Thông tin ứng dụng

**Tên ứng dụng:** ParaBank

**Loại hệ thống:** Online Banking Demo

**URL:** https://parabank.parasoft.com/parabank/

ParaBank mô phỏng một số nghiệp vụ cơ bản của ngân hàng trực tuyến như đăng ký tài khoản, đăng nhập, mở tài khoản, chuyển tiền, thanh toán hóa đơn, tra cứu giao dịch và quản lý thông tin khách hàng.

Trong phạm vi dự án, tập trung kiểm thử 3 chức năng:

- Register
- Open New Account
- Bill Pay

---

## 3. Mục tiêu kiểm thử

- Kiểm tra hoạt động của các chức năng trong phạm vi dự án.
- Xác minh hệ thống xử lý đúng dữ liệu hợp lệ và không hợp lệ.
- Kiểm tra việc validate dữ liệu đầu vào.
- Xác định các trường hợp hệ thống hoạt động không đúng yêu cầu.
- Ghi nhận và quản lý Bug trong quá trình kiểm thử.
- Tổng hợp và đánh giá kết quả kiểm thử.

---

## 4. Phạm vi kiểm thử

### Chức năng được kiểm thử

#### Register
Kiểm thử chức năng đăng ký tài khoản, bao gồm:

- Kiểm tra thông tin bắt buộc.
- Kiểm tra đăng ký với dữ liệu hợp lệ.
- Kiểm tra Username và Password.
- Kiểm tra Confirm Password.
- Kiểm tra Username đã tồn tại.
- Kiểm tra dữ liệu chứa khoảng trắng.
- Kiểm tra ký tự đặc biệt.
- Kiểm tra Phone Number và Zip Code.

**Số lượng: 20 Test Case**

#### Open New Account
Kiểm thử chức năng mở tài khoản mới, bao gồm:

- Mở tài khoản Checking.
- Mở tài khoản Savings.
- Kiểm tra danh sách loại tài khoản.
- Kiểm tra tài khoản nguồn.
- Kiểm tra tài khoản mới sau khi tạo.
- Kiểm tra loại tài khoản sau khi tạo.

**Số lượng: 6 Test Case**

#### Bill Pay
Kiểm thử chức năng thanh toán hóa đơn, bao gồm:

- Payee Name.
- Address.
- City.
- State.
- Zip Code.
- Phone Number.
- Account Number.
- Verify Account.
- Amount.
- Số tiền bằng 0.
- Số tiền âm.
- Số tiền vượt quá số dư.
- Dữ liệu chứa ký tự đặc biệt.
- Dữ liệu không hợp lệ.

**Số lượng: 19 Test Case**

### Chức năng không kiểm thử

Các chức năng sau nằm ngoài phạm vi của dự án:

- Login
- Transfer Funds
- Find Transactions
- Request Loan
- Update Contact Info

Ngoài ra, dự án không thực hiện:

- Performance Testing
- Security Testing
- Load Testing
- Compatibility Testing
- Source Code Testing
- Database Testing

---

## 5. Phương pháp kiểm thử

Dự án sử dụng:

**Manual Testing + Functional Testing**

Quy trình thực hiện:

```text
Phân tích yêu cầu
       ↓
Xây dựng Test Case
       ↓
Chuẩn bị dữ liệu kiểm thử
       ↓
Thực hiện kiểm thử
       ↓
Ghi nhận Test Result
       ↓
Pass / Fail
       ↓
Ghi nhận Bug
       ↓
Theo dõi Bug trên GitHub Issues
## 6. Phương pháp kiểm thử

Dự án sử dụng phương pháp **Manual Testing** và tập trung vào **Functional Testing**.

Quy trình kiểm thử:

- Phân tích yêu cầu và chức năng.
- Xây dựng Test Case.
- Chuẩn bị dữ liệu kiểm thử.
- Thực thi Test Case.
- Ghi nhận kết quả Pass/Fail.
- Ghi nhận Bug đối với các Test Case Failed.
- Theo dõi và quản lý Bug trên GitHub Issues.

---

## 7. Test Case

Tổng cộng **45 Test Case** được xây dựng và thực thi.

### Phân bổ Test Case

| Module | Số lượng |
|---|---:|
| Register | 20 |
| Open New Account | 6 |
| Bill Pay | 19 |
| **Tổng cộng** | **45** |

Các Test Case được thiết kế với cả dữ liệu hợp lệ và không hợp lệ nhằm kiểm tra khả năng xử lý dữ liệu đầu vào của hệ thống.

---

## 8. Quản lý Test Case

Test Case được xây dựng và quản lý trên **Testiny**.

Các nội dung được thực hiện:

- Xây dựng Test Case theo từng chức năng.
- Thiết lập Test Case ID.
- Mô tả điều kiện kiểm thử.
- Thiết lập Test Data.
- Ghi nhận Expected Result.
- Thực hiện kiểm thử và ghi nhận Actual Result.
- Cập nhật trạng thái Pass/Fail.
- Tổng hợp kết quả Test Run.

---

## 9. Kết quả kiểm thử

| Kết quả | Số lượng | Tỷ lệ |
|---|---:|---:|
| Passed | 33 | 73,3% |
| Failed | 12 | 26,7% |
| **Tổng cộng** | **45** | **100%** |

Kết quả kiểm thử cho thấy hệ thống có **33 Test Case Passed** và **12 Test Case Failed**.

Các Test Case Failed được sử dụng làm cơ sở để ghi nhận và quản lý Bug.

---

## 10. Quản lý Bug

Các lỗi phát hiện trong quá trình kiểm thử được ghi nhận và quản lý bằng **GitHub Issues**.

Mỗi Bug Report bao gồm:

- Bug ID
- Summary
- Steps to Reproduce
- Expected Result
- Actual Result
- Severity
- Status

Tổng cộng **12 Bug** được ghi nhận trong quá trình kiểm thử.

---

## 11. Phân loại Bug

| Module | Số Bug |
|---|---:|
| Register | 3 |
| Bill Pay | 9 |
| **Tổng cộng** | **12** |

Các lỗi chủ yếu liên quan đến việc hệ thống xử lý dữ liệu đầu vào không hợp lệ và chưa kiểm tra đầy đủ các trường thông tin.

---

## 12. Công cụ sử dụng

- **Testiny:** Quản lý và thực thi Test Case.
- **GitHub Issues:** Ghi nhận và theo dõi Bug.
- **Google Chrome:** Môi trường thực hiện kiểm thử.
- **Microsoft Word:** Tổng hợp và trình bày báo cáo.

---

## 13. Kỹ năng thực hành

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

## 14. Minh chứng dự án

Repository bao gồm các minh chứng cho quá trình kiểm thử:

- Test Case trên Testiny.
- Test Run và kết quả kiểm thử.
- Kết quả Passed/Failed.
- Bug Report.
- GitHub Issues.
- Hình ảnh minh chứng quá trình thực hiện Test Case.

---

## 15. Tổng kết

Dự án giúp thực hành quy trình kiểm thử phần mềm từ **phân tích yêu cầu → xây dựng Test Case → thực thi kiểm thử → ghi nhận kết quả → phát hiện Bug → quản lý Bug**.

Kết quả dự án gồm:

- **45 Test Case**
- **33 Passed**
- **12 Failed**
- **12 Bug**

Dự án là cơ sở để áp dụng kiến thức **Manual Testing** vào một hệ thống thực tế và xây dựng portfolio phục vụ vị trí **Tester/QA Intern**.
