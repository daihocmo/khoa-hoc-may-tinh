# Bài nhập môn

### Trước khi bắt đầu

Nếu bạn muốn tham gia vào thế giới lập trình, bạn cần nắm vững những kiến thức cơ bản về lập trình.

Có một sự khác biệt lớn giữa *học lập trình* và *học một vài ngôn ngữ lập trình*. Bạn có thể "học" hai ngôn ngữ lập trình, nhưng vẫn chưa thực sự *biết lập trình*.

Học một ngôn ngữ lập trình cũng giống như học một ngoại ngữ. Học lập trình giống như học cách tư duy. **Khả năng tư duy không bị giới hạn hay quyết định bởi bất kỳ ngôn ngữ nào**. Nếu bạn học một ngôn ngữ mới, khả năng tư duy của bạn không thay đổi. Lập trình cũng tương tự. Các khái niệm lập trình không phụ thuộc vào ngôn ngữ lập trình cụ thể.

Bài viết này sẽ tập trung vào các khái niệm lập trình, giúp bạn học được bất kỳ ngôn ngữ lập trình nào. Học theo cách này nhanh hơn nhiều và bạn không bị phân tâm bởi cú pháp của từng ngôn ngữ.

### Tư duy như một lập trình viên

Chúng ta có thể sử dụng **phương pháp tiếp cận thuật toán** để giải quyết vấn đề.

