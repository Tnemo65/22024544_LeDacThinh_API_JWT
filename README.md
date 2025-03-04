### Setup
#### Configure the MySQL database in [application.properties](http://_vscodecontentref_/1):

   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/security_db
   spring.datasource.username=root
   spring.datasource.password=yourpassword
   ```
#### Run the application:
   ```sh
   ./mvnw spring-boot:run
   ```
### API
1. POST /auth/addNewUser - Đăng ký người dùng mới
2. POST /auth/generateToken - Xác thực và nhận JWT token
3. GET /auth/welcome - Endpoint công khai
4. GET /auth/user/userProfile - Hồ sơ người dùng (yêu cầu ROLE_USER)
5. GET /auth/admin/adminProfile - Hồ sơ quản trị viên (yêu cầu ROLE_ADMIN)
6. POST /api/admin/create - Tạo tài nguyên mới (yêu cầu ROLE_ADMIN)
7. PUT /api/admin/update - Cập nhật tài nguyên (yêu cầu ROLE_ADMIN)
8. DELETE /api/admin/delete - Xóa tài nguyên (yêu cầu ROLE_ADMIN)
9. GET /api/user/profile - Lấy thông tin hồ sơ người dùng (yêu cầu ROLE_USER)

![WelcomePage](https://github.com/user-attachments/assets/b128b2dd-6797-4ae8-b759-33e9435303b1)

![Register](https://github.com/user-attachments/assets/e0ccef5a-9a67-4e1a-aea8-6aeae30297a6)

![Login](https://github.com/user-attachments/assets/7d3d80d6-9828-443c-8e14-7b8ed613f767)

![UserProfilewithJWT](https://github.com/user-attachments/assets/24931065-2690-489d-88ec-9a5c762a0324)

![AccountListWithAdminJWT](https://github.com/user-attachments/assets/36c26f1d-e849-4490-920d-3cf50627c80b)

![UpdateAccount](https://github.com/user-attachments/assets/85a6240a-5ffc-4055-8cb3-acbb725146b5)

![DeleteAccount](https://github.com/user-attachments/assets/d33bbaf3-b695-4977-8325-dc9242c5532b)




