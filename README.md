# Hướng dẫn sử dụng GIT
1. Tạo một tài khoản trên GITHUB
2. Tạo một thùng chứa đồ án (repository)
3. Tải và cài đặt GIT về máy local
4. Clone đồ án mới tạo về local
  - Cú pháp: git clone <URL>. URL là địa chỉ repository mà các bạn mới tạo
5. Thêm task mới làm xong vào git
  - git add . (Lệnh này là add tất cả nhưng thay đổi trong thư mục)
  - git add <tên file cần add>. (Lệnh này là add tất cả các thay đổi)
  - Kiểm tra trạng thái nó thay đổi bằng cú pháp: git status khi file mới làm đã chuyển sang màu xang thì ok
6. Xác nhận muốn đẩy lên github với cú pháp: git commit -m "". Lệnh này để xác nhận trước khi muốn đẩy lên web
7. push đồ án lên github với cú pháp: git push. khi push xong kiểm tra tiếp nếu nhánh đó đã clean thì ok
- Người tiếp theo trong nhóm sẽ pull đồ án về bằng cú pháp: git pull origin <tên nhánh>
- Tạo nhánh riêng để làm việc: cú pháp tạo nhánh: git branch <tên nhánh>
- Tạo xong nhánh thì checkout tới nhanh đó để làm việc với  cú pháp: git checkout <tên nhánh>
- Mỗi người làm xong task của mình thì đẩy lên github để lần sau làm, tránh trường hợp mất code.
- Sau khi hoàn thành tất cả task trong nhánh của mình thì merge tới master. Tưc là chuyển nhánh đó làm về nhánh master
8. Fix lỗi khi không thể clone đồ án về local: git config --global http.proxy "192.168.101.253:3128"
