# BKQUIZ :mortar_board:

## Assignment 1 - Đề 11 - DEADLINE : Thứ 3, 16/10/2018.

### 1.Yêu cầu 

* Tìm hiểu cách thức hoạt động của ứng dụng web được cho trong đề bài và thiết kế cho các tính năng của ứng dụng (cần thiết kế tối thiểu 05 giao diện).
* Các giao diện được thiết kế phải hỗ trợ hiển thị giống nhau trên các trình duyệt web phổ biến hiện nay (Chrome, Firefox, IE, Safari,...).
* Các giao diện được thiết kế phải hỗ trợ hiển thị trên nhiều loại thiết bị khác nhau (máy tính bàn, laptop, điện thoại di dộng, máy tính bảng,...).
* Toàn bộ mã HTML5/CSS3 phải được kiểm tra và sửa lỗi sử dụng công cụ online tại địa chỉ : [http://validator.w3.org](http://validator.w3.org)
* Sinh viên có thể sử dụng các hình ảnh, thư viện CSS3, javascript có sẵn, nhưng không được sao chép toàn bộ mã nguồn của các trang web khác.

### 2.Nộp bài 

* Mã nguồn
* Báo cáo: danh sách nhóm, bảng phân chia công việc từng thành viên trong nhóm (viết ngắn gọn), ảnh chụp màn hình của tất cả các giao diện thiết kế được trên các thiết bị máy tính để bàn, máy tính bảng, điện thoại di động. Ghi email liên hệ nhóm lên bìa báo cáo. Ghi chú: đối với assignment 1 chỉ cần nộp mã nguồn và báo cáo bản mềm (PDF).

### 3.Chung 

* Assignment 1 : 30% tổng Assignment.
* Mail thầy : [huuhieubk@gmail.com](https://mail.google.com/)

### 4.Thành viên:
1. Lê Trọnng Hiếu - 1511010.  [2]
2. Trần Quốc Hưng - 1511414.  [5]
3. Nguyễn Trọng Quý - 151xxx  [1]
4. Vũ Văn Huynh - 1511328.    [3],[4]

### 5.Tasks: 
* [1] Homepage before login. 
* [2] Homepage after login.
* [3] List category. 
* [4] List type detail.
* [5] List quiz.

## Assignment 2 - Chuẩn bị

### :triangular_flag_on_post: *Chú ý:* Trước khi commit (push) thì phải pull code về trước! 

## Một số lệnh git khi làm việc với branch:
#### Muốn thêm một file hoặc folder vào nhánh hiện tại qua các bước
```

1 git add [path tới file/folder]  // câu lệnh này sẽ thêm các file mới vào Head, thay đổi vẫn còn là local
2 git commit -m [Message]  // thông điệp đi kèm cho các file vừa add ở trên
3 git push origin [tên nhánh]   // các file mới add phía trên bây giờ mới thực sự có mặt ở remote

```
#### Làm việc với Branch và Merge (sử dụng khi coding): Giả sử đang ở nhánh A, muốn merger A vào master:
Các thay đổi mới tạo ở A được push lên remote bằng bước phía trên, sau đó tiến hành merge vào master
```

1 git merge master   // A tạo request gửi tới master mong muốn được ghép với master
2 git checkout master  // nhảy qua master
3 git merge A   //(master chấp nhận request phía trên của A
4 git push   // A bây giờ đã merge vào master

```
## GIT FLOW [Có thể không cần dùng nếu chưa rành về git]

### 1.Branch 

```
1 Master : Nơi chứa source hoàn chỉnh có thể chạy được trên production.

2 Dev : Nơi để test code trước khi push lên Master. Để đảm bảo code trên Master luôn an toàn 

3 Feature : Mỗi khi code một tính năng thì phải tạo nhánh cho tính năng đó. Nhánh này từ Master.

```

### :triangular_flag_on_post: *Lưu ý:* Khi dùng git flow
```
1 Đặt tên cho nhánh feature của mình Format : <Tên mình>-<Tên feature>

2 Mỗi người code riêng trên nhánh của mình 

3 Khi chỉnh sửa ở nhánh thành viên khác thì phải báo cho họ, đúng hay sai cũng phải báo cho họ trước khi sửa. 

4 Khi gặp conflic mà liên quan đến code người khác phải báo ngay cho người đó cùng solve. Không tự solve một mình.

5 Phải đảm bảo code chạy ngon thì mới push lên master. 
```
