---
hide:
  - navigation
---

# Lộ trình tự học Fullstack 6 tháng theo tuần.
Hiện tại lộ trình này mình viết cho cá nhân mình dùng nên nó vẫn chưa được hoàn chỉnh. Mình cũng sẽ chỉnh sửa và cải thiện trong quá trình học luôn.

!!! warning "Thời gian học lộ trình này chỉ mang tính chất ước lượng"
    Bạn có thể sẽ hoàn thành nó chậm hơn hoặc nhanh hơn so với thời gian mà chương trình đề cập. Phần này tùy thuộc vào bạn. Vậy nên, kể cả khi mình hoàn thành nó sau 6 tháng cũng không vấn đề gì. Điều quan trọng nhất là cần duy trì thói quen học hàng ngày.

## Chọn lộ trình khác

Nếu bạn muốn học những lộ trình khác thì có thể thử:

- [Fullstack Open](https://fullstackopen.com/en/)
- [TheOdinProject](https://www.theodinproject.com/)
- [FreeCodeCamp](https://www.freecodecamp.org/learn/full-stack-developer/)

Lộ trình mình viết lại để khắc phục những "nhược điểm" (theo cá nhân mình thôi nha) của TOP và FCC:

- FCC quá tập trung vào làm bài tập thực hành: Nghe có vẻ hơi ngược đời nhưng cách học của mình muốn là "học kiến thức nền tảng và đi xây dựng những dự án mà mình chọn". Mình khi học FCC hay cố hoàn thành bài tập cho xong mà không cảm thấy như đống kiến thức đó được sử dụng thực tế.
- TOP không thống nhất trong nguồn tài nguyên: Họ gợi ý mỗi việc học một phần kiến thức ở một trang khác nhau. Mình nghĩ là nó khá hay cho việc học thêm, nhưng nó khá phức tạp và phải chuyển qua chuyển lại các trang khác. Dù vậy nhưng lộ trình này cũng gợi ý kiểu vậy :D nhưng nó ít hơn.

## Lộ trình học
Lộ trình sẽ được chia ra làm 26 tuần. Cách học cơ bản của lộ trình là trong mỗi tuần sẽ có những phần kiến thức mà bạn cần (mình nghĩ là cần) học. Bạn hoàn toàn có thể bỏ qua những phần bạn đã học từ trước hoặc muốn học sau (Khi dự án bạn muốn xây dựng cần đến phần kiến thức đó). Lộ trình này được xây dựng dựa trên [lộ trình Fullstack của Repo này](https://github.com/nishant-Tiwari24/coding-resources).

Về phần dự án hàng tuần, thử nghĩ xem bạn muốn làm ứng dụng gì. Bạn có thể đọc [Hướng dẫn xây dựng dự án cơ bản](cach-len-ke-hoach.md) để học cách bắt đầu lên ý tưởng.

Mỗi tuần bạn nên thử làm ít nhất một dự án (một ứng dụng đơn giản để áp dụng các nội dung bạn đã học trong tuần, gì cũng được). Mình sẽ để một danh sách gợi ý bên dưới.

### Tuần 1: HTML, CSS

#### Bạn sẽ học

HTML/CSS cơ bản và responsive design

#### Nguồn tài nguyên học
Nguồn học cơ bản:

- [Khóa HTML/CSS cơ bản của F8 - Tiếng Việt](https://www.youtube.com/playlist?list=PL_-VfJajZj0U9nEXa4qyfB4U5ZIYCMPlz)
- [HTML Foundations](https://www.theodinproject.com/paths/foundations/courses/foundations#html-foundations)
- [CSS Foundations](https://www.theodinproject.com/paths/foundations/courses/foundations#css-foundations) 

Nếu học trên FullStackOpen thì học phần [Part 0 - Fundamentals of Web apps](https://fullstackopen.com/en/part0)

Đọc thêm các nội dung khác liên quan đến HTML/CSS:

- [Giới thiệu về DOM](https://viblo.asia/p/gioi-thieu-ve-dom-WAyK8J2ElxX) - Tìm hiểu về DOM (Document Object Model). Sẽ có một chút phần code của JavaScript, bạn có thể bỏ qua và chỉ cần tập trung vào hiểu DOM là gì.
- [Guide to Writing Semantic HTML](https://cs.fyi/guide/writing-semantic-html) - Cách viết semantic HTML (Semantic HTML refers to the use of HTML markup to convey the meaning of the content on a web page, rather than just its appearance)
- [Don't click here](https://www.dont-click-here.com/)  

### Tuần 2: JavaScript cơ bản
#### Bạn sẽ học
JavaScript cơ bản

- Các nội dung cơ bản như: variables (biến), loops (vòng lặp), functions (hàm), và arrays (chuỗi).
- Tìm hiểu về các chức năng ES6 như let, const, và arrow functions.
- DOM manipulation

#### Nguồn tài nguyên học

- [30-Days-Of-JavaScript](https://github.com/Asabeneh/30-Days-Of-JavaScript) - Học từ đầu - Khóa này đã có người dịch sang Tiếng Việt và bạn có thể đọc luôn: [Bản dịch Tiếng Việt của 30-Days-Of-JavaScript](https://github.com/Asabeneh/30-Days-Of-JavaScript/blob/master/Vietnamese/README.md).
- [33 Concepts Every JavaScript Developer Should Know](https://github.com/leonardomso/33-js-concepts) - Tổng hợp những concepts mà "JS devs" nên biết

#### Trong lúc học HTML/CSS/JS bạn có thể đọc thêm một số bài viết này
- [Command Line Basics](https://www.theodinproject.com/lessons/foundations-command-line-basics) - Tìm hiểu cách sử dụng giao diện dòng lệnh cơ bản cho các hệ điều hành Unix-based (MacOS, Linux .etc.)

### Tuần 3: Backend (Phần 1)
Thường mình thấy trong các khóa học hoặc chương trình khác thì mọi người thường hay cho học Frontend trước. Chương trình này sẽ lựa chọn Backend để khởi đầu trước.

Trích từ [một bình luận của một vozer khác](https://voz.vn/t/lo-trinh-tu-hoc-phat-trien-website-fullstack-fullstack-web-development.970731/post-33389959) trên Thread Fullstack của tôi:

> mình nghĩ nên bắt đầu từ BE trước, nắm vững các kiến thức cơ bản về DB, OOP, thuật toán, mạng, Linux,...
> rồi học liên quan đến setup, build web trên server qua Docker, VPS,...
> sau đấy mới move dần qua FE. Bắt đầu từ SSR để làm quen với HTML, CSS, JS sau đó chuyển qua CSR làm quen với các lib, framework như React, Vue, Angular

Thanks bác, lộ trình này sẽ học Backend trước rồi mới học Frontend

#### Bạn sẽ học
- Những kiến thức cơ bản về Internet: Cách Internet hoạt động, HTTP, tên miền, hosting, DNS, trình duyệt bla bla.
- Tìm hiểu về [JavaScript runtime environment](https://topdev.vn/blog/javascript-runtime-environment-la-gi/) và [Web Server](https://viblo.asia/p/web-server-la-gi-tim-hieu-ve-web-server-WR5JRv0rJGv)
- Viết [HTTP servers](https://scribe.rip/@gabriellamedas/the-http-server-explained-c41380307917).
- Lựa chọn ngôn ngữ Backend bạn muốn học (JavaScript, Ruby, Java, Go, Rust .etc.) và học [cơ bản](https://old.reddit.com/r/learnprogramming/comments/pxg54p/how_to_start_programming_from_zero/) của nó. Chương trình này sẽ lựa chọn Node.js
- Version Control System (Git và Github):
  - [Từ gà tới pro Git và Github trong 20 phút - Tự học Git siêu tốc](https://www.youtube.com/watch?v=1JuYQgpbrW0)
  - [Git and Github Crash Course](https://www.youtube.com/watch?v=RGOj5yH7evk)

#### Nguồn tài nguyên học
- [Awesome Lập trình](https://daihocmo.github.io/awesome-lap-trinh/) - Danh sách tổng hợp tài nguyên học lập trình và khoa học máy tính bằng Tiếng Việt.

Nếu bạn đang học Rust thì hãy đọc [Hướng dẫn cày Rust](https://daihocmo.github.io/awesome-lap-trinh/ngon-ngu/rust.html)

#### Đọc thêm
- [Commit Messages](https://www.theodinproject.com/lessons/foundations-commit-messages) - Học cách viết Commit Message mỗi khi thực hiện commit trong Git.
- [Problem Solving](https://www.theodinproject.com/lessons/foundations-problem-solving) - Giải quyết vấn đề trong lập trình.
- [Understanding Errors](https://www.theodinproject.com/lessons/foundations-understanding-errors) - Hiểu về lỗi trong lập trình (Bài viết này tập trung vào JS, nhưng đọc để hiểu về tư duy về lỗi lập trình khá hay)
- [Clean Code](https://www.theodinproject.com/lessons/foundations-clean-code) - Phần lớn thời gian lập trình được dành để đọc Code. Hướng dẫn viết Code dễ đọc.

### Tuần 4: Backend (Phần 2)

#### Bạn sẽ học
- Học [HTTP basics](https://www.freecodecamp.org/news/what-is-http/), [request-response cycle](https://davisgitonga.dev/blog/request-response-cycle).
- Tạo REST APIs.

#### Tài nguyên học
- [Khóa Node.js và Express.js của F8](https://www.youtube.com/playlist?list=PL_-VfJajZj0VatBpaXkEHK_UPHL7dW6I3)

Nếu bạn cũng đang học Rust như mình thì:

- [Create a blazingly fast REST API in Rust (Part 1/2)](https://hub.qovery.com/guides/tutorial/create-a-blazingly-fast-api-in-rust-part-1/)
- [Tạo CRUD API đơn giản với Rust](https://viblo.asia/p/tao-crud-api-don-gian-voi-rust-Az45bG0OKxY)

#### Có thể bạn sẽ muốn đọc thêm
- [Request-Response Cycle Through A Story](https://scribe.rip/@castonboyd/request-response-cycle-through-a-story-e552a7afff41)
- [CRUD là gì? So sánh sự khác biệt giữa CRUD và REST](https://vietnix.vn/crud-la-gi/)

### Tuần 5: NoSQL Databases (MongoDB)

#### Bạn sẽ học
- Tìm hiểu về [NoSQL concepts](https://viblo.asia/p/gioi-thieu-ve-nosql-database-djeZ1a9jZWz)
- Perform [CRUD operations](https://viblo.asia/p/crud-la-gi-lap-trinh-website-crud-crud-database-Ljy5VyLzlra) with MongoDB.
- Tìm hiểu về schema design và indexing:
  - [Database Schema Design](https://viblo.asia/p/lam-the-nao-de-thiet-ke-mot-co-so-du-lieu-phan-1-rYvGwavgKVw) - Thiết kế cơ sở dữ liệu

#### Nguồn tài nguyên học
- [A Comprehensive NoSQL Tutorial Using MongoDB](https://www.datacamp.com/tutorial/nosql-tutorial)
- [Learn About NoSQL Databases in This 3-hour Course](https://www.freecodecamp.org/news/learn-nosql-in-3-hours/)

### Tuần 6: SQL cơ bản

#### Bạn sẽ học
- Learn SQL syntax.
- Perform CRUD operations with SQL databases (e.g., MySQL or PostgreSQL).

#### Nguồn tài nguyên học
Chưa có

### Tuần 7: ORMs (Sequelize/Mongoose)

#### Bạn sẽ học
- Learn about Object-Relational Mapping.
- Use Sequelize for SQL and Mongoose for MongoDB.
- Understand model relationships.

#### Nguồn tài nguyên học
Chưa có 

### Tuần 8: React cơ bản

#### Bạn sẽ học
- Học React nền tảng: JSX, components, props, và state.
- Sử dụng React Developer Tools.
- Xây dựng một task tracker app.

#### Nguồn tài nguyên học

### Tuần 9: Styling React Apps (Hoặc Vue, Stelve .etc.)

#### Bạn sẽ học
- Style React apps sử dụng Tailwind CSS hoặc styled-components.
- Học responsive design trong React

#### Nguồn tài nguyên học

### Tuần 10: TypeScript cơ bản

#### Bạn sẽ học
- Học TypeScript syntax và static typing.
- Tích hợp TypeScript với React.
- Tìm hiểu về type declarations cho APIs và models.

#### Nguồn tài nguyên học

### Tuần 11: Next.js cơ bản

#### Bạn sẽ học
- Học server-side rendering (SSR) và static site generation (SSG).
- Xây dựng SEO-friendly apps.


- Xây dựng một blog site sử dụng Next.js.

#### Nguồn tài nguyên học

### Tuần 12: Monorepos và Turborepo

#### Bạn sẽ học
- Học monorepos và how to organize multiple dự án.
- Sử dụng Turborepo cho performance optimization.


- Tạo một monorepo cho shared libraries trong React và Node.js.

#### Nguồn tài nguyên học

### Tuần 13: Websockets & RTC cơ bản

#### Bạn sẽ học
- Học real-time communication với Websockets.
- Học RTC cho video/audio communication.

#### Nguồn tài nguyên học

### Tuần 14: Testing cơ bản

#### Bạn sẽ học
- Học unit và integration testing.
- Sử dụng Jest và React Testing Library.
- Test APIs và frontend components.

#### Nguồn tài nguyên học

### Tuần 15: Authentication & JWT

#### Bạn sẽ học
- Học secure user authentication.
- Sử dụng JWT và cookies cho session management.

#### Nguồn tài nguyên học

### Tuần 16: Tối ưu cơ sở dữ liệu

#### Bạn sẽ học
- Tìm hiểu về database optimization techniques (e.g., indexing, query optimization).


- Optimize queries cho existing dự án.

#### Nguồn tài nguyên học

### Tuần 17: Khái niệm Backend nâng cao

#### Bạn sẽ học
- Học thêm về asynchronous programming và error handling.
- Học middleware chaining.
- Implement các logic backend phức tạp.


- Refactor APIs với advanced features như rate limiting và complex queries.

#### Nguồn tài nguyên học

### Tuần 18: Ref, Populate, và API Design

#### Bạn sẽ học
- Sử dụng ref và populate trong Mongoose cho relationships.
- Học API versioning và documentation (Swagger).

  
- Add relationships to your MongoDB models.   

#### Nguồn tài nguyên học

### Tuần 19: Các chức năng Frontend nâng cao    

#### Bạn sẽ học
- Học dynamic form handling, animations, và accessibility features trong React.
- Tìm hiểu về Framer Motion cho animations.

#### Nguồn tài nguyên học

### Tuần 20: Project Planning    

#### Bạn sẽ học
- Plan một capstone project.
- Define features, Tạo high-level (HLD) và low-level designs (LLD)

#### Nguồn tài nguyên học

### Tuần 21: Capstone Backend Development     

#### Bạn sẽ học
- Xây dựng the backend cho your capstone project.
- Implement CRUD APIs, authentication, và error handling.


- Set up Express.js, MongoDB, và authentication cho the project. 

#### Nguồn tài nguyên học

### Tuần 22: Capstone Frontend Development    

#### Bạn sẽ học
- Xây dựng the frontend cho your capstone project.
- Sử dụng React hoặc Next.js cho user interface.
- Style the app với Tailwind CSS.   


- Tích hợp the backend với the frontend. 

#### Nguồn tài nguyên học

### Tuần 23: Real-Time Features trong Capstone    

#### Bạn sẽ học
- Add real-time features sử dụng Websockets hoặc RTC.
- Implement live chat hoặc real-time notifications


- Enhance the capstone app với real-time functionality.  

#### Nguồn tài nguyên học

### Tuần 24: Testing và Deployment     

#### Bạn sẽ học
- Test the app thoroughly.
- Deploy the app to một cloud platform (e.g., Vercel, Heroku)
   

#### Nguồn tài nguyên học

### Tuần 25: Linting và Performance Optimization    

#### Bạn sẽ học
- Set up linting tools (e.g., ESLint, Prettier).
- Optimize frontend và backend performance.
- Học về caching strategies

#### Nguồn tài nguyên học

### Tuần 26: Final Enhancements & Portfolio

#### Bạn sẽ học
- Polish the capstone project.

#### Đặc biệt chút
- Add the project to một portfolio site.
- Prepare cho interviews với dự án và một resume.   
- Tạo một portfolio cá nhân sử dụng Next.js.
- Showcase all 10 dự án trong portfolio của bạn. 


## Danh sách dự án

Danh sách 10 ý tưởng gợi ý để xây dựng ứng dụng Fullstack.

### Dự án 1: Task Tracker App    
  
#### Mô tả
Một React app to track daily tasks với add, edit, và delete functionality.    

#### Các bước xây dựng
1. Set up React. 
2. Xây dựng một task list UI. 
3. Add state management với React hooks. 
4. Store tasks locally.

#### Tech Stack
React, CSS 

### Dự án 2: Bookshelf App

#### Mô tả
một MongoDB-powered app to manage một collection of books với search và CRUD operations.

#### Các bước xây dựng
1. Set up MongoDB.
2. Tạo Express APIs cho CRUD operations.
3. Connect backend to một React frontend

#### Tech Stack
Node.js, Express, MongoDB, React

### Dự án 3:  Blog Platform       . 

#### Mô tả
Một platform cho users to post, edit, và delete blog entries. Includes JWT-based authentication.

#### Các bước xây dựng
1. Xây dựng REST APIs với Express. 
2. Sử dụng MongoDB hoặc PostgreSQL cho storing blogs. 
3. Add authentication

#### Tech Stack
Node.js, MongoDB/PostgreSQL, React  

### Dự án 4: Chat App    

#### Mô tả
Real-time chat app sử dụng Websockets với user authentication.  
#### Các bước xây dựng
1. Set up Websockets on the backend.
2. Implement chat UI trong React.
3. Add JWT authentication.   
#### Tech Stack
Node.js, Websockets, React

### Dự án 5: E-Commerce Store

#### Mô tả
một store với product listings, một cart system, và checkout functionality.    
  
#### Các bước xây dựng
1. Design product APIs. 
2. Add cart logic trong React.
3. Tích hợp Razorpay/Stripe cho payments.

#### Tech Stack
React, Node.js, MongoDB, Payment APIs

### Dự án 6: Portfolio Website

#### Mô tả
một personal portfolio to showcase dự án và skills.   

#### Các bước xây dựng
1. Sử dụng Next.js cho SSR.
2. Style với Tailwind CSS.
3. Add portfolio content dynamically sử dụng JSON.    

#### Tech Stack
Next.js, Tailwind CSS   


### Dự án 7: Expense Tracker    
 
#### Mô tả
một tool to track income và expenses với visualizations.    

#### Các bước xây dựng
1. Tạo React components cho transactions.
2. Store data trong MongoDB.
3. Visualize data sử dụng Chart.js.

#### Tech Stack
React, MongoDB, Chart.js   

### Dự án 8: Online Classroom Platform    

#### Mô tả
một platform cho faculty to share documents, conduct live sessions, và Tạo assignments.   

#### Các bước xây dựng
1. Xây dựng backend với Express.
2. Implement user roles.
3. Add WebRTC cho live classes.  

#### Tech Stack
Node.js, WebRTC, React   


### Dự án 9: Video Conferencing App    
 
#### Mô tả
một basic conferencing app sử dụng WebRTC cho real-time communication.   

#### Các bước xây dựng
1. Set up WebRTC APIs.
2. Xây dựng React frontend.
3. Manage connections sử dụng signaling servers.   

#### Tech Stack
WebRTC, React 

### Dự án 10: Capstone E-Commerce App    
#### Mô tả
một fully-featured app với real-time notifications, authentication, và performance optimization.  
#### Các bước xây dựng

1. Plan HLD và LLD.
2. Develop backend APIs.
3. Add Websocket-based notifications.
4. Deploy on the cloud.   
#### Tech Stack

Node.js, React, MongoDB, Websockets   
     

### Chi tiết về việc xây dựng dự án

1.  Progressive Complexity : Projects grow trong difficulty from simple React apps (e.g., Task Tracker) to advanced, multi-featured applications (e.g., Capstone E-Commerce App).
2.  Full Stack Integration : Emphasizes both frontend và backend skills, including databases, APIs, và real-time communication.
3.  Deployment : Includes một deployment step (e.g., sử dụng Vercel, Heroku, hoặc AWS) to simulate production environments.