[Lập trình máy tính](https://en.wikipedia.org/wiki/Computer_programming) là quá trình thiết kế và xây dựng một chương trình máy tính có thể chạy được. Một chương trình máy tính là **tập hợp các chỉ dẫn** mà máy tính có thể thực thi để hoàn thành một nhiệm vụ cụ thể.

Nói một cách đơn giản, lập trình là việc hướng dẫn máy tính những việc cần làm. Để mô tả cho máy tính biết nó cần làm gì, các lập trình viên sử dụng nhiều ngôn ngữ lập trình khác nhau.

Bây giờ, hãy lấy giấy bút hoặc mở một trình soạn thảo văn bản bất kỳ và viết ra tất cả các bước bạn cần thực hiện để nấu một bát mì gói thơm ngon, giá rẻ cho sinh viên nghèo. Đây là ví dụ của tôi:

* Đến tủ bếp và mở cửa tủ.
* Lấy một gói mì (ở đây tôi lấy mì Hảo Hảo).
* Đóng cửa tủ bếp.
* Mở tủ đựng dụng cụ bếp.
* Lấy thìa, đũa, chảo, nồi.
* Đóng tủ đựng dụng cụ bếp.
* Mở tủ lạnh.
* Lấy các nguyên liệu khác: xúc xích, trứng, giò.
* Đóng tủ lạnh.
* Thái xúc xích, giò.
* Rán trứng.
* Rán xúc xích và giò.
* Đun nước.
* Cho mì vào nồi nấu sơ qua.
* Cho các nguyên liệu đã chế biến vào nồi mì.

Như vậy là xong

Đây là cách các lập trình viên tư duy. Bạn có thể thấy nó không phức tạp và ai cũng có thể làm được. Trong các bước trên, có một số trường hợp bổ sung mà tôi đã bỏ qua để đơn giản hóa, ví dụ như nếu không có sữa trong tủ lạnh thì sao, nếu bạn hết sữa hoặc ngũ cốc thì sao, nếu bạn không có thìa hoặc bát sạch thì sao, nếu bạn làm rơi và vỡ bát, v.v.

Nhưng bạn đã hiểu ý chính rồi. Và trong video sau, bạn sẽ thấy điều gì xảy ra nếu bạn không cụ thể và chi tiết khi viết chỉ dẫn (hoặc code). Hãy xem video này:

[https://www.youtube.com/watch?v=cDA3_5982h8](https://www.youtube.com/watch?v=cDA3_5982h8)

Đây là cách lập trình hoạt động (đa phần thời gian là vậy). Bạn biết mình phải làm gì, bạn viết code cho việc đó, sau đó bạn kiểm tra xem nó có hoạt động như mong muốn không. Nếu không, bạn biết mình đã làm sai điều gì đó. Bạn thay đổi code và thử lại cho đến khi có được giải pháp đúng.

### Thuật toán

Thuật toán là một tập hợp các quy trình từng bước được xác định rõ ràng, đưa ra câu trả lời đúng cho một vấn đề cụ thể.

Một thuật toán hợp lệ cần đáp ứng các điều kiện sau:

* Với cùng input, luôn tạo ra cùng một output.
* Phải rõ ràng, được định nghĩa rành mạch và chỉ có một cách diễn giải duy nhất.
* Phải hữu hạn, nghĩa là cần được thực hiện trong một khoảng thời gian hữu hạn và sử dụng không gian hữu hạn.

Ví dụ điển hình nhất về thuật toán mà bạn đã thấy trong cuộc sống là công thức nấu ăn. Bạn biết cần bao lâu để nấu món ăn đó, cần những nguyên liệu nào và cần chuẩn bị chúng theo thứ tự nào. Nếu bạn làm theo công thức đó hai lần và nấu món ăn theo cùng một cách chính xác, cả hai lần bạn sẽ có được cùng một món ăn.

Để giải quyết các nhiệm vụ bằng lập trình, điều đầu tiên chúng ta cần làm là thiết kế một thuật toán. Khi làm điều đó, bạn nên viết nó ra. Có hai cách để viết thuật toán: bằng sơ đồ khối và bằng code giả.

### Sơ đồ khối (Flowchart)

[Sơ đồ khối](https://en.wikipedia.org/wiki/Flowchart) (Flowchart) là một loại sơ đồ biểu diễn quy trình làm việc hoặc quy trình. Sơ đồ khối cũng có thể được định nghĩa là biểu diễn bằng sơ đồ của một thuật toán, một cách tiếp cận từng bước để giải quyết một nhiệm vụ.

Mỗi sơ đồ khối bao gồm các khối xây dựng. Để hiểu sơ đồ khối, trước tiên bạn cần biết ý nghĩa của từng khối xây dựng. Tôi đã tạo bảng đơn giản này để bạn có thể tham khảo bất cứ lúc nào cho đến khi bạn nắm vững tất cả.

Như bạn thấy, không có nhiều khối trong sơ đồ khối. Một số khối khác tồn tại, nhưng hiện tại chúng không quan trọng. Tôi sẽ chỉ cho bạn cách giải quyết các nhiệm vụ chỉ bằng các ký hiệu này. Hãy bắt đầu với các ví dụ.

### Tuần tự (Sequence)

Các chỉ dẫn trong chương trình được thực thi theo thứ tự chúng được viết. Hãy tạo sơ đồ khối cho một nhiệm vụ đơn giản, trong đó người dùng sẽ nhập hai số và chương trình sẽ in ra tổng của hai số đó.

### Phân nhánh (Branch)

Nếu một phần code nào đó trong thuật toán chỉ cần được thực thi khi một số điều kiện được đáp ứng, chúng ta cần sử dụng phân nhánh. Với phân nhánh, chúng ta có thể chia code thành hai hoặc nhiều đường dẫn. Để minh họa ví dụ về phân nhánh, hãy tạo sơ đồ khối cho một chương trình nhận input của người dùng là một số và in ra "Số là số dương" hoặc "Số là số âm".

### Vòng lặp (Loop)

Đôi khi trong code, chúng ta cần thực hiện cùng một việc nhiều lần. Chúng ta luôn có hai lựa chọn. Một là viết cùng một code nhiều lần, hai là sử dụng vòng lặp. Vấn đề với việc viết cùng một code nhiều lần là nó không gọn gàng và tốn thời gian. Đó là lý do tại sao chúng ta nên sử dụng vòng lặp.

Trong lập trình máy tính, vòng lặp là một chuỗi các lệnh được lặp lại liên tục cho đến khi đạt được một điều kiện nhất định. Phần lớn thời gian, chúng ta viết một vòng lặp với một loại bộ đếm nào đó để vòng lặp biết cần thực hiện cùng một code bao nhiêu lần và khi nào thì dừng. Hãy tạo sơ đồ khối cho một chương trình nhận một số làm input của người dùng và in ra tất cả các số (nguyên) giữa 0 và số đó.

Như bạn thấy, vòng lặp lặp lại ba bước: kiểm tra xem biến A có nhỏ hơn biến Counter không, in giá trị của biến Counter và tăng giá trị của biến Counter thêm một.

**Bây giờ, hãy thử tự giải quyết nhiệm vụ này:** Tạo một chương trình nhận input của người dùng và kiểm tra xem đó có phải là số 0 không. Nếu không phải, hãy in bình phương của số đó và nếu là 0 thì kết thúc chương trình.

### Biến số (Variable)

Trong các bài tập trước, tôi luôn đề cập đến biến số, nhưng chưa bao giờ giải thích biến số là gì. Biến số là các vị trí trong bộ nhớ có tên và là nơi chúng ta lưu trữ dữ liệu từ input. Giá trị của mỗi biến số có thể thay đổi trong quá trình thực thi chương trình. Để truy cập giá trị của một biến số, chúng ta chỉ cần viết tên của biến số đó.

Mỗi biến số có tên, giá trị và kiểu. Tôi sẽ nói về kiểu dữ liệu sau. Để gán giá trị cho một biến số, chúng ta cần viết tên biến số, sau đó là dấu bằng '=' và sau đó là giá trị.

Ví dụ:

Để gán giá trị 10 cho một biến số có tên 'tuổi', ta chỉ cần viết `tuổi = 10`.

Nếu muốn thay đổi giá trị của biến số 'tuổi', ta có thể làm tương tự: `tuổi = 30`. Điều đó được gọi là gán lại.

Luôn nên đặt tên biến số một cách mô tả thay vì chỉ sử dụng một chữ cái như 'A' hoặc 'x'.

### Kiểu dữ liệu (Data type)

Trong khoa học máy tính và lập trình máy tính, [kiểu dữ liệu](https://en.wikipedia.org/wiki/Data_type) hay đơn giản là kiểu là một thuộc tính của dữ liệu, cho máy tính biết cách lập trình viên định sử dụng dữ liệu. Tôi sẽ không làm phiền bạn với các chi tiết, bạn chỉ cần nhớ năm kiểu dữ liệu phổ biến sau:

* Số nguyên (int): Kiểu dữ liệu này được sử dụng cho các số nguyên. Ví dụ: `int age = 20` hoặc `int size = 10`.
* Chuỗi (string): Kiểu dữ liệu này được sử dụng cho văn bản hoặc chuỗi ký tự. Ví dụ: `string name = "John Doe"` hoặc `string sentence = "Today is a sunny day."`. Thông thường, một chuỗi luôn được bao quanh bởi dấu ngoặc kép.
* Ký tự (char): Kiểu dữ liệu này được sử dụng cho một chữ cái duy nhất. `char letter = 'a'`.
* Số thực dấu phẩy động (float): Kiểu dữ liệu này được sử dụng cho các số chứa dấu thập phân. Ví dụ: `float number = 3.14`.
* Boolean (bool): Kiểu dữ liệu này chỉ được sử dụng cho True hoặc False (đúng hoặc sai, 0 hoặc 1). Ví dụ: `bool flag = True`.

Như tôi đã đề cập trước đó, mỗi biến số có một tên, một giá trị và một kiểu. Khi tôi viết:

`int age = 10`

`int` là kiểu của biến số, `age` là tên của biến số và `10` là giá trị của biến số đó.

### Toán tử số học (Arithmetic operators)

Trong lập trình, bạn có thể sử dụng các toán tử số học giữa các biến số hoặc một số giá trị cụ thể. Phép cộng, phép trừ, phép nhân giống như trong toán học và phép chia thì hơi khác một chút.

Ví dụ, bạn có thể viết như sau:

`sum = a + b` -> điều này sẽ lưu tổng của các giá trị `a` và `b` vào biến số `sum`.

`c = d - 7` -> điều này sẽ lưu kết quả của phép trừ vào biến số `c`.

`result = 15 * 3` -> điều này sẽ lưu 45 vào biến số `result`.

Có ba "kiểu" phép chia:

`x = a / b` -> đây là phép chia thực.

`y = 13 DIV 5` -> đây là phép chia số nguyên và nó sẽ lưu 2 vào biến số `y`.

`z = 13 MOD 5` -> đây là phép chia lấy số dư và nó sẽ lưu 3 vào biến số `z`.

### Toán tử quan hệ (Relational operators)

Trong khoa học máy tính, [toán tử quan hệ](https://en.wikipedia.org/wiki/Relational_operator) là một cấu trúc hoặc toán tử ngôn ngữ lập trình, dùng để kiểm tra hoặc định nghĩa một số loại quan hệ giữa hai thực thể. Bao gồm phép bằng nhau về số (ví dụ: 5 = 5) và phép bất đẳng thức (ví dụ: 4 ≥ 3).

Kết quả của phép đánh giá là đúng hoặc sai. Các toán tử quan hệ được sử dụng cho phân nhánh mà tôi đã giải thích ở trên.

Các toán tử là: bằng (==), không bằng (≠), lớn hơn (>), nhỏ hơn (<), lớn hơn hoặc bằng (≥), nhỏ hơn hoặc bằng (≤).

### Các phép toán Boolean

Các phép toán Boolean bắt nguồn từ [đại số Boolean](https://en.wikipedia.org/wiki/Boolean_algebra), trong đó các giá trị của các biến số là đúng hoặc sai (1 hoặc 0). Tôi không muốn làm phiền bạn nhiều với đại số Boolean, nhưng có ba phép toán chính mà bạn cần biết:

* AND (phép hội): Kết quả của phép toán này chỉ đúng khi cả hai điều kiện đều đúng, nếu không thì sai.
* OR (phép tuyển): Kết quả của phép toán này là đúng khi một trong hai điều kiện đúng.
* NOT (phép phủ định): Phép toán này đảo ngược giá trị của điều kiện. Nếu điều kiện đúng thì phép phủ định sẽ cho kết quả là sai và ngược lại.

Các phép toán Boolean cũng chủ yếu được sử dụng cho phân nhánh và có thể kết hợp với các toán tử quan hệ. Ví dụ, nếu bạn có một nhiệm vụ cần kiểm tra xem số đó có nhỏ hơn 50 hay không và không phải là 7, bạn sẽ thực hiện điều đó trong sơ đồ khối như thế này:

Vậy là xong. Nếu bạn đã hiểu mọi thứ đến giờ, bạn có thể nói rằng BÂY GIỜ BẠN có thể tư duy như một lập trình viên. Đây là kiến thức tối thiểu bạn cần biết để bắt đầu lập trình. Đây là nền tảng mà bạn xây dựng ngày càng nhiều kiến thức.

Bạn có thể nhận thấy rằng chúng ta không bắt đầu với bất kỳ ngôn ngữ lập trình nào. Đó là vì mọi thứ ở trên có thể áp dụng cho hầu hết các ngôn ngữ lập trình. Bây giờ, khi bạn hiểu được nền tảng, bạn có thể dễ dàng bắt đầu với bất kỳ ngôn ngữ lập trình nào.

### Các bước tiếp theo

Sau khi hoàn thành các bài tập thực hành ở trên, bạn có thể tự hỏi điều tiếp theo cần làm hoặc học là gì. Rõ ràng là bạn không thể làm được nhiều nếu chỉ biết vẽ sơ đồ khối.

Bây giờ bạn có thể chọn một ngôn ngữ lập trình và học cú pháp của nó. Tôi khuyên bạn nên học Python hoặc JavaScript. Cả hai ngôn ngữ đều dễ cài đặt trên máy tính của bạn và cú pháp thì đơn giản. Ở giai đoạn này của kinh nghiệm lập trình, tôi khuyên bạn nên chọn Python hoặc JavaScript chứ không phải C#, Java hoặc bất kỳ ngôn ngữ lập trình hướng đối tượng nào.
