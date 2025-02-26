# Hướng dẫn tự học NodeJS và ExpressJS
Dựa trên khóa học của F8

## Phần 1: Giới thiệu và Cài đặt Môi trường

### 1\. HTTP protocol | Giao thức HTTP | Giao thức truyền tải siêu văn bản

* **Tóm tắt:**  HTTP (Hypertext Transfer Protocol) là giao thức nền tảng của World Wide Web, quy định cách client (ví dụ: trình duyệt web) và server giao tiếp với nhau để truyền tải dữ liệu (ví dụ: trang web, hình ảnh, video...). Hiểu về các khái niệm cơ bản của HTTP như request methods (GET, POST...), status codes, headers... là rất quan trọng để lập trình web.

### 2\. SSR & CSR | Sever side rendering | Client side rendering

* **Tóm tắt:** Phân biệt giữa SSR (Server-Side Rendering - Kết xuất phía máy chủ) và CSR (Client-Side Rendering - Kết xuất phía máy khách):
    * **SSR:** Server tạo ra trang HTML hoàn chỉnh và gửi về cho client. Trình duyệt chỉ cần hiển thị. Ưu điểm: SEO tốt hơn, tải trang nhanh hơn lần đầu.
    * **CSR:** Server gửi về trang HTML cơ bản và JavaScript. Trình duyệt tải JavaScript và tự render trang. Ưu điểm: Tương tác mượt mà hơn sau lần tải đầu.
    * NodeJS và ExpressJS thường được dùng để xây dựng server backend, có thể hỗ trợ cả SSR và CSR (kết hợp với ReactJS hoặc các frontend framework khác).

### 3\. Cài đặt NodeJS && Express framework

* **Tóm tắt:** Hướng dẫn cài đặt NodeJS (môi trường runtime JavaScript phía server) và ExpressJS (framework web cho NodeJS, giúp xây dựng ứng dụng web và API nhanh chóng).

### 4\. Sử dụng thư viện Nodemon | Install Nodemon & inspector

* **Tóm tắt:**
    * **Nodemon:**  Thư viện giúp tự động restart server NodeJS khi code có thay đổi, giúp tăng tốc độ phát triển.
    * **Inspector (Node Inspector/Chrome DevTools):**  Công cụ để debug code NodeJS, giúp tìm và sửa lỗi.

### 5\. Add sourcode lên Github | Add git repository

* **Tóm tắt:** Hướng dẫn cách khởi tạo Git repository và đẩy source code dự án lên Github để quản lý phiên bản và chia sẻ code.

### 6\. Cài đặt thư viện Morgan | Install Morgan | Morgan - npm

* **Tóm tắt:** Morgan là middleware (phần mềm trung gian) cho ExpressJS, dùng để logging các HTTP request (ví dụ: method, path, status code, thời gian phản hồi...). Giúp theo dõi hoạt động của server và debug.

### 7\. Khái niệm Template Engine | Sử dụng thư viện Handlebars

* **Tóm tắt:** Template Engine (ví dụ: Handlebars, EJS, Pug) giúp tạo ra HTML động từ dữ liệu server-side. Thay vì viết HTML cứng, template engine cho phép nhúng logic (ví dụ: vòng lặp, điều kiện) và dữ liệu vào HTML template, sau đó engine sẽ render ra HTML cuối cùng. Handlebars là một template engine phổ biến cho NodeJS.

### 8\. Static file & SCSS | Cấu hình sử dụng file tĩnh

* **Tóm tắt:**
    * **Static files:**  Các file tĩnh (ví dụ: CSS, JavaScript, hình ảnh...) được server phục vụ trực tiếp mà không cần xử lý thêm. Cấu hình ExpressJS để phục vụ static files từ một thư mục cụ thể.
    * **SCSS (Sassy CSS):**  CSS preprocessor, mở rộng CSS với nhiều tính năng mạnh mẽ hơn. Cấu hình để biên dịch file SCSS thành CSS trong dự án NodeJS.

