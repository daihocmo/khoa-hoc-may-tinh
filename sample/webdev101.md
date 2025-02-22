# 101 khái niệm cần biết trong lập trình web

<!-- 1. Internet
2. Internet Protocol (IP) Suite
3. IP Address
4. Transmission Control Protocol (TCP)
5. Packets and Data Link (Open Systems Interconnection(OSI) Model)
6. World Wide Web (WWW)
7. Hypertext Transfer Protocol (HTTP)
8. Uniform Resource Locator (URL)
9. Browser
10. Client
11. Server
12. HTTP Request
13. HTTP Response
14. HTTP Messages
15. Domain Name
16. Registrar
17. Internet Corporation for Assigned Names and Numbers (ICANN)
18. Domain Name System (DNS)
19. HyperText Markup Language (HTML)
20. Dev Tools
21. Code Editor
22. HTML Elements
23. HTML Forms
24. HTML Attributes
25. Anchor tag
26. Document Object Model (DOM)
27. Head
28. Body
29. Accessibility and Semantics
30. Div tag
31. Cascading Style Sheets (CSS)
32. Inline Style
33. CSS properties
34. Cascade
35. Style Tag
36. Selector
37. Class
38. CSS Specificity
39. External Stylesheet
40. Box Model
41. Block
42. Inline
43. Relative positioning
44. Absolute positioning
45. Fixed positioning
46. Responsive Layout
47. Media Query
48. Flexbox
49. Grid Layout
50. calc() function
51. Custom Properties
52. Syntactically Awesome Stylesheets (SASS)
53. JavaScript
54. Script Tag
55. Defer attribute
56. ECMAScript
57. Let keyword
58. Const keyword
59. Dynamically Typed
60. TypeScript
61. Events
62. Browser API
63. Event Listener
64. Functions and Data Structures
65. Array
66. Object
67. Primitive types
68. Prototypal Inheritance
69. Classes
70. Frontend Framework
71. Components
72. Declarative Code
73. Imperative Code
74. NodeJS
75. V8 Engine
76. Event Loop
77. Node Package Manager (NPM)
78. Module
79. Export statement
80. Import statement
81. Server-Side Rendering (SSR) 
82. HTTP Methods 
83. Status Code 
84. 404 Not Found 
85. Single-page application (SPA) 
86. JavaScript Object Notation (JSON) 
87. Static-Site Generation (SSG) 
88. Hydration 
89. First Contentful Paint (FCP) & Time to Interactive (TTI) 
90. Fullstack Framework 
91. Module Bundlers 
92. Linter 
93. Database 
94. User Authentication 
95. Web Server 
96. Localhost 
97. Cloud 
98. Containers 
99. Infrastructure as a service (IAAS) / Platform-as-a-Service (PAAS) / Backend-as-a-Service (BAAS) / Software as a service (SAAS) 
100. World Wide Web-based on blockchain technology (Web3) 
101. Google it!  -->

Được tạo bởi Gemini

**Mạng và Giao Thức**

1.  **Internet:** Mạng lưới toàn cầu kết nối các máy tính lại với nhau, cho phép chúng giao tiếp và chia sẻ thông tin.
2.  **Internet Protocol (IP) Suite:** Bộ giao thức nền tảng cho hoạt động của Internet, bao gồm các giao thức như IP, TCP, UDP, v.v.
3.  **IP Address:** Địa chỉ số duy nhất được gán cho mỗi thiết bị kết nối vào mạng Internet, giúp định danh và định vị thiết bị trên mạng.
4.  **Transmission Control Protocol (TCP):** Giao thức truyền tải dữ liệu đáng tin cậy, đảm bảo dữ liệu được gửi và nhận theo đúng thứ tự, không bị mất.
5.  **Packets and Data Link (Open Systems Interconnection(OSI) Model):**
    *   **Packets (Gói tin):** Đơn vị dữ liệu được chia nhỏ để truyền tải qua mạng.
    *   **Data Link (Lớp liên kết dữ liệu):** Lớp thứ hai trong mô hình OSI, chịu trách nhiệm truyền dữ liệu giữa hai nút mạng liền kề.
