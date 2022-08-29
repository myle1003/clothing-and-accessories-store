## 1. Đăng nhập: 
- Khi chưa thực hiện đăng nhập, người dùng có thể thực hiện được các chức năng trừ chức năng của admin, nhưng người dùng không thể quay lại xem giỏ hàng và quản lý đơn hàng nếu chưa đăng nhập mà thoát khỏi hệ thống.
- Hiển thị liên kết đến trang đăng ký nếu người dùng chưa có tài khoản chọn đăng ký tài khoản.
- Hệ thống yêu cầu người dùng nhập username, password và nhấn đăng nhập 
    + Password sẽ được ẩn
- Hệ thống sẽ kiểm tra username và password đã được nhập chưa?
    + Nếu chưa nhập đủ thì thông báo cần nhập đầy đủ username, password
    + Nếu đã nhập đủ thì kiểm tra username và password có tồn tại trong database không?
        * Có thì lưu thông tin đăng nhập và chuyển đến trang chủ tương ứng với phân quyền truy cập của tài khoản.
        * Sai thì thông báo username và password không đúng cần nhập lại.

*Sơ đồ tuần tự chức năng đăng nhập*

![](image/1.login.svg)

## 2. Đăng ký:
- Người dùng nhấn chọn đăng ký.
- Hệ thống sẽ hiện form đăng ký yêu cầu người dùng nhập 
    + Tên người dùng: Yêu cầu không được để trống 
    + Mật khẩu: Yêu cầu không được để trống 
    + Email: Yêu cầu đúng form của email và không được để trống. 
- Nhấn nút đăng ký hệ thống
    + Kiểm tra user đã tồn tại chưa, nếu tồn tại rồi thì báo lỗi và yêu cầu nhập lại.
    + Nếu đã kiểm tra đúng thông tin, thực hiện tạo tài khoản, lưu thông tin và chuyển đến trang chủ.

*Sơ đồ tuần tự chức năng đăng ký*

![](image/2.logup.svg)

## 3. Trang chủ
- Người dùng truy cập vào hệ thống, nhấp chọn trang chủ hay đăng nhập/ đăng ký thành công.
### Khách hàng
- Hệ thống hiển thị
    + Danh sách các danh mục sản phẩm.
    + Danh sách các sản phẩm sale/ trend/ yêu thích.
    + Truy cập quản lý giỏ hàng.
    + Đặt hàng (nhập thông tin địa chỉ, số điện thoại và đơn vị giao hàng).
    + Xem thông tin cửa hàng hệ thống.

### Admin
- Hiển thị các chức năng của hệ thống thuộc quyền admin
    + Quản lý các danh mục.
    + Quản lý sản phẩm.
    + Quản lý đơn hàng mà khách hàng đẵ thực hiện mua hàng.
    + Quản lý đơn vị vận chuyển.
    + Tìm kiếm 

![](image/3.home.svg)

## 4. Quản lý doanh mục
### Khách hàng
- Tại trang chủ nhấn chọn danh mục.
- Hệ thống sẽ hiển thị danh sách các danh mục của cửa hàng.
- Nhấn chọn danh người dùng muốn tìm hiểu.
- Hệ thống sẽ hiển thị tất cả các sản phẩm của hệ thống thuộc danh mục đó.

*Sơ đồ tuần tự chức năng xem danh mục của khách hàng*

![](image/4.category-customer.svg)

### Admin
- Tại trang chủ nhấn chọn quản lý danh mục.
- Hệ thống sẽ hiển thị các danh mục của cửa hàng.
    + Người dùng nhấn chọn thêm/ sửa danh mục.
    + Hệ thống chuyển đến trang thêm/sửa danh mục và hiển thị form thêm/sửa danh mục
        * Người dùng nhập thông tin vào form: tên danh mục( yêu cầu không được để trống, và chưa tồn tại trong hệ thống).
    + Người dùng chọn xóa danh mục
    + Hệ thống sẽ kiểm tra xem đã có sản phẩm nào thuộc danh mục này chưa
        * Nếu đã tồn tại, thông báo tồn tại sản phẩm thuộc danh mục này, nên không thể xóa danh mục.
        * Chưa tồn tại thì thực hiện xóa danh mục.

*Sơ đồ tuần tự chức năng quản lý danh mục của admin*

![](image/4.category-admin.svg)