### 9\. Tích hợp Bootstrap vào dự án | Use Bootstrap 4

* **Tóm tắt:** Hướng dẫn tích hợp Bootstrap (framework CSS phổ biến) vào dự án NodeJS và ExpressJS để tạo giao diện nhanh chóng và responsive.

## Phần 2: Routing và Phương thức HTTP

### 10\. Basic routing | Kĩ thuật định tuyến trong NodeJS

* **Tóm tắt:** Routing (định tuyến) là quá trình xác định cách ứng dụng phản hồi với các request đến từ client (dựa trên URL và HTTP method). Trong ExpressJS, routing được định nghĩa bằng cách sử dụng `app.get()`, `app.post()`, `app.put()`, `app.delete()`,... để map các HTTP method và path đến các handler functions (middleware hoặc controller).

### 11\. GET method | Phương thức GET

* **Tóm tắt:** Phương thức HTTP GET dùng để **lấy dữ liệu từ server**. Dữ liệu có thể được truyền qua URL (query parameters). GET requests thường dùng để lấy trang web, danh sách sản phẩm, thông tin chi tiết...

### 12\. Query parameters | Chuỗi truy vấn

* **Tóm tắt:** Query parameters (chuỗi truy vấn) là phần thêm vào sau dấu `?` trong URL, dùng để truyền dữ liệu bổ sung cho server trong GET requests. Ví dụ: `?page=2&sort=price`. ExpressJS cung cấp cách để truy cập query parameters từ request object (`req.query`).

### 13\. Form default behavior | Hành vi mặc định của Form trong HTML

* **Tóm tắt:**  Hành vi mặc định của form HTML khi submit là gửi request **GET** đến server (nếu không chỉ định method) và **tải lại trang**. Cần hiểu hành vi này để xử lý form submit trong ứng dụng web.

### 14\. POST method | Phương thức POST | Giao thức HTTP

* **Tóm tắt:** Phương thức HTTP POST dùng để **gửi dữ liệu lên server** (ví dụ: dữ liệu form, dữ liệu JSON...). Dữ liệu được gửi trong body của request. POST requests thường dùng để tạo mới dữ liệu, submit form, upload file...

## Phần 3: Mô hình MVC và CRUD Operations

### 15\. Mô hình MVC | MVC model

* **Tóm tắt:** MVC (Model-View-Controller) là một design pattern (mẫu thiết kế) phổ biến trong phát triển web, giúp tổ chức code ứng dụng thành 3 phần riêng biệt:
    * **Model:**  Xử lý logic dữ liệu, tương tác với database.
    * **View:**  Hiển thị dữ liệu cho người dùng (UI). Trong NodeJS/ExpressJS, View thường là template engine hoặc frontend framework (ReactJS...).
    * **Controller:**  Xử lý request từ user, tương tác với Model để lấy/cập nhật dữ liệu, chọn View để render và trả về response cho user.
    * MVC giúp code dễ quản lý, bảo trì, và mở rộng hơn.

### 16\. MVC Routes & Controllers | Mô hình MVC

* **Tóm tắt:**  Trong mô hình MVC, routes (định tuyến) thường được liên kết với controllers. Controller functions sẽ xử lý logic cho từng route cụ thể (ví dụ: xử lý request lấy danh sách khóa học, request tạo mới khóa học...).

### 17\. MVC Model | Xây dựng thành phần Model trong mô hình MVC

* **Tóm tắt:** Xây dựng thành phần Model trong ứng dụng NodeJS/ExpressJS theo mô hình MVC. Model chịu trách nhiệm tương tác với database (ví dụ: sử dụng Mongoose để làm việc với MongoDB). Định nghĩa schema (cấu trúc dữ liệu), các phương thức CRUD (Create, Read, Update, Delete) cho dữ liệu.

### 18\. \[CRUD] Read from DB | Đọc Database | Xây dựng phần trang chủ

