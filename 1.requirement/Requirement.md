# REQUIREMENTS 
*Các chức năng dự kiến:*
## Khách hàng
### 1. Đăng nhập: 
- Mục đích: Hệ thống yêu cầu người dùng đăng nhập để có thể lưu lại giỏ hàng cho những lần đăng nhập sau.
- Người dùng cần nhập: Email và mật khẩu.
    - Mật khẩu sẽ được ẩn
    - Yêu cầu nhập đủ và đúng thông tin. Nếu không hệ thống sẽ trả về thông tin lỗi.  
- Nhấn nút đăng nhập, hệ thống kiểm tra, nếu đúng yêu cầu sẽ chuyển đến trang chủ của khách hàng.
- Nhấn nút đăng ký để thực hiện chức năng đăng ký nếu chưa có tài khoản. 
### 2. Đăng ký:
- Mục đích: Hệ thống cho phép người dùng đăng ký tài khoản để có thể lưu giỏ hàng cho lần sau sử dụng.
- Người dùng cần nhập:
    + Tên người dùng: Yêu cầu không được để trống
    + Email: Yêu cầu đúng form của email và không được để trống. 
    + Mật khẩu: Yêu cầu không được để trống
- Nhấn nút đăng ký, hệ thống kiểm tra thông tin, tạo tài khoản và chuyển đến trang chủ của hệ thống.
### 3. Trang chủ
- Hiển thị các chức năng của hệ thống
    + Danh sách các danh mục sản phẩm.
    + Danh sách các sản phẩm sale/ trend/ yêu thích.
    + Có thể thực hiện tìm kiếm tên danh mục/ sản phẩm.
    + Truy cập quản lý giỏ hàng.
    + Đặt hàng (nhập thông tin địa chỉ, số điện thoại và đơn vị giao hàng).
    + Xem thông tin cửa hàng hệ thống.
### 4. Quản lý doanh mục
- Mục đích: Hệ thống cho phép người dùng chọn lựa danh mục sản phẩm mà người dùng muốn xem.
- Tại trang chủ, người dùng lựa chọn danh mục sản phẩm mình muốn xem, hệ thống sẽ hiển thị các sản phẩm thuộc danh mục.
    + Khách hàng có thể lựa chọn các danh mục sản phẩm khác.
    + Thực hiện chức năng tìm kiếm.
### 5. Quản lý sản phẩm
- Mục đích: Hệ thống cho phép người dùng xem được chi tiết sản phẩm.
- Tại trang chủ, người dùng lựa chọn sản phẩm mình muốn xem, hệ thống sẽ hiển thị các thông tin chi tiết sản phẩm.
    + Khách hàng: 
        * Có thể lựa chọn kích thước, màu sắc và thêm sản phẩm vào giỏ hàng.
        * Cũng có thể chọn xem các sản phẩm tương tự khác của shop.
### 6. Quản lý giỏ hàng
- Mục đích: Hệ thống cho phép người dùng xem được chi tiết giỏ hàng của bản thân.
- Tại giao diện người dùng chọn giỏ hàng, hệ thống sẽ hiển thị các sản phẩm hiện đang có trong giỏ hàng.
    + Người dùng có thể tăng/ giảm số lượng ở mỗi sản phẩm.
    + Có thể xóa sản phẩm sản phẩm khỏi giỏ hàng khi không muốn mua nữa.
    + Chọn mua hàng để mua các sản phẩm trong giỏ hàng được chọn.
    + Giỏ hàng sẽ mất nếu khách hàng chưa đặt nhập nhưng thoát khỏi hệ thống.
    + Khi người dùng đã đăng nhập thì giỏ hàng sẽ được lưu cho những lần dùng sau.
### 7. Quản lý đơn hàng
- Mục đích: Hệ thống cho phép người dùng quản lý được đơn hàng của bản thân, chức năng này chỉ thực hiện được khi người dùng đã đăng nhập.
- Tại giao diện giỏ hàng người dùng chọn mua hàng, hệ thống sẽ hiển thị tổng sản phẩm người dùng chọn và yêu cầu khách hàng nhập đủ thông tin.
    + Tên người nhận: mặc định tên người dùng(đối với tài khoản đã đăng nhập)/ trống (đối với người dùng chưa đăng nhập) yêu cầu không được để trống.
    + Số điện thoại: không được để trống.
    + Đia chỉ: không được để trống.
