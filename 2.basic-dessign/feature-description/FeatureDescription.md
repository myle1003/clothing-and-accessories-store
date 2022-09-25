## 1. Đăng nhập: 
- Giúp người dùng có thể thực hiện các chức năng của hệ thống
- Sau khi người dùng nhấn chọn đăng nhập
- Hệ thống yêu cầu người dùng nhập email, password và nhấn đăng nhập 
    + Password sẽ được ẩn
- Hệ thống sẽ kiểm tra email và password đã được nhập chưa?
    + Nếu chưa nhập đủ thì thông báo cần nhập đầy đủ email, password
    + Nếu đã nhập đủ thì kiểm tra email và password có tồn tại trong database không?
        * Có thì lưu thông tin đăng nhập và chuyển đến trang chủ tương ứng với phân quyền truy cập của tài khoản.
        * Sai thì thông báo email và password không đúng cần nhập lại.

*Sơ đồ tuần tự chức năng đăng nhập*

![](image/1.login.svg)

## 2. Đăng ký:
- Người dùng nhấn chọn đăng ký.
- Hệ thống sẽ hiện form đăng ký yêu cầu người dùng nhập
    + email: Yêu cầu đúng form của email và không được để trống. 
    + name: Yêu cầu không được để trống 
    + password: Yêu cầu không được để trống 
    + phone
    + address
- Nhấn nút đăng ký hệ thống
    + Kiểm tra email đã tồn tại chưa, nếu tồn tại rồi thì báo lỗi và yêu cầu nhập lại.
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

*Sơ đồ tuần tự chức năng xem trang chủ*

![](image/3.home.svg)

## 4. Quản lý doanh mục
### Khách hàng
- Tại trang chủ nhấn chọn danh mục.
- Hệ thống sẽ hiển thị danh sách các danh mục của cửa hàng.
- Nhấn chọn danh mục người dùng muốn tìm hiểu.
- Hệ thống sẽ hiển thị tất cả các sản phẩm của hệ thống thuộc danh mục đó.

*Sơ đồ tuần tự chức năng xem danh mục của khách hàng*

![](image/4.category-customer.svg)

### Admin
- Tại trang chủ nhấn chọn quản lý danh mục.
- Hệ thống sẽ hiển thị các danh mục của cửa hàng.
    + Người dùng nhấn chọn thêm/ sửa danh mục.
    + Hệ thống chuyển đến trang thêm/sửa danh mục và hiển thị form thêm/sửa danh mục
        * Người dùng nhập thông tin vào form: tên danh mục( yêu cầu không được để trống, và chưa tồn tại trong hệ thống), hình ảnh (không được để trống).
    + Người dùng chọn xóa danh mục
    + Hệ thống sẽ kiểm tra xem đã có sản phẩm nào thuộc danh mục này chưa
        * Nếu đã tồn tại, thông báo tồn tại sản phẩm thuộc danh mục này, nên không thể xóa danh mục.
        * Chưa tồn tại thì thực hiện xóa danh mục.

*Sơ đồ tuần tự chức năng quản lý danh mục của admin*

![](image/4.category-admin.svg)

## 5. Quản lý sản phẩm 
### Khách hàng
- Sau khi người dùng chọn danh mục.
- Hệ thống sẽ hiển thị danh sách các sản phẩm thuộc cửa hàng.
- Nhấn chọn sản phẩm.
- Hệ thống sẽ hiển thị thông tin chi tiết của sảng phẩm đó
    + Tên sản phẩm: luôn có.
    + Danh mục: luôn có.
    + Hình ảnh: luôn có.
    + Giá: luôn có.
    + Màu sắc: luôn có
    + Size: luôn có
    + Đánh giá: có thể có hoặc không.
    + Bình luận:có thể có hoặc không.

*Sơ đồ tuần tự chức năng xem sản phẩm của khách hàng*

![](image/5.product-customer.svg)

### Admin
- Tại trang chủ nhấn chọn quản lý sản phẩm.
- Hệ thống sẽ hiển thị các sản phẩm của cửa hàng.
    + Người dùng nhấn chọn thêm/ sửa sản phẩm .
    + Hệ thống chuyển đến trang thêm/sửa sản phẩm và hiển thị form thêm/sửa sản phẩm
        * Người dùng nhập thông tin vào form: 
            * Tên sản phẩm: không được để trống.
            * Danh mục: không được để trống.
            * Hình ảnh: không được để trống.
            * Giá: không được để trống.
            * Mô tả: có thể có hoặc không.
        + Người dùng chọn xóa sản phẩm.
        * Hệ thống sẽ thực hiện xóa sản phẩm.