6.  **World Wide Web (WWW):** Hệ thống thông tin toàn cầu được xây dựng trên Internet, bao gồm các trang web, tài liệu, và ứng dụng web được truy cập thông qua trình duyệt.
7.  **Hypertext Transfer Protocol (HTTP):** Giao thức truyền tải siêu văn bản, được sử dụng để truyền tải các tài nguyên như trang web, hình ảnh, video trên Internet.
8.  **Uniform Resource Locator (URL):** Địa chỉ duy nhất xác định vị trí của một tài nguyên trên Internet, ví dụ như một trang web.
9.  **Browser (Trình duyệt):** Phần mềm cho phép người dùng truy cập và xem các trang web trên Internet (ví dụ: Chrome, Firefox, Safari).
10. **Client (Máy khách):** Thiết bị hoặc phần mềm gửi yêu cầu đến máy chủ để truy cập các dịch vụ hoặc tài nguyên.
11. **Server (Máy chủ):** Thiết bị hoặc phần mềm cung cấp các dịch vụ hoặc tài nguyên theo yêu cầu từ máy khách.
12. **HTTP Request (Yêu cầu HTTP):** Thông điệp được gửi từ máy khách đến máy chủ để yêu cầu một tài nguyên (ví dụ: trang web).
13. **HTTP Response (Phản hồi HTTP):** Thông điệp được gửi từ máy chủ về máy khách để trả lời cho một yêu cầu HTTP (ví dụ: nội dung trang web).
14. **HTTP Messages (Thông điệp HTTP):** Các thông điệp được sử dụng để giao tiếp giữa máy khách và máy chủ, bao gồm yêu cầu HTTP và phản hồi HTTP.
15. **Domain Name (Tên miền):** Tên dễ nhớ để đại diện cho một địa chỉ IP, ví dụ như google.com.
16. **Registrar (Nhà đăng ký tên miền):** Tổ chức được ủy quyền để đăng ký và quản lý tên miền.
17. **Internet Corporation for Assigned Names and Numbers (ICANN):** Tổ chức phi lợi nhuận quản lý các tên miền và địa chỉ IP trên toàn cầu.
18. **Domain Name System (DNS):** Hệ thống phân giải tên miền thành địa chỉ IP, giúp người dùng truy cập trang web bằng tên miền thay vì địa chỉ IP phức tạp.

**HTML, CSS và DOM**

19. **HyperText Markup Language (HTML):** Ngôn ngữ đánh dấu dùng để tạo cấu trúc nội dung của trang web.
20. **Dev Tools (Công cụ nhà phát triển):** Bộ công cụ tích hợp trong trình duyệt, giúp nhà phát triển kiểm tra và sửa lỗi trang web (ví dụ: kiểm tra HTML, CSS, JavaScript).
21. **Code Editor (Trình soạn thảo code):** Phần mềm giúp nhà phát triển viết và chỉnh sửa code (ví dụ: VS Code, Sublime Text, Atom).
22. **HTML Elements (Phần tử HTML):** Các thành phần cơ bản của trang HTML, được tạo thành bởi các thẻ (ví dụ: `<p>`, `<h1>`, `<img>`).
23. **HTML Forms (Biểu mẫu HTML):** Phần tử HTML cho phép người dùng nhập dữ liệu và gửi đến máy chủ.
24. **HTML Attributes (Thuộc tính HTML):** Các thuộc tính được sử dụng để cung cấp thêm thông tin cho các phần tử HTML (ví dụ: `src` của thẻ `<img>`, `href` của thẻ `<a>`).
25. **Anchor tag (Thẻ neo):** Thẻ `<a>` dùng để tạo liên kết đến các trang web khác hoặc các phần khác nhau của trang.
26. **Document Object Model (DOM):** Mô hình biểu diễn cấu trúc HTML dưới dạng cây, cho phép JavaScript truy cập và thay đổi nội dung trang web.
27. **Head (Phần đầu):** Phần chứa thông tin metadata của trang HTML, không hiển thị trực tiếp trên trang web.
28. **Body (Phần thân):** Phần chứa nội dung chính của trang HTML, hiển thị trực tiếp trên trang web.
29. **Accessibility and Semantics (Khả năng tiếp cận và Ngữ nghĩa):**
    *   **Accessibility (Khả năng tiếp cận):** Thiết kế trang web để người khuyết tật có thể dễ dàng sử dụng.
    *   **Semantics (Ngữ nghĩa):** Sử dụng các phần tử HTML phù hợp để mô tả chính xác ý nghĩa và cấu trúc của nội dung.