- Người dùng có thể chọn quản lý đơn hàng để xem tình trạng(chờ xử lý/ đang giao/ giao hàng thành công/ đã hủy) các đơn hàng của bản thân.
## Admin
### 1. Đăng nhập: 
- Mục đích: Hệ thống yêu cầu người dùng đăng nhập để sử dụng được các chức năng quản lý hệ thống.
- Người dùng cần nhập: Email và mật khẩu.
    - Mật khẩu sẽ được ẩn
    - Yêu cầu nhập đủ và đúng thông tin. Nếu không hệ thống sẽ trả về thông tin lỗi.  
- Nhấn nút đăng nhập, hệ thống kiểm tra, nếu đúng yêu cầu sẽ chuyển đến trang của admin.
### 2. Trang chủ
- Hiển thị các chức năng của hệ thống thuộc quyền admin
    + Quản lý các danh mục.
    + Quản lý sản phẩm.
    + Quản lý đơn hàng mà khách hàng đã thực hiện mua hàng.
    + Quản lý đơn vị vận chuyển.
    + Tìm kiếm 
### 4. Quản lý doanh mục
- Mục đích: Admin có thể thêm sửa xóa các danh mục theo nhu cầu của cửa hàng.
- Tại trang chủ, admin lựa chọn quản lý danh mục sản phẩm, hệ thống sẽ hiển thị các danh mục của cửa hàng, admin có thể quản lý các danh mục
    + Thêm/ sửa danh mục: tên danh mục là bắt buộc không được để trống.
    + Xóa danh mục: chỉ được xóa khi chưa có sản phẩm nào thuộc danh mục đang tồn tại.
### 5. Quản lý sản phẩm
- Mục đích: Admin có thể thêm sửa xóa các sản phẩm theo nhu cầu của cửa hàng.
- Tại trang chủ, admin lựa chọn quản lý sản phẩm, hệ thống sẽ hiển thị các sản phẩm của cửa hàng, admin có thể quản lý các sản phẩm
    + Thêm/ sửa sản phẩm: tên sản phẩm, danh mục, giá, hình ảnh sản phẩm là bắt buộc không được để trống; mô tả chi tiết sản phẩm.
    + Xóa sản phẩm: sản phẩm sẽ bị xóa cả trong giỏ hàng của khách hàng.
### 6. Quản lý đơn vị vận chuyển
- Mục đích: Admin có thể thêm sửa xóa các đơn vị vận chuyển theo nhu cầu của cửa hàng.
- Tại trang chủ, admin lựa chọn quản lý đơn vị vận chuyển, hệ thống sẽ hiển thị các đơn vị vận chuyển của cửa hàng, admin có thể quản lý các đợn vị vận chuyển
    + Thêm/ sửa đơn vị: tên đơn vị, giá tương thích cho trường hợp đơn hàng nội thành/ ngoại thành những mực này không được để thống.
    + Xóa đơn vị: chỉ xóa được các đơn vị chưa được thực hiện, nếu đơn vị đã được thực hiện thì đơn vị đó sẽ được đưa vào danh sách ngưng sử dụng, nhưng vẫ còn trong hệ thống, những đơn hàng mới sẽ không thể chọn đơn vị đó.
### 7. Quản lý đơn hàng
- Mục đích: Admin có thể sửa các đơn hàng của khách hàng.
- Tại giao diện người dùng chọn quản lý giỏ hàng, hệ thống sẽ hiển thị các đơn hàng chưa được giao của của hàng.
    + Admin có thể chỉnh sửa tình trạng của đơn hàng.
    + Admin có thể chọn hiển thị đơn hàng theo trạng thái( chờ xử lý, đang giao, đã giao hàng thành công, đã hủy).
    + Hoặc hiển thị đơn hàng theo ngày/ tháng/ năm.