*Sơ đồ tuần tự chức năng quản lý sản phẩm của admin*

![](image/5.product-admin.svg)

## 5. Tìm kiếm sản phẩm 
### Khách hàng
- Tại thanh tìm kiếm, nhập tên sản phẩm muốn tìm.
- Hệ thống sẽ hiển thị danh sách các sản phẩm có tên gần giống thuộc danh mục khách hàng đang đứng.
- Nhấn chọn sản phẩm.
- Hệ thống sẽ hiển thị thông tin chi tiết của sảng phẩm đó.

*Sơ đồ tuần tự chức năng xem sản phẩm của khách hàng*

![](image/5.search.svg)

## 6. Quản lý giỏ hàng
### Khách hàng
- Tại trang chủ nhấn chọn giỏ hàng.
- Hệ thống sẽ hiển thị các sản phẩm người dùng đã thêm vào giỏ hàng.
    + Người dùng nhấn chọn tăng/ giảm số lượng sản phẩm .
    + Người dùng cũng có thể chọn xóa sản phẩm không muốn mua nữa ra khỏi giỏ hàng.
        * Hệ thống sẽ thực hiện xóa sản phẩm.
    + Chọn mua hàng để mua các sản phẩm trong giỏ hàng được chọn.
    + Giỏ hàng sẽ mất nếu khách hàng chưa đặt nhập nhưng thoát khỏi hệ thống.
    + Khi người dùng đã đăng nhập thì giỏ hàng sẽ được lưu cho những lần dùng sau.

*Sơ đồ tuần tự chức năng quản lý giỏ hàng của khách hàng*

![](image/6.cart.svg)

## 7. Quản lý đơn vị vận chuyển
### Admin
- Tại trang chủ nhấn chọn quản lý đơn vị vận chuyển.
- Hệ thống sẽ hiển thị các đơn vị vận chuyển của cửa hàng.
    + Người dùng nhấn chọn thêm/ sửa đơn vị vận chuyển.
    + Hệ thống chuyển đến trang thêm/sửa dợn vị vận chuyển và hiển thị form thêm/sửa đơn vị vận chuyển
        * Người dùng nhập thông tin vào form: 
            * Tên đợn vị: không được để trống.
            * Khu vực: không được để trống(nội thành/ ngoại thành).
            * Giá: không được để trống.
            * Ghi chú: ví dụ: giao hàng giờ hành chính hoặc ngoài giờ hàng chính.
        * Người dùng chọn xóa đợn vị vận chuyển.
        * Hệ thống sẽ thực hiện kiểm tra đơn vị đó đã thực hiện đơn hàng nào của của hàng chưa.
            * Nếu chưa thì xóa đơn vị vận chuyển.
            * Rồi thì chuyển đơn vị vào danh sách ngưng sử dụng.

*Sơ đồ tuần tự chức năng quản lý đơn vị vận chuyển của admin*

![](image/7.deliver.svg)

## 8. Quản lý đơn hàng
Chức năng này chỉ thực hiện được khi người dùng phải đăng nhập.
### Khách hàng
- Tại trang chủ nhấn chọn quản lý hàng.
- Hệ thống sẽ hiển thị các đơn hàng đang giao.
    + Người dùng có thể chọn xem đơn đang xử lý.
    + Đơn đang giao.
    + Đơn đã giao.
    + Đơn đã hủy.

*Sơ đồ tuần tự chức năng xem đơn hàng của khách hàng*

![](image/8.bill-customer.svg)

### Admin
- Tại trang chủ nhấn chọn quản lý đơn hàng.
- Hệ thống sẽ hiển thị các đơn hàng chưa được xử lý.
    + Người dùng nhấn chọn xem đơn hàng theo 
        * Chưa được xử lý
        * Đang giao
        * Đã giao thành công
        * Đã hủy.
    + Hệ thống hiển thị các đơn hàng theo lựa chọn của admin.
    + Nhấn chọn đơn hàng.
    + Hệ thống hiển thị các thông tin chi tiết của đơn hàng.
    + Người dùng nhập chỉnh sửa đơn hàng: 
        * Tình trạng đơn hàng: không được để trống.

*Sơ đồ tuần tự chức năng quản lý đơn hàng của admin*

![](image/8.bill-admin.svg)


