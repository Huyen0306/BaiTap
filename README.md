# BÀI TẬP

## I. GIẢI THÍCH RÕ VỀ CẤU TRÚC
**Các tác nhân (Actors) chính:**

1. **Khách hàng (Người mua)**: Người dùng truy cập TechMall để tìm kiếm, mua sắm và quản lý đơn hàng.
2. **Người bán**: Người đăng sản phẩm, quản lý đơn hàng và tương tác với khách hàng.
3. **Admin (Quản trị viên hệ thống)**: Quản lý toàn bộ hoạt động của nền tảng, từ sản phẩm, người dùng đến giao dịch.
4. **Hệ thống bên ngoài**: Ví dụ như cổng thanh toán, dịch vụ vận chuyển.
## II. DANH SÁCH CÁC USE CASE CỦA TECHMALL
#### 1. Use Case của Khách hàng (Người mua):
- **Đăng ký tài khoản**: Khách hàng tạo tài khoản mới để trở thành thành viên.
- **Đăng nhập**: Khách hàng đăng nhập vào hệ thống bằng tài khoản đã đăng ký.
- **Tìm kiếm sản phẩm**: Khách hàng nhập từ khóa hoặc sử dụng bộ lọc để tìm sản phẩm.
- **Xem chi tiết sản phẩm**: Khách hàng xem thông tin sản phẩm (giá, mô tả, đánh giá).
- **Thêm sản phẩm vào giỏ hàng**: Khách hàng chọn sản phẩm và thêm vào giỏ để mua sau.
- **Quản lý giỏ hàng**: Khách hàng chỉnh sửa (thêm, bớt) sản phẩm trong giỏ hàng.
- **Đặt hàng**: Khách hàng xác nhận đơn hàng, chọn địa chỉ giao hàng và phương thức thanh toán.
- **Thanh toán**: Khách hàng thực hiện thanh toán qua các phương thức như ví điện tử, thẻ tín dụng, hoặc COD (trả tiền khi nhận hàng).
- **Theo dõi đơn hàng**: Khách hàng kiểm tra trạng thái đơn hàng (đang xử lý, đang giao, đã giao).
- **Đánh giá sản phẩm**: Khách hàng để lại nhận xét và đánh giá sau khi nhận hàng.
- **Yêu cầu hoàn tiền/đổi trả**: Khách hàng gửi yêu cầu nếu sản phẩm có vấn đề.
- **Sử dụng mã giảm giá/voucher**: Khách hàng áp dụng mã khuyến mãi khi thanh toán.
- **Chat với người bán**: Khách hàng liên lạc trực tiếp với người bán để hỏi thông tin.
  
#### 2. Use Case của Người bán:
- **Đăng ký tài khoản người bán**: Người bán tạo tài khoản để bắt đầu kinh doanh.
- **Đăng nhập**: Người bán truy cập vào hệ thống quản lý shop.
- **Đăng sản phẩm**: Người bán thêm sản phẩm mới (ảnh, mô tả, giá, số lượng).
- **Quản lý sản phẩm**: Người bán chỉnh sửa hoặc xóa sản phẩm đã đăng.
- **Quản lý đơn hàng**: Người bán xem, xác nhận, và xử lý đơn hàng từ khách.
- **Theo dõi vận chuyển**: Người bán kiểm tra trạng thái giao hàng.
- **Chat với khách hàng**: Người bán trả lời thắc mắc hoặc hỗ trợ khách.
- **Quản lý doanh thu**: Người bán xem thống kê doanh thu và lợi nhuận.
- **Tạo chương trình khuyến mãi**: Người bán thiết lập giảm giá hoặc voucher cho sản phẩm.

