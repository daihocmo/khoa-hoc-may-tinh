Bài viết này được dịch từ bài viết gốc [How to Plan and Build a Programming Project - A Legitimate Guide for Beginners](plan.md). Vì bản dịch này sẽ là dịch cho cá nhân mình đọc nên là nếu mọi người đọc mà thấy có vấn đề ở đoạn nào thì gửi Issue hoặc Pull Request lên Github nha. 

# Cách lập kế hoạch và xây dựng dự án lập trình - Hướng dẫn cho người mới bắt đầu.

Bài viết này sẽ giải thích cách lập kế hoạch và xây dựng một dự án lập trình, cách chia nhỏ một dự án để bạn có thể bắt đầu thực hiện những dự án đỉnh của chóp nhằm giúp nâng cao kỹ năng lập trình.

Bài viết này sẽ không hướng dẫn cách cấu trúc thư mục, các practices tốt nhất để có thể xây dựng dự án hoặc cách cài đặt Extensions của VSCode để giúp đạt được clean code. Bài này được viết ra để giúp những người mới lập trình cảm thấy bớt sợ hãi hơn khi họ cố gắng thoát khỏi tutorial hell (tutorial hell, học quá nhiều nhưng không áp dụng) và xây dựng những dự án lập trình của riêng mình.

Khi mới bắt đầu thì đống dự án trông sẽ rất dễ khiến bạn nản. Khi mới bắt đầu học lập trình, tôi sẽ bắt đầu học một khóa học hoặc làm theo hướng dẫn và nghĩ rằng mình đã hiểu hướng dẫn. Tuy nhiên, khi ngừng xem và cố gắng tái tạo lại những gì đã học, nó chẳng đi đến đâu cả.