30. **Div tag (Thẻ div):** Thẻ `<div>` là một container chung dùng để nhóm các phần tử HTML lại với nhau.
31. **Cascading Style Sheets (CSS):** Ngôn ngữ định kiểu cho trang web, giúp trang web có giao diện đẹp mắt và nhất quán.
32. **Inline Style (Kiểu nội tuyến):** CSS được viết trực tiếp trong thuộc tính `style` của các phần tử HTML.
33. **CSS properties (Thuộc tính CSS):** Các thuộc tính dùng để định kiểu cho các phần tử (ví dụ: `color`, `font-size`, `margin`).
34. **Cascade (Tính kế thừa):** Cơ chế CSS áp dụng các kiểu theo thứ tự ưu tiên, các kiểu sau sẽ ghi đè lên các kiểu trước nếu có xung đột.
35. **Style Tag (Thẻ style):** Thẻ `<style>` dùng để nhúng CSS vào trang HTML.
36. **Selector (Bộ chọn):** Cách chọn các phần tử HTML để áp dụng kiểu CSS (ví dụ: `p`, `.class`, `#id`).
37. **Class (Lớp):** Thuộc tính `class` dùng để nhóm các phần tử HTML có cùng kiểu dáng.
38. **CSS Specificity (Độ ưu tiên của CSS):** Quy tắc xác định thứ tự ưu tiên của các bộ chọn CSS khi có nhiều kiểu cùng tác động đến một phần tử.
39. **External Stylesheet (Bảng định kiểu ngoài):** File CSS riêng biệt, được liên kết với trang HTML thông qua thẻ `<link>`.
40. **Box Model (Mô hình hộp):** Mô hình biểu diễn mỗi phần tử HTML như một hộp chữ nhật, bao gồm: nội dung, padding, border, margin.
41. **Block (Khối):** Các phần tử HTML chiếm toàn bộ chiều rộng của dòng và tạo ngắt dòng (ví dụ: `<div>`, `<p>`, `<h1>`).
42. **Inline (Nội tuyến):** Các phần tử HTML chỉ chiếm không gian cần thiết và không tạo ngắt dòng (ví dụ: `<span>`, `<a>`, `<img>`).
43. **Relative positioning (Định vị tương đối):** Di chuyển phần tử theo vị trí tương đối so với vị trí ban đầu của nó.
44. **Absolute positioning (Định vị tuyệt đối):** Di chuyển phần tử theo vị trí tuyệt đối so với phần tử chứa nó.
45. **Fixed positioning (Định vị cố định):** Giữ nguyên vị trí của phần tử ngay cả khi người dùng cuộn trang.
46. **Responsive Layout (Bố cục đáp ứng):** Thiết kế trang web để hiển thị tốt trên nhiều loại thiết bị khác nhau (điện thoại, máy tính bảng, máy tính).
47. **Media Query (Truy vấn phương tiện):** CSS cho phép áp dụng các kiểu khác nhau tùy thuộc vào điều kiện của thiết bị (ví dụ: kích thước màn hình).
48. **Flexbox:** Mô hình bố cục CSS cho phép sắp xếp các phần tử một cách linh hoạt.
49. **Grid Layout:** Mô hình bố cục CSS cho phép chia trang web thành các hàng và cột để sắp xếp các phần tử.
50. **calc() function (Hàm calc()):** Hàm CSS cho phép tính toán các giá trị trong CSS (ví dụ: `width: calc(100% - 20px);`).
51. **Custom Properties (Biến CSS):** Cho phép định nghĩa các biến trong CSS để tái sử dụng các giá trị.
52. **Syntactically Awesome Stylesheets (SASS):** Một trình tiền xử lý CSS mở rộng chức năng của CSS.