* **Tóm tắt:** Thực hiện thao tác **Read (Đọc)** trong CRUD operations. Xây dựng chức năng đọc dữ liệu từ database (ví dụ: danh sách khóa học) và hiển thị lên trang chủ (View).

### 19\. Course detail page | Xây dựng trang chi tiết | Thực hành NodeJS

* **Tóm tắt:** Xây dựng trang chi tiết khóa học. Route và controller để xử lý request lấy thông tin chi tiết của một khóa học cụ thể (dựa trên ID), sau đó render trang chi tiết (View) với dữ liệu khóa học.

### 20\. \[CRUD] Create new course | Dựng trang tạo mới khóa học | Thực hành NodeJS

* **Tóm tắt:** Thực hiện thao tác **Create (Tạo)** trong CRUD operations. Xây dựng form tạo mới khóa học (View), route và controller để xử lý form submit (POST request), validate dữ liệu, và lưu khóa học mới vào database (Model).

### 21\. \[CRUD] Update course | Dựng trang chỉnh sửa | Thực hành NodeJS

* **Tóm tắt:** Thực hiện thao tác **Update (Cập nhật)** trong CRUD operations. Xây dựng form chỉnh sửa khóa học (View), route và controller để xử lý form submit (PUT hoặc POST request), validate dữ liệu, và cập nhật thông tin khóa học trong database (Model).

### 22\. \[CRUD] Delete course | Tạo chức năng xóa trong trang | Thực hành NodeJS

* **Tóm tắt:** Thực hiện thao tác **Delete (Xóa)** trong CRUD operations. Xây dựng chức năng xóa khóa học. Route và controller để xử lý request xóa (DELETE request), xóa khóa học khỏi database (Model).

### 23\. Soft delete | Kĩ thuật xóa mềm | Thực hành NodeJS

* **Tóm tắt:** Kỹ thuật xóa mềm (Soft Delete) thay vì xóa hẳn dữ liệu khỏi database, sẽ thêm một flag (ví dụ: `deletedAt` timestamp) để đánh dấu bản ghi là đã xóa. Dữ liệu vẫn còn trong database nhưng không hiển thị và không được sử dụng trong ứng dụng. Ưu điểm: có thể khôi phục dữ liệu đã xóa, lưu lịch sử.

### 24\. Deleted count documents | Hiển thị số liệu đã xóa | Thực hành NodeJS

* **Tóm tắt:** Hiển thị số lượng bản ghi đã bị xóa mềm trong ứng dụng.

### 25\. "Select all" with checkbox | Chức năng chọn & bỏ chọn | Thực hành NodeJS

* **Tóm tắt:** Xây dựng chức năng "chọn tất cả" và "bỏ chọn tất cả" bằng checkbox trong giao diện quản lý dữ liệu (ví dụ: danh sách khóa học).

### 26\. Fix bug action form | Sửa lỗi form hành động | Thực hành NodeJS

* **Tóm tắt:** Sửa lỗi liên quan đến form hành động (ví dụ: form submit, form delete) trong ứng dụng.

### 27\. Sort middleware | Chức năng sắp xếp trang quản lý | Thực hành NodeJS

* **Tóm tắt:** Sử dụng middleware để thêm chức năng sắp xếp dữ liệu (ví dụ: sắp xếp danh sách khóa học theo tên, ngày tạo...) trên trang quản lý. Middleware sẽ xử lý logic sắp xếp trước khi controller xử lý request.

### 28\. Sort query helper | Hoàn thiện logic chức năng Sort | Thực hành NodeJS

* **Tóm tắt:** Hoàn thiện logic chức năng sắp xếp dữ liệu, có thể sử dụng helper functions để tái sử dụng logic sắp xếp.

### 29\. Auto increment id field | Trường tăng ID tự động | Thực hành NodeJS

* **Tóm tắt:**  Cấu hình database (ví dụ: MongoDB) để trường ID (primary key) tự động tăng giá trị khi thêm bản ghi mới, giúp đơn giản hóa việc quản lý ID.
