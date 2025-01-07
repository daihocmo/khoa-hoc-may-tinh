---
hide:
  - navigation
---

# Hướng dẫn bắt đầu học KHMT
Đây là các giáo trình tự học mà bạn có thể đọc, bài viết dưới đây sẽ là hướng dẫn của cá nhân mình cách bắt đầu tự học Khoa học máy tính dựa trên TeachYourselfCS. TeachYourselfCS ngắn hơn so với OSSU với đọc nhiều hơn nên đây sẽ là giáo trình mình lựa chọn (Tùy thuộc vào cách học của bạn mà có thể OSSU sẽ tốt hơn hoặc bạn muốn học hơn).

- [TeachYourselfCS](https://teachyourselfcs.com/)
- [ossu/computer-science](https://github.com/ossu/computer-science)
- [How to ACTUALLY learn CS](https://www.reddit.com/r/learnprogramming/comments/fnxyq7/how_to_actually_learn_cs) - Một bài viết chia sẻ trải nghiệm tự học của người này dựa trên các giáo trình trên.

## Hướng dẫn TeachYourselfCS

**CẬP NHẬT:** Mình thử tìm hiểu thêm thì thấy có khá nhiều vấn đề trong cách định hướng nên quyết định làm thêm mục dưới. Gợi ý của TYCS khá cô đọng, có đôi lúc bị nâng cao quá và ở một số phần mình thấy vẫn chưa cung cấp đủ các phần khác mà có thể bạn cần.

Tham gia cộng đồng tự học trên Discord để cùng trao đổi: [Khoa học máy tính!](https://discord.gg/x93EE354PB)

> TYCS: TeachYourselfCS (Từ giờ trong hướng dẫn sẽ viết tắt như vậy)

### 1. Programming
Gợi ý của TYCS là cuốn [Structure and Interpretation of Computer Programs](https://sarabander.github.io/sicp/html/index.xhtml). 

Đọc hướng dẫn học cuốn sách này của romanbird: [Structure and Interpretation of Computer Programs](https://romanbird.github.io/sicp/) (Bao gồm cả Lab với Homework luôn). Hướng dẫn học này sẽ sử dụng cả bài giảng CS61A nữa (Còn kho bài giảng trên MIT nhưng TYCS gợi ý CS61A hơn).

### 2. Computer Architecture
Có hai lựa chọn cho mọi người: 

- [Nand2Tetris](https://www.nand2tetris.org/course)
  - Có thể bạn sẽ muốn đọc [nand2tetris: a book review and recap](https://sevko.io/articles/nand-2-tetris/)
  - Trong trang chủ của Nand2Tetris thì sẽ được chia ra làm hai nửa: Hardware và Software. Phần Hardware là 6 chương đầu còn 6 chương còn lại là về Software. Bạn có thể đọc miễn phí 6 chương đầu trên trang chủ.
  - 6 chương sau của cuốn sách có thể được học trong khóa [Build a Modern Computer from First Principles: Nand to Tetris Part II (project-centered course)](https://www.coursera.org/learn/nand2tetris2)
- CS:APP: Tui chọn Nand2Tetris vì nó miễn phí ;-; 
  - Bài giảng của [Computer Systems: A programmer's Perspective](https://www.youtube.com/playlist?list=PLyboo2CCDSWnhzzzzDQ3OBPrRiIjl-aIE) trên Youtube.
  - Một Repository hiếm hoi cho cuốn CS:APP: [Zhenye-Na/CSAPP-Labs](https://github.com/Zhenye-Na/CSAPP-Labs)

> In seeking simplicity and cohesiveness, Nand2Tetris trades off depth. In particular, two very important concepts in modern computer architectures are pipelining and memory hierarchy, but both are mostly absent from the text.

Đây là bài giảng cho [memory hierarchy](https://www.youtube.com/watch?v=zDJxqQ3J8r0&list=PLyboo2CCDSWnhzzzzDQ3OBPrRiIjl-aIE&index=11&pp=iAQB) từ cuốn CS:APP.

> For anybody that doesn't want the watch the entire series and have some programming background the most worth while lectures are:
>
> - Lecture 10: Program Optimization,
> - Lecture 16: System Level IO
> - Lecture 20: Dynamic Memory Allocation Advanced Concepts
> - Lecture 23: Concurrent Programming

(Cho những người xem Lectures của CS:APP ở trên).

### 3. Data Structure and Algorithms
TYCS gợi ý học cuốn [The Algorithm Design Manual](https://www8.cs.umu.se/kurser/TDBAfl/VT06/algorithms/BOOK/BOOK/BOOK.HTM) (Có thể đọc miễn phí trên trang web này)

Bạn có thể truy cập trang [The Algorithms](https://the-algorithms.com/) để tìm cách áp dụng thuật toán bất kì trong ngôn ngữ yêu thích của bạn.

Cho những người muốn xem video bài giảng, thì đây là bài giảng của [Tim Roughgarden](http://timroughgarden.org/videos.html).

- [Algorithms 1](https://www.youtube.com/playlist?list=PLXFMmlk03Dt7Q0xr1PIAriY5623cKiH7V)
- [Algorithms 2](https://www.youtube.com/playlist?list=PLXFMmlk03Dt5EMI2s2WQBsLsZl7A5HEK6)
- Lấy slide bài giảng với các thông tin khác trên repo này: [AlessandroCorradini/Stanford-University-Algorithms-Design-and-Analysis](https://github.com/AlessandroCorradini/Stanford-University-Algorithms-Design-and-Analysis)

> For practice, our preferred approach is for students to solve problems on [Leetcode](http://leetcode.com/). These tend to be interesting problems with decent accompanying solutions and discussions. They also help you test progress against questions that are commonly used in technical interviews at the more competitive software companies. We suggest solving around 100 random leetcode problems as part of your studies.
> 
> Finally, we strongly recommend *[How to Solve It](https://smile.amazon.com/How-Solve-Mathematical-Princeton-Science/dp/069116407X/)* as an excellent and unique guide to general problem solving; it's as applicable to computer science as it is to mathematics.

### 4. Toán

1. Discrete mathematics: Đọc [lecture notes by László Lovász](https://cims.nyu.edu/~regev/teaching/discrete_math_fall_2005/dmbook.pdf)
2. Chuyển qua học đại số tuyến tính (Linear Algebra): [Essence of linear algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab).
3. For a more advanced treatment, we suggest *[Mathematics for Computer Science](https://courses.csail.mit.edu/6.042/spring18/mcs.pdf)*, the book-length lecture notes for the MIT course of the same name. That course's video lectures are also [freely available](https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2010/video_galleries/video-lectures/), and are our recommended video lectures for discrete math.

### 5. Hệ điều hành
Theo gợi ý từ TYCS:

> *Operating Systems: Three Easy Pieces* is a good alternative that's [freely available online](http://pages.cs.wisc.edu/~remzi/OSTEP/). We particularly like the structure and readability of the book, and feel that the exercises are worthwhile.

Đọc [hướng dẫn cách học OSTEP (Viết tắt của Operating Systems: Three Easy Pieces) được viết bởi OSSU](https://github.com/ossu/computer-science/blob/master/coursepages/ostep/README.md).

Các repository lưu trữ phần Code và bài tập của sách:

- [ostep-code](https://github.com/remzi-arpacidusseau/ostep-code) 
- [ostep-homework](https://github.com/remzi-arpacidusseau/ostep-homework/)


### 6. Cơ sở dữ liệu
Gợi ý của bên trang hướng dẫn là xem bài giảng CS186: [CS186Berkeley](https://www.youtube.com/@CS186Berkeley/videos)

Vấn đề là định hướng học từ đâu và học thế nào thì không thấy đề cập trong trang, nên t sẽ bổ sung thêm là:

- Đọc Repo này trên Github để tìm Slide bài giảng các thứ: [Learning materials for UCB CS186](https://github.com/PKUFlyingPig/CS186)
- Tham khảo thêm lộ trình học khóa này (2024): [cs186berkeley](https://cs186berkeley.net/)
- [Các dự án trong khóa học: CS186 Projects](https://cs186.gitbook.io/project)

### 7. Mạng máy tính
Trong đúng một quyển là **Computer Networking: A Top-Down Approach**.

> Our favorite book on the topic is *[Computer Networking: A Top-Down Approach](https://smile.amazon.com/Computer-Networking-Top-Down-Approach-7th/dp/0133594149/)*. The small projects and exercises in the book are well worth doing, and we particularly like the "Wireshark labs", which they have [generously provided online](http://www-net.cs.umass.edu/wireshark-labs/).

Tài nguyên học
- Bạn có thể xem [video bài giảng miễn phí của Computer Networking: a Top-Down Approach](http://gaia.cs.umass.edu/kurose_ross/online_lectures.htm)
- [Lecture notes của sách trên](https://github.com/VasanthVanan/computer-networking-top-down-approach-notes)

### 8. Ngôn ngữ và Trình biên dịch
Nếu bạn hiểu cách ngôn ngữ và trình biên dịch thực sự hoạt động, bạn sẽ viết mã tốt hơn và học ngôn ngữ mới dễ dàng hơn.

> Our suggested introductory text is the excellent *[Crafting Interpreters](https://craftinginterpreters.com/contents.html)* by Bob Nystrom, available for free online. It's well organized, highly entertaining, and well suited to those whose primary goal is simply to better understand their languages and language tools. We suggest taking the time to work through the whole thing, attempting whichever of the "challenges" sustain your interest.

Bạn có thể đọc thêm trên [Repo chính thức của sách](https://github.com/munificent/craftinginterpreters).

### 9. Hệ thống phân tán

Nếu bạn chọn đọc sách thì:

> Our suggested book for self-study is Martin Kleppmann's *[Designing Data-Intensive Applications](https://smile.amazon.com/Designing-Data-Intensive-Applications-Reliable-Maintainable-ebook/dp/B06XPJML5D/)*. Far better than a traditional textbook, DDIA is a highly readable book designed for practitioners, which somehow avoids sacrificing depth or rigor.

Một số tài nguyên khác:

- [Ghi chú học tập của một người học trên Github](https://github.com/keyvanakbary/learning-notes/blob/master/books/designing-data-intensive-applications.md)

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

