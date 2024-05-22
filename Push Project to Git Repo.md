# Hướng dẫn Đẩy Dự Án Lên GitLab

## Bước 1: Tạo Repository trên GitLab

- Đăng nhập vào tài khoản GitLab của bạn.
- Chọn "New project" hoặc "New repository" để tạo một repository mới.
- Điền thông tin như tên dự án, mô tả và các cài đặt khác nếu cần.

## Bước 2: Khởi tạo dự án và tạo commit

- Mở terminal hoặc command prompt trên máy tính của bạn.
- Di chuyển đến thư mục chứa mã nguồn dự án của bạn.
- Nếu dự án của bạn chưa là một repository Git, hãy chạy lệnh sau để khởi tạo:

    ```
    git init
    ```

- Tạo commit với thông điệp mô tả các thay đổi:
    ```
    git commit -m "Initial commit"
    ```


## Bước 3: Liên kết Repository của GitLab với Repository Local

- Sao chép URL của repository từ trang GitLab của bạn.
- Liên kết repository local của bạn với repository trên GitLab bằng cách chạy lệnh sau:
    ```
    git remote add origin <URL_repository_GitLab>
    ```


## Bước 4: Đẩy các thay đổi lên GitLab

- Đảm bảo bạn đã thực hiện commit các thay đổi cần thiết.
- Đẩy các thay đổi lên repository trên GitLab bằng lệnh:
    ```
    git push -u origin master
    ```

    (Nếu bạn đang sử dụng branch khác, hãy thay thế `master` bằng tên branch của bạn).

## Bước 5: Xác minh trên GitLab

- Mở lại trình duyệt và kiểm tra trên trang dự án trên GitLab để xác nhận rằng mã nguồn đã được đẩy lên thành công.