**JavaScript**

53. **JavaScript:** Ngôn ngữ lập trình dùng để tạo tương tác và xử lý logic trên trang web.
54. **Script Tag (Thẻ script):** Thẻ `<script>` dùng để nhúng JavaScript vào trang HTML.
55. **Defer attribute (Thuộc tính defer):** Thuộc tính của thẻ `<script>` cho phép trình duyệt tải và thực thi script sau khi HTML đã được phân tích cú pháp.
56. **ECMAScript:** Tiêu chuẩn hóa ngôn ngữ JavaScript.
57. **Let keyword (Từ khóa let):** Từ khóa để khai báo biến có phạm vi block-scope.
58. **Const keyword (Từ khóa const):** Từ khóa để khai báo hằng số (biến không thể thay đổi giá trị).
59. **Dynamically Typed (Định kiểu động):** Kiểu dữ liệu của biến được xác định trong quá trình chạy chương trình, không cần khai báo trước.
60. **TypeScript:** Ngôn ngữ siêu tập của JavaScript, thêm kiểu tĩnh và các tính năng khác để phát triển ứng dụng lớn.
61. **Events (Sự kiện):** Các tương tác của người dùng hoặc trình duyệt (ví dụ: click, mouseover, load).
62. **Browser API (API của trình duyệt):** Các giao diện lập trình ứng dụng do trình duyệt cung cấp, cho phép JavaScript tương tác với trình duyệt (ví dụ: DOM API, Fetch API).
63. **Event Listener (Trình lắng nghe sự kiện):** Hàm JavaScript được gọi khi một sự kiện xảy ra.
64. **Functions and Data Structures (Hàm và cấu trúc dữ liệu):**
    *   **Functions (Hàm):** Khối code được dùng để thực hiện một công việc cụ thể.
    *   **Data Structures (Cấu trúc dữ liệu):** Cách tổ chức và lưu trữ dữ liệu (ví dụ: mảng, đối tượng).