#### 3. Use Case của Admin (Quản trị viên):
- **Quản lý tài khoản người dùng**: Admin kiểm tra, khóa, hoặc kích hoạt tài khoản khách hàng/người bán.
- **Quản lý sản phẩm**: Admin kiểm duyệt, xóa sản phẩm vi phạm quy định.
- **Xử lý tranh chấp**: Admin giải quyết khiếu nại giữa người mua và người bán.
- **Quản lý giao dịch**: Admin giám sát các giao dịch thanh toán và hoàn tiền.
- **Cập nhật hệ thống**: Admin thêm tính năng mới hoặc chỉnh sửa chính sách.
#### 4. Use Case liên quan đến Hệ thống bên ngoài:
- **Xử lý thanh toán**: Hệ thống cổng thanh toán (ví dụ: ShopeePay, ngân hàng) xác nhận giao dịch.
- **Cập nhật trạng thái vận chuyển**: Hệ thống logistics thông báo trạng thái giao hàng.

---

### Khuôn mẫu đặc tả Use Case chuẩn
#### 1. Tên Use Case
- **Mô tả**: Tên ngắn gọn, rõ ràng, sử dụng động từ + danh từ (ví dụ: "Đặt hàng", "Thanh toán giao dịch").
- **Ví dụ**: Đặt hàng
#### 2. Mã định danh (Use Case ID) (bỏ qua không cần làm)
- **Mô tả**: Một mã duy nhất để phân biệt use case trong dự án (thường dùng trong hệ thống lớn).
- **Ví dụ**: UC-001
#### 3. Mô tả ngắn gọn (Brief Description)
- **Mô tả**: Tóm tắt mục đích và phạm vi của use case trong 1-2 câu.
- **Ví dụ**: Use case này cho phép khách hàng chọn sản phẩm từ giỏ hàng và xác nhận đặt hàng trên hệ thống Shopee.
#### 4. Tác nhân (Actors)
- **Mô tả**: Các thực thể (người hoặc hệ thống) tương tác với use case. 
    - **Tác nhân chính (Primary Actor)**: Người khởi tạo use case.
    - **Tác nhân phụ (Secondary Actors)**: Các thực thể hỗ trợ (nếu có).
- **Ví dụ**: 
    - Tác nhân chính: Khách hàng
    - Tác nhân phụ: Hệ thống thanh toán, Đơn vị vận chuyển
#### 5. Điều kiện tiên quyết (Preconditions)
- **Mô tả**: Trạng thái cần thiết trước khi use case có thể bắt đầu.
- **Ví dụ**: 
    - Khách hàng đã đăng nhập vào tài khoản Shopee.
    - Có ít nhất một sản phẩm trong giỏ hàng.
#### 6. Luồng chính (Basic Flow)
- **Mô tả**: Mô tả chi tiết các bước chính của use case theo thứ tự, thể hiện kịch bản thành công (happy path).
- **Ví dụ**: 
    1. Khách hàng truy cập giỏ hàng trên ứng dụng Shopee.
    2. Khách hàng chọn sản phẩm muốn mua và nhấn nút "Thanh toán".
    3. Hệ thống hiển thị thông tin đơn hàng (sản phẩm, giá, phí vận chuyển).
    4. Khách hàng chọn địa chỉ giao hàng từ danh sách đã lưu hoặc nhập mới.
    5. Khách hàng chọn phương thức thanh toán (ví dụ: ShopeePay, COD).
    6. Khách hàng nhấn "Xác nhận đặt hàng".
    7. Hệ thống gửi thông báo xác nhận đơn hàng thành công tới khách hàng.
#### 7. Luồng phụ (Alternative Flows)
- **Mô tả**: Các kịch bản thay thế hoặc biến thể của luồng chính.
- **Ví dụ**: 
    - **7a. Sản phẩm hết hàng**: 
        1. Tại bước 2, hệ thống thông báo sản phẩm đã chọn hết hàng.
        2. Khách hàng quay lại giỏ hàng để chọn sản phẩm khác.
    - **7b. Thanh toán thất bại**: 
        1. Tại bước 5, hệ thống thanh toán báo lỗi (hết tiền trong ví).
        2. Khách hàng chọn phương thức thanh toán khác hoặc nạp tiền.
