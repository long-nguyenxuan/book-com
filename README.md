# luch-booking

## business requirement 
buổi trưa, anh em văn phòng thường đặt cơm, 
cần 1 cái web access được bằng mobile để thuận tiện trong việc book cơm và thanh toán qua MOMO

## input/output 
user: 
  1. đăng ký (sign in using Google)
  2. update thông tin (tên, số điện thoại, facebook)
  3. book cơm và thanh toán bằng momo 
admin: 
  1. add new thực đơn của từng ngày 
  2. set trạng thái là "nhận book" hoặc "close book"
## business logic
sau khi admin add new thực đơn của ngày thì user có thể book, 
khi thực hiện book thì user sẽ được book 
sau khi chọn xong thì hiển thị QR code momo để thanh toán. 
nếu không thanh toán thì lưu trạng thái "nợ" 
admin có thể xuất thông tin danh sách book thành excel để thuận tiện in ấn

## Advanced features
Cho phép đặt cơm qua Facebook Messenger 
Cho phép đặt cơm qua Slack 
Cho phép đặt cơm qua Teams 

## System constraints
web này chạy tốt với 100 users trên hạ tầng AWS t2.micro (1 vCPU, 1 GiB RAM) 

## Technical Stack 
- OS: Ubuntu server 18.04 
- DB: MySQL 
- Server: ASP.NET Core with nginx
- Client: web app with mobile compatible 