65. **Array (Mảng):** Cấu trúc dữ liệu dùng để lưu trữ một danh sách các phần tử.
66. **Object (Đối tượng):** Cấu trúc dữ liệu dùng để lưu trữ các cặp key-value.
67. **Primitive types (Kiểu dữ liệu nguyên thủy):** Các kiểu dữ liệu cơ bản như number, string, boolean, null, undefined.
68. **Prototypal Inheritance (Kế thừa nguyên mẫu):** Cơ chế kế thừa trong JavaScript dựa trên nguyên mẫu (prototype) của các đối tượng.
69. **Classes (Lớp):** Cú pháp trong JavaScript để tạo ra các đối tượng (từ ES6).
70. **Frontend Framework (Framework frontend):** Thư viện cung cấp cấu trúc và công cụ để xây dựng giao diện người dùng (ví dụ: React, Angular, Vue.js).
71. **Components (Thành phần):** Các khối xây dựng độc lập của giao diện người dùng.
72. **Declarative Code (Code khai báo):** Code mô tả kết quả mong muốn, không quan tâm đến cách thực hiện chi tiết.
73. **Imperative Code (Code mệnh lệnh):** Code mô tả từng bước thực hiện để đạt được kết quả.
74. **NodeJS:** Môi trường chạy JavaScript trên server.
75. **V8 Engine:** Công cụ JavaScript được Google sử dụng trong Chrome và Node.js.
76. **Event Loop:** Cơ chế xử lý bất đồng bộ trong JavaScript.
77. **Node Package Manager (NPM):** Trình quản lý gói cho Node.js.
78. **Module (Module):** Đơn vị code độc lập có thể tái sử dụng trong các dự án.
79. **Export statement (Câu lệnh export):** Câu lệnh dùng để xuất các module.
80. **Import statement (Câu lệnh import):** Câu lệnh dùng để nhập các module.
81.  **Server-Side Rendering (SSR):** Quá trình render trang web trên server trước khi gửi đến trình duyệt.
82.  **HTTP Methods:** Các phương thức HTTP (GET, POST, PUT, DELETE...) dùng để thực hiện các thao tác với tài nguyên trên server.
83.  **Status Code:** Mã trạng thái HTTP phản hồi từ server cho biết kết quả của yêu cầu (ví dụ: 200 OK, 404 Not Found).
84.  **404 Not Found:** Mã trạng thái HTTP cho biết server không tìm thấy tài nguyên được yêu cầu.
85.  **Single-page application (SPA):** Ứng dụng web chỉ tải một trang HTML và sau đó cập nhật nội dung động thông qua JavaScript.
86.  **JavaScript Object Notation (JSON):** Định dạng dữ liệu văn bản nhẹ dùng để trao đổi dữ liệu giữa server và client.
87.  **Static-Site Generation (SSG):** Quá trình tạo ra các trang web tĩnh tại thời điểm build.
88.  **Hydration:** Quá trình thêm tính tương tác vào các trang web được tạo bằng SSG hoặc SSR.
89.  **First Contentful Paint (FCP) & Time to Interactive (TTI):**
    *   **FCP:** Thời gian mà trình duyệt hiển thị nội dung đầu tiên trên trang.
    *   **TTI:** Thời gian mà trang web trở nên tương tác được với người dùng.
90. **Fullstack Framework:** Framework cung cấp cả frontend và backend (ví dụ: Next.js, Remix).
91. **Module Bundlers:** Công cụ đóng gói các module JavaScript thành một hoặc một vài file để tối ưu hóa hiệu suất (ví dụ: Webpack, Parcel).
92. **Linter:** Công cụ kiểm tra lỗi code và tuân thủ quy tắc (ví dụ: ESLint).
93. **Database:** Hệ thống lưu trữ dữ liệu (ví dụ: MySQL, PostgreSQL, MongoDB).
94. **User Authentication:** Quá trình xác thực người dùng để truy cập vào ứng dụng.
95. **Web Server:** Phần mềm xử lý các yêu cầu từ trình duyệt và gửi lại phản hồi (ví dụ: Nginx, Apache).
96. **Localhost:** Địa chỉ IP 127.0.0.1 dùng để truy cập các dịch vụ chạy trên máy tính cục bộ.
97. **Cloud:** Nền tảng điện toán đám mây, cung cấp các dịch vụ IT qua Internet (ví dụ: AWS, Google Cloud, Azure).
98. **Containers:** Công nghệ ảo hóa cấp hệ điều hành, đóng gói ứng dụng và các phụ thuộc của nó vào một đơn vị di động (ví dụ: Docker).
99. **Infrastructure as a service (IAAS) / Platform-as-a-Service (PAAS) / Backend-as-a-Service (BAAS) / Software as a service (SAAS):** Các mô hình dịch vụ điện toán đám mây khác nhau.
100. **World Wide Web-based on blockchain technology (Web3):** Ý tưởng về một web phi tập trung dựa trên công nghệ blockchain.
101. **Google it! (Lên Google mà tìm!):** Khi bạn muốn tìm hiểu thêm thông tin về một thứ gì đó.

Hy vọng những định nghĩa này sẽ giúp ích cho bạn!
