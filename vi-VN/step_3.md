## Thêm mắt cho robot của bạn

Hãy thêm mắt cho robot của bạn!

+ Mở [trinket này](http://jumpto.cc/web-robot).
    
    Dự án sẽ trông giống như thế này:
    
    ![ảnh chụp màn hình](images/robot-starter.png)

Mỗi hình ảnh trong dự án này có tên riêng (hoặc **`id`**). Ví dụ: mã HTML để xử lý các hình ảnh khuôn mặt và mắt ('khuôn mặt', 'mắt1' và 'mắt2', bắt đầu từ dòng 8 của mã của bạn) trông như thế này:

    <img id="face" ...>
    <img id="eyes1" ...>
    <img id="eyes2" ...>
    

Bạn có thể sử dụng `id` của hình ảnh để tạo cho nó phong cách riêng, bằng cách sử dụng CSS và ký hiệu `#`. Điều này cho phép bạn tạo phong cách riêng cho từng hình ảnh.

Nhấp vào tập tin `style.css`. Chú ý kích thước khuôn mặt của robot và các hình ảnh khác nhau như thế nào?

![ảnh chụp màn hình](images/robot-id.png)

+ Thêm mã CSS này để tạo kiểu mắt cho robot:
    
        # eyes1 {
        chiều rộng: 200px;
        }
        

Lưu ý rằng bạn đang tạo kiểu chỉ cho hình ảnh `mắt1`, bằng cách sử dụng `#mắt1` trong mã CSS của bạn. Nếu bạn thích đôi mắt khác nhau, bạn có thể sử dụng `#eyes2` hoặc `#eyes3` thay thế!

![ảnh chụp màn hình](images/robot-eyes-width.png)

Bạn có thấy cách mỗi hình ảnh được hiển thị lần lượt? Điều này được gọi là định vị **tương đối**. Nếu bạn muốn cho trình duyệt biết chính xác nơi đặt mắt robot của bạn, bạn sẽ cần sử dụng định vị **tuyệt đối** thay thế.

+ Thêm ba dòng này vào mã CSS cho hình ảnh `eyes1` của bạn:
    
        vị trí: tuyệt đối;
        đầu: 200px;
        trái: 100px;
        

Bạn sẽ thấy mắt của robot di chuyển đến đúng vị trí trên robot của bạn.

![ảnh chụp màn hình](images/robot-eyes-position.png)

Mã CSS này cho trình duyệt biết hiển thị hình ảnh cách góc trên bên trái của trang web bao xa.

![ảnh chụp màn hình](images/robot-eyes-position2.png)

Bạn có thể sử dụng `bottom` thay vì `top` để cho trình duyệt biết hiển thị hình ảnh cách cuối màn hình bao xa, cũng như `right` phải, hay `left`, trái.