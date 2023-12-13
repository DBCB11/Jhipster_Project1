# Jhipster - project 1
JHipster là một nền tảng phát triển để nhanh chóng tạo, phát triển và triển khai các ứng dụng web hiện đại và kiến ​​trúc vi dịch vụ
# Cài đặt jhipster
1. Cài đặt [Java](https://adoptium.net/temurin/releases/?version=11), [Node.js](https://nodejs.org/en), [Git](https://git-scm.com/)
2. Cài đặt Jhipster bằng cách chạy câu lệnh `npm install -g generator-jhipster` trong cửa sổ cmd.
3. Tạo một thư mục mới và đi vào trong nó.
4. Mở cửa sổ cmd trong thư mục đó và chạy lệnh `jhipster`

# Demo tạo 1 project bằng Jhipster sử dụng MySQL
1. Tạo project QuanLyLopHoc:

Dưới đây là các cài đặt cho project. Ở đây mình sẽ sử dụng môi trường cho database là `H2 with disk-based persistence`, việc mình không sử dụng MySQL cho môi trường database của mình là vì đây chỉ là một bản thử, một dự án chạy thử nên mình đã ưu tiên sử dụng `H2 with disk-based persistence`.

![img](<Screenshot (627).png>)

2. Sau khi jhipster build xong chương trình. Mình đã dùng lệnh `mvnw` để khởi chạy thử và kiểm tra xem có lỗi gì không.

![img](<Screenshot (628).png>)

Mình đã bị 3 lỗi nhưng đều là cùng liên quan đến `method when` nên sẽ chỉ cần sửa trong 1 file:

![img](<Screenshot (629).png>)

3. Tạo các thực thể 

Định nghĩa tập thực thể trong [JDL Studio](https://start.jhipster.tech/jdl-studio/)

![img](<Screenshot (630).png>)

Tải xuống và copy vào trong thư mục của dự án

Mở cửa sổ cmd trong thư mục dự án và chạy lệnh `jhipster jdl 'your_file_name'.jdl` để cài JDL vào dự án jhipster của mình.

![img](<Screenshot (631).png>)

Ấn a để overwrite tất cả

![img](<Screenshot (632).png>)

4. Kiểm thử dự án

Chạy lệnh mvnw trong cửa sổ cmd của thư mục dự án

Nếu không còn lỗi nào thì sẽ có dòng như sau sẽ được hiện ra:

![img](<Screenshot (634).png>)

Sau đó chạy lệnh `npm start` để khởi động giao diện

Hình ảnh dự án minh họa

![img](<Screenshot (635).png>)

![img](<Screenshot (636).png>)

![img](<Screenshot (637).png>)

![img](<Screenshot (638).png>)

# Ưu điểm và nhược điểm
Ở đây mình đã rút ra được một số ưu điểm và nhược điểm trên phương diện khi mới chỉ là một sinh viên năm 3, chưa biết quá nhiều về lập trình.

## Ưu điểm
1. Giúp tạo ra một ứng dụng cơ bản nhanh chóng, tiết kiệm thời gian thông qua các mô hình được quyết định sẵn.
1. Mình có thể học từ mã nguồn được sinh ra tự động
1. Tích hợp sẵn các công nghệ phổ biến như Spring Boot, Angular, React, ...
1.  Có sẵn những tài liệu phong phú, có một cộng đồng đông đảo giúp đỡ.
1. Đặc biệt Jhipster hỗ trợ các công cụ quản lý phiên bản CI/CD có thể giúp mình - một người mới - làm quen với lĩnh vực lập trình.

## Nhược điểm
1. Do tính năng đầy đủ và linh hoạt, khiến mình lúc đầu cảm thấy khá phức tạp.
2. Ngoài ra việc sử dụng Jhipster đôi khi đòi hỏi một số hiểu biết với nền tảng và các công nghệ được sử dụng
3. Đặc biệt, việc tinh chỉnh lúc đầu khá khiến mình mất thời gian vì mã nguồn được tự động sinh ra.
4. Tuy Jhipster giúp tạo ra ứng dụng web, nhưng có thể trở nên phức tạp và có khả năng chứa đựng những tính năng không cần thiết. 