#### 8. Ngoại lệ (Exceptions)
- **Mô tả**: Các tình huống lỗi nghiêm trọng ngăn cản use case hoàn thành.
- **Ví dụ**: 
    - Hệ thống bị lỗi kết nối mạng, khách hàng không thể đặt hàng.
    - Địa chỉ giao hàng không hợp lệ, hệ thống yêu cầu nhập lại.
#### 9. Điều kiện hậu quả (Postconditions)
- **Mô tả**: Trạng thái của hệ thống sau khi use case hoàn thành (thành công hoặc thất bại).
- **Ví dụ**: 
    - **Thành công**: Đơn hàng được tạo, thông báo gửi tới khách hàng và người bán.
    - **Thất bại**: Đơn hàng không được tạo, khách hàng được thông báo lý do.
#### 10. Giả định (Assumptions)
- **Mô tả**: Các giả định được đưa ra khi viết use case.
- **Ví dụ**: 
    - Khách hàng có kết nối internet ổn định.
    - Hệ thống thanh toán hoạt động bình thường.
#### 11. Yêu cầu đặc biệt (Special Requirements)
- **Mô tả**: Các yêu cầu phi chức năng liên quan (hiệu suất, bảo mật, giao diện…).
- **Ví dụ**: 
    - Thời gian xử lý đơn hàng dưới 5 giây.
    - Dữ liệu thanh toán phải được mã hóa.
#### 12. Tần suất sử dụng (Frequency of Use)
- **Mô tả**: Dự đoán mức độ thường xuyên use case được thực hiện.
- **Ví dụ**: Hàng triệu lần mỗi ngày trên toàn hệ thống Shopee.
#### 13. Vấn đề mở (Open Issues)
- **Mô tả**: Các câu hỏi hoặc điểm chưa rõ cần làm rõ với các bên liên quan.
- **Ví dụ**: 
    - Có cần xác nhận OTP cho mỗi đơn hàng không?
    - Ai chịu trách nhiệm xử lý lỗi giao hàng sai địa chỉ?
---

### Ví dụ áp dụng khuôn mẫu cho Use Case "Đặt hàng" trên Shopee
#### 1. Tên Use Case
- Đặt hàng
#### 2. Mã định danh (bỏ qua không cần làm)
- UC-001
#### 3. Mô tả ngắn gọn
- Use case này cho phép khách hàng chọn sản phẩm từ giỏ hàng và xác nhận đặt hàng trên hệ thống Shopee.
#### 4. Tác nhân
- Tác nhân chính: Khách hàng
- Tác nhân phụ: Hệ thống thanh toán, Đơn vị vận chuyển
#### 5. Điều kiện tiên quyết
- Khách hàng đã đăng nhập vào tài khoản Shopee.
- Có ít nhất một sản phẩm trong giỏ hàng.
#### 6. Luồng chính
1. Khách hàng truy cập giỏ hàng.
2. Khách hàng chọn sản phẩm và nhấn "Thanh toán".
3. Hệ thống hiển thị thông tin đơn hàng.
4. Khách hàng chọn địa chỉ giao hàng.
5. Khách hàng chọn phương thức thanh toán.
6. Khách hàng nhấn "Xác nhận đặt hàng".
7. Hệ thống gửi thông báo xác nhận.
#### 7. Luồng phụ
- **7a. Sản phẩm hết hàng**: 
    1. Hệ thống thông báo hết hàng.
    2. Khách hàng quay lại giỏ hàng.
- **7b. Thanh toán thất bại**: 
    1. Hệ thống báo lỗi thanh toán.
    2. Khách hàng chọn phương thức khác.
#### 8. Ngoại lệ
- Hệ thống mất kết nối, không thể đặt hàng.
#### 9. Điều kiện hậu quả
- **Thành công**: Đơn hàng được tạo, thông báo gửi đi.
- **Thất bại**: Đơn hàng không được tạo.
#### 10. Giả định
- Khách hàng có kết nối internet.
#### 11. Yêu cầu đặc biệt
- Thời gian xử lý dưới 5 giây.
#### 12. Tần suất sử dụng
- Hàng triệu lần mỗi ngày.
#### 13. Vấn đề mở
- Có cần xác nhận OTP không?