Để khắc phục điều này, tôi đã đăng sự thất vọng của mình lên subreddit [r/learnprogramming](https://www.reddit.com/r/learnprogramming/). Những phản hồi tôi nhận được đều tập trung vào việc xây dựng những dự án của riêng tôi. Lời khuyên này thoạt nghe có vẻ hay và là lời khuyên đúng đắn, tuy nhiên vấn đề đối với tôi là tôi thậm chí không thể xem hướng dẫn và tái tạo kết quả. Tôi phải xây dựng một dự án như thế nào? Một dự án cao hơn 10 cấp độ so với phần hướng dẫn và vào thời điểm đó, dường như những dự án đó vượt xa khả năng của tôi. Tôi thậm chí còn không biết phải bắt đầu như thế nào chứ đừng nói đến việc tôi sẽ kết hợp tất cả lại với nhau như thế nào. Vấn đề cơ bản là tôi không biết cách đi từ điểm A đến điểm B.

![](https://www.peterlunch.com/_next/image?url=%2Fimages%2FarticleImgs%2Fgood-example-of-build-something-800x467.png&w=1920&q=75)

Những người mới bắt đầu cảm thấy thất vọng vì dường như họ không thể thoát khỏi tutorial hell và vì vậy họ tìm kiếm lời khuyên. Tuy nhiên, những gì họ nhận được cũng có nghĩa là redditor đang ném thẳng vào phản hồi của những dự án xây dựng mà không hề cân nhắc rằng nếu người mới thậm chí không thể sao chép một hướng dẫn thì họ sẽ tạo dự án của riêng mình như thế nào. Trong thời gian học lập trình, tôi đã thấy rất nhiều ví dụ về cùng một câu hỏi mà tôi có và những câu trả lời giống nhau.

Để lập kế hoạch và xây dựng một dự án lập trình, hiện nay tôi sử dụng ba bước chính khi xây dựng dự án, vì vậy hãy bắt đầu với bước đầu tiên.

## Bước 1: Xác định dự án

Bước đầu tiên khi lập kế hoạch cho một dự án lập trình là xác định nó.

Định nghĩa dự án là một mô tả về dự án bằng ngôn ngữ viết. Nó phải cực kỳ đơn giản để bất kỳ ai đọc nó cũng có thể hiểu dự án nói về cái gì.

Khi bắt đầu định nghĩa dự án của mình, hãy tự hỏi 4 điều sau:

1. Dự án của bạn là gì và về cái gì?
2. [MVP](https://www.productplan.com/glossary/minimum-viable-product/) (Minimal Viable Product hay "Sản phẩm khả thi tối thiểu") của dự án đó là gì?
3. Sprinkles là gì?
4. Khi nào dự án sẽ hoàn thành?

> Sprinkles ở đây có nghĩa là rắc, và nó không liên quan gì đến thuật ngữ Tiếng Anh chuyên ngành đâu. Ở đây có thể hiểu Sprinkles là "trang trí dự án của bạn thêm lung linh" (Đọc tiếp sẽ rõ). 

### Doughnut (MVP) before the sprinkles

Một trong những bài học mà tôi đã học được ngay từ đầu khóa bootcamp của mình là ta cần có bánh donut thì mới có thể rắc tiêu lên được.

![three donuts on table with sprinkles](https://www.peterlunch.com/_next/image?url=%2Fimages%2FarticleImgs%2Fpatrick-fore-ZmH0g1ievTg-unsplash.jpg&w=1920&q=75)

Có thể bạn luôn muốn làm cho một cái gì đó trông thật ngầu và thêm các tính năng hay. Tuy nhiên, nếu ứng dụng của bạn không hoàn thành được các chức năng cơ bản thì những tính năng tuyệt vời đó sẽ chẳng đi đến đâu cả. The sprinkles have no doughnut to go on.

Vì vậy, hãy đảm bảo rằng bạn xác định được MVP là gì trước khi bắt đầu quá trình sprinkles của mình.

### Một bản định nghĩa dự án mẫu

Để đưa ra một ví dụ đơn giản, giả sử chúng ta sắp xây dựng một ứng dụng máy tính (calculator), chúng ta sẽ có định nghĩa dự án cơ bản như bên dưới:

**Dự án ứng dụng máy tính**

*Dự án của bạn là gì và về cái gì?* - Dự án máy tính là một dự án xây dựng một máy tính có thể truy cập trên trình duyệt. Dự án sẽ được xây dựng bằng HTML, CSS và JavaScript. Nó sẽ cho phép người dùng nhập số và tính kết quả của những số đó dựa trên phép toán mà họ chọn.

*MVP là gì?* -  là một máy tính hiển thị trong trình duyệt web có thể thực hiện các phép tính cộng, trừ, nhân và chia dựa trên input của người dùng và hiển thị cho người dùng kết quả của phép tính ấy.

*Sprinkles là gì?* - Là styling cho ứng dụng máy tính, nhận Input từ bàn phím chứ không chỉ là bấm các nút ở trên màn hình. Đồng thời một số các chức năng cao cấp hơn ví dụ như là tính số mũ của x.

* Khi nào dự án sẽ hoàn thành? -* Dự án sẽ hoàn thành sau khi tất cả các tính năng MVP đã được implemented và ứng dụng máy tính đã được viết thiết kế giao diện xong (Ở đây hiểu từ "thiết kế" là hoàn thành viết phần HTML/CSS cho máy tính đó).

Định nghĩa trên rất đơn giản và dễ hiểu. Nếu mẹ tôi nhặt nó lên, bà sẽ hiểu dự án đó là gì. Cô ấy sẽ hiểu vì nó cho bạn biết dự án là gì, các tính năng MVP mà bạn phải xây dựng, điều thú vị khi có các tính năng và khi nào nó sẽ hoàn thành. Bằng cách xác định dự án, bạn sẽ làm cho dự án bớt đáng sợ hơn.

Khi bạn đã xác định được dự án, bạn có thể bắt đầu bước tiếp theo.

## Bước 2: Tạo quy trình làm việc

Bước tiếp theo là đơn giản nhất. Thông thường, bước này có thể được kết hợp với bước 3. Tuy nhiên, bây giờ chúng ta sẽ xem nó ở đây như một bước riêng biệt để tôi có thể chỉ cho bạn cách thiết lập quy trình làm việc rất cơ bản cho những dự án của riêng bạn. Khi bạn đã thực hiện nó một lần, nó có thể là bước mặc định cho những dự án còn lại của bạn.

Sử dụng một công cụ miễn phí như [Trello](https://trello.com/) để quản lý dự án, sử dụng khung quy trình làm việc [Kanban](https://www.atlassian.com/agile/kanban). Bạn không cần phải biết hoặc hiểu Kanban là gì khi mới bắt đầu, bạn chỉ cần sử dụng như cách làm ở đây.

Để xây dựng bảng Kanban, hãy tạo 4 cột:

1.  TODO (Cần làm)
2.  DOING (Đang làm)
3.  DONE (Đã làm xong)
4.  BUGS / NOT SURE HOW TO DO (Lỗi, không biết nên làm gì)

![Trello kanban board with 4 columns todo, doing, done and bugs.](https://www.peterlunch.com/_next/image?url=%2Fimages%2FarticleImgs%2Fkanban-1-800x415.png&w=1920&q=75)


Trong các cột này, chúng ta sẽ thêm thẻ. Khi làm việc trên các thẻ đó, chúng ta sẽ chuyển chúng vào cột **DOING** và sau khi hoàn thành thẻ đó, chúng ta có thể chuyển nó sang cột **DONE**. Nếu bạn gặp phải một lỗi nào đó hoặc không chắc chắn về cách thực hiện điều gì đó, chúng ta có thể chuyển lỗi đó sang cột **BUGS / NOT SURE HOW TO DO**.

Quy trình này là một phiên bản siêu đơn giản của Kanban và khi làm việc với vai trò là một developer, rất có thể bạn sẽ có nhiều cột hơn như testing, coding review, backlog và các cột khác. Tuy nhiên, đối với những dự án cá nhân và đặc biệt là với người mới bắt đầu, chỉ cần như này là đủ.

Bây giờ chúng ta đã thiết lập xong quy trình làm việc, chúng ta có thể bắt đầu bước cuối cùng.

## Bước 3: Chia dự án thành các phần nhỏ hơn

Chìa khóa để xây dựng những dự án của riêng bạn bắt đầu bằng việc chia dự án lớn thành các phần nhỏ hơn, ít đáng sợ hơn. Những thành phần nhỏ hơn này sẽ trở thành thẻ của chúng ta từ bước 2.

Bây giờ điều này nghe có vẻ đơn giản, nhưng khi tôi mới bắt đầu, tôi đã không nghĩ rằng bạn có thể làm được điều này. Tôi nghĩ hầu hết các nhà phát triển chỉ mới bắt đầu lập trình và dự án được thực hiện từ họ giống như bạn thấy trong phim. Tôi nghĩ đó là điều tôi phải làm được. Tuy nhiên, bây giờ tôi đã có cơ hội làm việc trong ngành này, tôi biết điều đó chắc chắn không phải như vậy, trên thực tế, một nhà phát triển giỏi sẽ chia dự án đó thành các nhiệm vụ nhỏ hơn.

![estefannie giả vờ lập trình như trong phim](https://www.peterlunch.com/_next/image?url=%2Fimages%2FarticleImgs%2Fgiphy-downsized.gif&w=1080&q=75)

Tuy nhiên, là người mới bắt đầu, có thể khó biết cách chia nhỏ một việc gì đó thành các nhiệm vụ nhỏ hơn. Nếu bạn không biết cách thực sự xây dựng dự án thì làm sao bạn có thể chia nhỏ nó?

Chà, điều đầu tiên bạn cần làm là xem xét định nghĩa dự án của mình và sau đó chia nó thành các phần nhỏ hơn.

Hãy tiếp tục sử dụng ví dụ về ứng dụng máy tính để tạo các thẻ thành phần của chúng ta:

1. Hàm tính toán – MVP
2. Nhận thông tin đầu vào của người dùng - MVP
3. Giao diện người dùng HTML - MVP
4. Tạo kiểu CSS cho giao diện người dùng - rắc ✨
5. Trình nghe sự kiện JavaScript - MVP
6. Thêm hình động cho phép tính - rắc ✨

![bảng trello với thẻ việc cần làm từ danh sách trên](https://www.peterlunch.com/_next/image?url=%2Fimages%2FarticleImgs%2Fkanban-2-800x373.png&w=1920&q=75)

Bạn sẽ nhận thấy rằng đối với mỗi thẻ, chúng ta đã gán nhãn MVP hoặc nhãn rắc. Điều này nhằm giúp bạn nhìn thấy một cách trực quan những thẻ nào là quan trọng nhất và do đó thẻ nào nên được sử dụng đầu tiên.

Lợi ích lớn nhất của các tấm thẻ là chúng đã đơn giản hóa những gì chúng ta phải làm rồi. Điều này làm cho những dự án bớt đáng sợ hơn vì bạn không tạo ra một ứng dụng máy tính lớn gây khó chịu, thay vào đó bạn đang thực hiện 6 dự án nhỏ hơn sẽ kết hợp để tạo ra một dự án lớn.

Khi bạn làm việc trên một tấm thẻ, bạn sẽ di chuyển nó vào cột đang làm. Dành thời gian để thành phần hoạt động trước khi bạn chuyển sang thẻ tiếp theo.

Nhưng chúng ta vẫn chưa hoàn thành, chúng ta có thể đơn giản hóa và cải thiện quy trình làm việc của mình hơn nữa để đảm bảo rằng chúng ta không bị cản trở bởi quy mô của dự án khi xây dựng.

### Chia từng thành phần thành các danh sách kiểm tra nhỏ hơn

Sau khi có thẻ cấp cao, chúng ta có thể chia các thành phần đó thành các nhiệm vụ nhỏ hơn bằng cách chia các nhiệm vụ đó thành danh sách kiểm tra để chúng ta có thể theo dõi tiến trình của mình.

Ví dụ dưới đây chỉ là cách bộ não của tôi hoạt động để bạn có thể chia nó thành những phần nhỏ hơn hoặc lớn hơn tùy thuộc vào điều gì phù hợp với bạn. Hãy sử dụng thẻ chức năng tính toán làm ví dụ về cách chia nhỏ một thành phần hơn nữa.

Vì nhiệm vụ này là nhiệm vụ MVP và tôi đã xác định MVP là các phép tính cơ bản cộng, trừ, nhân và chia nên chúng ta cần thêm các hàm đó vào danh sách kiểm tra.

![Danh sách kiểm tra các nhiệm vụ cần hoàn thành](https://www.peterlunch.com/_next/image?url=%2Fimages%2FarticleImgs%2Fkanban-3-600x483.png&w=1200&q=75)

Bây giờ chúng ta đã chia thẻ chức năng tính toán thành 4 dự án nhỏ mà chúng ta có thể thực hiện. Điều đó dễ dàng hơn nhiều so với nhiệm vụ trừu tượng và cực kỳ khó khăn là xây dựng một ứng dụng máy tính hoặc thậm chí viết các chức năng của máy tính (thẻ).

Bây giờ chúng ta có thể tập trung và tìm ra cách thực hiện từng chức năng này. Khi làm điều đó, chúng ta có thể kiểm tra những mục đó, mang lại cho chúng ta cảm giác hoàn thành và tiến bộ. Sau đó, khi chúng ta đã hoàn thành tất cả bốn mục đó, chúng ta có thể di chuyển thẻ đó vào cột đã hoàn thành và bẻ khóa thẻ tiếp theo.

Từ đây trở đi chúng ta chỉ cần lặp lại quy trình cho mỗi thẻ. Tuy nhiên, bạn không nên dành nhiều thời gian để cố gắng làm cho mỗi thẻ có mọi nhiệm vụ riêng lẻ, điều này khiến tôi mắc phải sai lầm mà tôi đã mắc phải khi bắt đầu.

### Đừng mắc kẹt trong việc làm cho nó trở nên hoàn hảo

Khi bạn chia các thẻ và các nhiệm vụ trong danh sách kiểm tra, đừng gặp khó khăn khi cố gắng đảm bảo rằng bạn có mọi chức năng và chi tiết nhỏ được chia nhỏ.

Nếu làm như vậy, bạn có thể sẽ bị mắc kẹt trong các giai đoạn lập kế hoạch và sẽ không bao giờ chuyển sang giai đoạn xây dựng, nếu không giai đoạn xây dựng của bạn sẽ quá cứng nhắc. Bạn cần một số khoảng trống trong những dự án của mình.

Điều tôi nhận thấy khi thực hiện những dự án của mình là tôi thường xuyên phải thêm nhiều thẻ và nhiệm vụ hơn khi thực hiện. Điều này là không thể tránh khỏi, bạn đang xây dựng một thứ gì đó lần đầu tiên nên bạn sẽ không biết chính xác những gì bạn cần xây dựng trước khi bắt đầu.

Ví dụ: bạn có thể không có thẻ tạo kiểu khi lần đầu tiên bắt đầu lập kế hoạch cho ứng dụng máy tính của mình và chỉ nhận ra sau khi hoàn thành thẻ khung HTML rằng bạn có thể nên tạo kiểu cho ứng dụng.

Vì vậy, đừng mắc kẹt trong việc thực hiện kế hoạch hoàn hảo, hãy viết đủ để bạn có thể bắt đầu và bổ sung thêm khi thực hiện. Bạn cũng có thể sử dụng cột **lỗi/không biết** để đặt những thẻ mà bạn chưa thể làm được hoặc những thẻ bạn đang mắc kẹt để giúp bạn tiếp tục di chuyển.

## Bắt đầu xây dựng dự án lập trình của bạn

Bây giờ bạn đã có các công cụ hợp pháp để lập kế hoạch và xây dựng một dự án lập trình khi mới bắt đầu. Hy vọng bài đăng này đã làm cho khái niệm xây dựng dự án bớt trừu tượng và đáng sợ hơn.

Điều quan trọng là xác định rõ ràng dự án, thiết lập quy trình làm việc của bạn và sau đó chia dự án thành các thành phần nhỏ hơn để tạo ra dự án lớn hơn. Bằng cách đó, dự án không giống như một ngọn núi khổng lồ để leo lên, thay vào đó, nó sẽ giống như một chiếc thang với mỗi bước giúp bạn đạt được mục tiêu của mình.

Nếu bạn thấy ai đó đang gặp khó khăn để thoát khỏi tutorial hell, đừng chỉ bảo họ xây dựng. Nói cho họ biết cách lập kế hoạch và xây dựng.

Lập kế hoạch là điều tuyệt vời, nhưng điều quan trọng là sau đó hãy bắt đầu và xây dựng. Vì vậy, hãy tiếp tục xây dựng những dự án tuyệt vời, đồng thời nâng cao kỹ năng lập trình của bạn và chia sẻ tiến trình của bạn với tôi trên [twitter](https://twitter.com/thelynchpinau).
