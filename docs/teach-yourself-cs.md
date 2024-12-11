# Hướng dẫn bắt đầu học KHMT
Đây là các giáo trình tự học mà bạn có thể đọc, bài viết dưới đây sẽ là hướng dẫn của cá nhân mình cách bắt đầu tự học Khoa học máy tính dựa trên TeachYourselfCS. TeachYourselfCS ngắn hơn so với OSSU với đọc nhiều hơn nên đây sẽ là giáo trình mình lựa chọn (Tùy thuộc vào cách học của bạn mà có thể OSSU sẽ tốt hơn hoặc bạn muốn học hơn).

- [TeachYourselfCS](https://teachyourselfcs.com/)
- [ossu/computer-science](https://github.com/ossu/computer-science)
- [How to ACTUALLY learn CS](https://www.reddit.com/r/learnprogramming/comments/fnxyq7/how_to_actually_learn_cs) - Một bài viết chia sẻ trải nghiệm tự học của người này dựa trên các giáo trình trên.

## Hướng dẫn TeachYourselfCS

**CẬP NHẬT:** Mình thử tìm hiểu thêm thì thấy có khá nhiều vấn đề trong cách định hướng nên quyết định làm thêm mục dưới. Gợi ý của TYCS khá cô đọng, có đôi lúc bị nâng cao quá và ở một số phần mình thấy vẫn chưa cung cấp đủ các phần khác mà có thể bạn cần.

Tham gia cộng đồng tự học trên Discord để cùng trao đổi: [Khoa học máy tính!](https://discord.gg/x93EE354PB)

> Nếu việc tự học 9 chủ đề trong nhiều năm làm bạn cảm thấy quá sức, chúng tôi khuyên bạn chỉ nên tập trung vào hai cuốn sách: CS:APP và DDIA. Theo kinh nghiệm của chúng tôi, hai cuốn sách này mang lại hiệu quả cực kỳ cao trên tổng thời gian đầu tư học, đặc biệt cho các kỹ sư tự học và tốt nghiệp từ bootcamp làm việc trên các ứng dụng trực tuyến. Chúng cũng có thể được coi là chất xúc tác giúp bạn có động lực học các chủ đề còn lại.

### 1. Programming
Do bị loạn khi đọc sách nên t đi tìm một hướng tiếp cận khác, là sử dụng lộ trình được một người làm sẵn để học theo, có thể học song song cả bài giảng CS61A lẫn sách (Sẽ được đề cập thêm ở trong tài liệu được để đường dẫn ở đây): [Structure and Interpretation of Computer Programs](https://romanbird.github.io/sicp/) (Bao gồm cả Lab với Homework luôn). Lưu ý là sẽ sử dụng Scheme

### 2. Computer Architecture
Nếu mọi người muốn học thông qua bài giảng trên Youtube thì có một danh sách phát, dưới dạng Recording lại thôi: [Computer Systems: A programmer's Perspective](https://www.youtube.com/playlist?list=PLyboo2CCDSWnhzzzzDQ3OBPrRiIjl-aIE)

Một Repository hiếm hoi cho cuốn CS:APP: [Zhenye-Na/CSAPP-Labs](https://github.com/Zhenye-Na/CSAPP-Labs)

Có một ông trong phần bình luận trên Youtube của bài giảng gợi ý:

For anybody that doesn't want the watch the entire series and have some programming background the most worth while lectures are:

- Lecture 10: Program Optimization,
- Lecture 16: System Level IO
- Lecture 20: Dynamic Memory Allocation Advanced Concepts
- Lecture 23: Concurrent Programming

### 3. Data Structure and Algorithms
Chuyển qua về việc học DSA, cá nhân t thử nhìn qua khóa trên Youtube thì chất lượng khá thấp (Khóa trên Youtube là quay lại bài giảng với sách thì chưa đọc). T tìm cái gì đó dễ tiếp cận với các video được chia bite-sized để dễ tiếp thu thì có bộ video bài giảng của đại học Stanford về môn này, thiên về hướng hiểu thuật toán hơn là sử dụng một ngôn ngữ cụ thể:

- [Algorithms 1](https://www.youtube.com/playlist?list=PLXFMmlk03Dt7Q0xr1PIAriY5623cKiH7V)
- [Algorithms 2](https://www.youtube.com/playlist?list=PLXFMmlk03Dt5EMI2s2WQBsLsZl7A5HEK6)
Lấy slide bài giảng với các thông tin khác trên repo này: [AlessandroCorradini/Stanford-University-Algorithms-Design-and-Analysis](https://github.com/AlessandroCorradini/Stanford-University-Algorithms-Design-and-Analysis)

Luyện tập thì: [Solve Algorithms Code Challenges](https://www.hackerrank.com/domains/algorithms) (Hoặc có thể dùng Leetcode nhưng Leetcode có vẻ chuyên cho việc đi phỏng vấn hơn).


### 4. Toán
Về phần học toán, t đang khá phân vân nên là đây mới là định hướng thôi

- Phần liên quan nhất với CS là toán rời rạc, nên t sẽ bắt đầu trước từ cái này: <https://cims.nyu.edu/~regev/teaching/discrete_math_fall_2005/dmbook.pdf>
- Chuyển qua học đại số tuyến tính (Linear Algebra): [Essence of linear algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab).

Còn một gợi ý khác là học cuốn Math for Computer Science nhưng nó hơi nâng cao so với t nên bỏ qua

### 5. Hệ điều hành
Theo gợi ý từ TYCS:

> *Operating Systems: Three Easy Pieces* is a good alternative that's [freely available online](http://pages.cs.wisc.edu/~remzi/OSTEP/). We particularly like the structure and readability of the book, and feel that the exercises are worthwhile.

Thì bạn nên đọc [hướng dẫn cách học OSTEP (Viết tắt của Operating Systems: Three Easy Pieces) được viết bởi OSSU](https://github.com/ossu/computer-science/blob/master/coursepages/ostep/README.md).

Các repository lưu trữ phần Code và bài tập của sách:

- [ostep-code](https://github.com/remzi-arpacidusseau/ostep-code) 
- [ostep-homework](https://github.com/remzi-arpacidusseau/ostep-homework/)

Trên trang của OSTEP sẽ yêu cầu bạn tải từng chương của sách riêng biệt. Nếu bạn sử dụng MacOS/Linux hoặc bất kì OS nào hỗ trợ Bash, bạn hãy tải script [theagoliveira/OSTEP.sh](https://gist.github.com/theagoliveira/65980c144bf53cf8ee5e351bd827d7e7) và chạy để nó tự động tải hết tệp PDF về cho bạn.

### 6. Cơ sở dữ liệu
Gợi ý của bên trang hướng dẫn là xem bài giảng CS186: [CS186Berkeley](https://www.youtube.com/@CS186Berkeley/videos)

Vấn đề là định hướng học từ đâu và học thế nào thì không thấy đề cập trong trang, nên t sẽ bổ sung thêm là:

- Đọc Repo này trên Github để tìm Slide bài giảng các thứ: [Learning materials for UCB CS186](https://github.com/PKUFlyingPig/CS186)
- Tham khảo thêm lộ trình học khóa này (2024): [cs186berkeley](https://cs186berkeley.net/)
- [Các dự án trong khóa học: CS186 Projects](https://cs186.gitbook.io/project)

### 7. Mạng máy tính
Trong đúng một quyển là **Computer Networking: A Top-Down Approach**.

> Our favorite book on the topic is *[Computer Networking: A Top-Down Approach](https://smile.amazon.com/Computer-Networking-Top-Down-Approach-7th/dp/0133594149/)*. The small projects and exercises in the book are well worth doing, and we particularly like the "Wireshark labs", which they have [generously provided online](http://www-net.cs.umass.edu/wireshark-labs/).

Bạn có thể xem [video bài giảng miễn phí của Computer Networking: a Top-Down Approach](http://gaia.cs.umass.edu/kurose_ross/online_lectures.htm)

### 8. Ngôn ngữ và Trình biên dịch
Nếu bạn hiểu cách ngôn ngữ và trình biên dịch thực sự hoạt động, bạn sẽ viết mã tốt hơn và học ngôn ngữ mới dễ dàng hơn.

> Our suggested introductory text is the excellent *[Crafting Interpreters](https://craftinginterpreters.com/contents.html)* by Bob Nystrom, available for free online. It's well organized, highly entertaining, and well suited to those whose primary goal is simply to better understand their languages and language tools. We suggest taking the time to work through the whole thing, attempting whichever of the "challenges" sustain your interest.

Bạn có thể đọc thêm trên [Repo chính thức của sách](https://github.com/munificent/craftinginterpreters).

### 9. Hệ thống phân tán

Nếu bạn chọn đọc sách thì:

> Our suggested book for self-study is Martin Kleppmann's *[Designing Data-Intensive Applications](https://smile.amazon.com/Designing-Data-Intensive-Applications-Reliable-Maintainable-ebook/dp/B06XPJML5D/)*. Far better than a traditional textbook, DDIA is a highly readable book designed for practitioners, which somehow avoids sacrificing depth or rigor.

Một số tài nguyên khác:

- [Tóm tắt sách](https://github.com/awdoiudh/Designing-Data-Intensive-Applications-2nd-Edition/tree/main/en-us) - Bản Tiếng Trung (Bản gốc) sẽ được viết đầy đủ hơn.
- [Ghi chú học tập của một người học trên Github](https://github.com/keyvanakbary/learning-notes/blob/master/books/designing-data-intensive-applications.md)
- [bcherny/designing-data-intensive-application-notes.md](https://gist.github.com/bcherny/b870a60d1650973df7e400c8603ac76d)

Nếu bạn muốn học theo video bài giảng thì:

> For those who prefer video, an excellent course with videos available online is [MIT's 6.824](https://www.youtube.com/watch?v=cQP8WApzIQQ&list=PLrw6a1wE39_tb2fErI4-WkMbsvGQk9_UB), a graduate course taught by Robert Morris with readings available [here](https://pdos.csail.mit.edu/6.824/schedule.html).

## Các học phần khác trong chương trình chính
Phần này được trích dẫn trực tiếp từ [ossu/computer-science](https://github.com/ossu/computer-science)

### CS Tools
Understanding theory is important, but you will also be expected to create programs. There are a number of tools that are widely used to make that process easier. Learn them now to ease your future work writing programs.

**Topics covered**: `terminals and shell scripting` `vim` `command line environments` `version control` `and more`

| Courses | Duration | Effort | Prerequisites | Discussion |
| :-- | :-: | :-: | :-: | :-: |
| [The Missing Semester of Your CS Education](https://missing.csail.mit.edu/) | 2 weeks | 12 hours/week | - | [chat](https://discord.gg/5FvKycS) |


### Core security

**Topics covered** `Confidentiality, Integrity, Availability` `Secure Design` `Defensive Programming` `Threats and Attacks` `Network Security` `Cryptography` `and more`

| Courses | Duration | Effort | Prerequisites | Discussion |
| :-- | :-: | :-: | :-: | :-: |
| [Cybersecurity Fundamentals](https://www.edx.org/course/cybersecurity-fundamentals) | 8 weeks | 10-12 hours/week | - | [chat](https://discord.gg/XdY3AwTFK4) |
| [Principles of Secure Coding](https://www.coursera.org/learn/secure-coding-principles) | 4 weeks | 4 hours/week | - | [chat](https://discord.gg/5gMdeSK) |
| [Identifying Security Vulnerabilities](https://www.coursera.org/learn/identifying-security-vulnerabilities) | 4 weeks | 4 hours/week | - | [chat](https://discord.gg/V78MjUS) |

### Core ethics

**Topics covered**: `Social Context` `Analytical Tools` `Professional Ethics` `Intellectual Property` `Privacy and Civil Liberties` `and more`

| Courses | Duration | Effort | Prerequisites | Discussion |
| :-- | :-: | :-: | :-: | :-: |
| [Ethics, Technology and Engineering](https://www.coursera.org/learn/ethics-technology-engineering) | 9 weeks | 2 hours/week | none | [chat](https://discord.gg/6ttjPmzZbe) |
| [Introduction to Intellectual Property](https://www.coursera.org/learn/introduction-intellectual-property) | 4 weeks | 2 hours/week | none | [chat](https://discord.gg/YbuERswpAK) |
| [Data Privacy Fundamentals](https://www.coursera.org/learn/northeastern-data-privacy) | 3 weeks | 3 hours/week | none | [chat](https://discord.gg/64J34ajNBd) |

### Môn học cuối

[Software Engineering: Introduction](https://www.edx.org/learn/software-engineering/university-of-british-columbia-software-engineering-introduction). Cần học Core Programming, và có một [sizable project](https://github.com/ossu/computer-science/blob/master/FAQ.md#why-require-experience-with-a-sizable-project-before-the-Software-Engineering-courses)


## Học sâu hơn về các định hướng cụ thể (Chuyên ngành hẹp)

Ban đầu mình có theo OSSU nhưng nội dung lộ trình khá là nặng, nhưng mình vẫn gợi ý theo Advanced CS của bên họ cho từng mảng mà bạn muốn theo: [ossu/computer-science](https://github.com/ossu/computer-science?tab=readme-ov-file#advanced-cs)

