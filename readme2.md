---
## **Tên dự án:**
- Website quản lý bán vé xem phim PenguTicket.


## **Giới thiệu:**
- Xây dựng website quản lý bán vé xem phim với các tính năng chính: tìm kiếm phim, đặt vé, chọn suất chiếu và thanh toán.


## **Thành viên nhóm:**
1. *Phạm Phúc Đức - 20520162 - ducdottoan2002*
2. *Nguyễn Hoàng Phúc - 20520277 - hoangfphucs*
3. *Nguyễn Đức Tấn - 20520751 - FloRRenn*
4. *Nguyễn Nhật Hiếu Trung - 20520830 - nnhieutrung*


## **Công nghệ:**
- **Database: MySQL 8.0.32**

- **Backend: Restful API**
  - Java 17
  - Spring Boot 3.0.6
  - Maven 3.9.1
  - JWT (io.jsonwebtoken) 0.11.5

- **Frontend:**
	- HTML
	- CSS
	- JS

- **Khác:**
	- Docker: Cho phép triển khai project nhanh chóng trên các máy tính khác nhau.
	- Nginx: Dựng server cho các service trong docker.
	- Sandbox của VNPay: phát triển và kiểm thử các tính năng, giao diện và tích hợp của các ứng dụng thanh toán của VNPAY mà không ảnh hưởng đến môi trường sản phẩm thực tế.


## **Cài đặt:**
- docker-compose up --build

## **Sử dụng:**
### **Các Website:**
- Website chính: 127.0.0.1:8080 
	- Giúp người dùng tìm kiếm phim, thông tin về các phim đang chiếu(tên phim, poster, thể loại, thời lượng).
- Website cho Admin: 127.0.0.1:34524 
	- Giúp cho admin quản lý dữ về liệu suất chiếu phim như:Thêm, xóa, sửa phim chiếu, lịch chiếu, phòng chiếu, số lượng ghế và lưu lại một số thông tin thanh toán. 
- Website cho API: 127.0.0.1:9782
	- Dùng để kiểm tra, gỡ lỗi các yêu cầu HTTP đến API và nhận lại các phản hồi từ API.
- Website cho Database (PHPMyAdmin): 127.0.0.1:9782 
	- Dùng để Quản lý cơ sở dữ liệu(thêm, xóa, sửa các bảng), Sao lưu dữ liệu, Quản lý người dùng và quyền truy cập.


## **Chức năng của trang web:**
### **#Chức năng của User:**
- Đăng ký
	+ Xác thực tài khoản qua email
- Đăng nhập
- Đăng xuất
- Quên mật khẩu
	+ Xác nhận mật khẩu mới qua email
- Tìm kiếm phim theo từ khóa, thể loại
- Đặ̣t vé:
	+ Lựa chọn suất chiếu(ngày, giờ, phòng chiếu)
	+ Chọn chỗ ngồi
	+ Thanh toán (VNPAY, QR Code, Thẻ Nội Địa, Thể Quốc Tế) i
    	* Gửi vé điện tử và chi tiết thanh toán qua email khi thanh toán thành công.

### **#Chức năng của Admin:**
- Thêm, xóa, sữa dữ liệu liên quan đến các suất chiếu phim như: phim chiếu, lịch chiếu, phòng chiếu, số lượng ghế và lưu lại thông tin thanh toán.

### **#Bảo mật:**
- JWT (JSON Web Token): Phân quyền truy cập và xác thực user.


## **REST API:**
- Xem chi tiết tại http://127.0.0.1:9595/swagger-ui/index.html


© Group Pengu - NT213.N21.ANTT, University of Information Technology - UIT
