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