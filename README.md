# base-PHP2

git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/Cuongneee/base-PHP2.git
git push -u origin main

Tạo 1 kho lưu trữ mới (create a new repository)
Tạo trực tiếp trên github thì sau khi tạo xong thì chạy lệnh

Ví dụ Repo có link HTTP là: https://github.com/Cuongneee/base-PHP2.git

Lệnh:  git clone https://github.com/Cuongneee/base-PHP2.git

Project có sẵn trên máy thì chạy tập lệnh sau:

Ví dụ Repo có link HTTP là: https://github.com/Cuongneee/base-PHP2.git

    git init
    git add .
    git commit -m "first commit"
    git branch -M main
    git remote add origin https://github.com/Cuongneee/base-PHP2.git
    git push -u origin main
Nếu chạy lệnh git push -u origin main mà thấy xuất hiện dòng git push --set-upstream .... thì các em cần copy cái lệnh set-upstream đó để chạy. Vì lần đầu push code lên Repo nó hay như vậy.

Đẩy code lên GIT
Sau khi hoàn thành bước Tạo 1 kho lưu trữ mới thì các bạn tiến hành đẩy code lên khi có thay đổi (Thêm/Sửa/Xóa file)

Chạy tập lệnh sau:

    git add .
    git commit -m "Mô tả thay đổi vào đây"
    git push
GIT IGNORE
Khái niệm

Là thằng để quản lý các file KHÔNG ĐẨY LÊN GIT
Trong 1 project có thể có nhiều file .gitignore
Trường hợp dự án đặt folder vendor trong .gitignore

Khi clone code từ git về thì cd vào trong thư mục dự án.
Chạy lệnh composer update or composer install
PACKAGE USING
Route: https://github.com/bramus/router

View: https://github.com/EFTEC/BladeOne

Model: https://github.com/doctrine/dbal/

3.1. Lệnh cài: composer require doctrine/dbal

3.2. Tài liệu sử dụng: https://www.doctrine-project.org/projects/doctrine-dbal/en/4.0/reference/introduction.html

Validate: https://github.com/rakit/validation

ENV: https://github.com/vlucas/phpdotenv

.htaccess:

RewriteEngine On
RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]
RewriteRule ^index\.php$ - [L]
RewriteCond %{REQUEST_FILENAME} !-f
RewriteCond %{REQUEST_FILENAME} !-d
RewriteRule . index.php [L]
