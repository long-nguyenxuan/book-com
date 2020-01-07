# luch-booking

## business requirement 
cần 1 cái web access được bằng mobile để thuận tiện trong việc book cơm và thanh toán qua MOMO
## input/output 
user: 
	1. đăng ký (sign in using Google)
  2. update thông tin (tên, số điện thoại)
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
