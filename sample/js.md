# Hướng dẫn học JS cực nhanh
Chắc thế, cái này do Gemini viết dựa trên nội dung khóa học của F8 nha.

## Phần 1: Giới thiệu và Cài đặt

### Cài đặt môi trường, công cụ phù hợp để học JavaScript

Để học JavaScript, bạn cần:

* **Trình duyệt web:** Bất kỳ trình duyệt hiện đại nào (Chrome, Firefox, Edge...) đều có thể chạy JavaScript.
* **Trình soạn thảo code:** VS Code (Visual Studio Code) là lựa chọn tốt, miễn phí, nhiều extension hỗ trợ JavaScript.
* **Node.js (tùy chọn):**  Để chạy JavaScript ngoài trình duyệt (backend, công cụ...). Cài đặt từ [https://nodejs.org/](https://www.google.com/url?sa=E&source=gmail&q=https://nodejs.org/).

### Cách sử dụng JS trong file HTML

Có 2 cách chính để nhúng JavaScript vào file HTML:

* **Internal (nội tuyến):** Viết code JS trực tiếp trong thẻ `<script>` bên trong `<head>` hoặc `<body>` của file HTML.
* **External (ngoại tuyến):** Viết code JS trong file riêng (`.js`), sau đó liên kết đến file HTML bằng thẻ `<script src="path/to/script.js"></script>`. Cách này tốt hơn cho dự án lớn, dễ quản lý code.

* **Ví dụ (External JS - phổ biến nhất):**

* **`index.html`:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ví dụ External JS</title>
</head>
<body>
    <h1>Xin chào JavaScript!</h1>
    <script src="script.js"></script>
</body>
</html>
```

* **`script.js`:**

```javascript
    alert('Chào mừng đến với JavaScript!');
```

## Phần 2: Cú pháp và Cơ bản

### Khai báo biến

Biến dùng để lưu trữ dữ liệu trong chương trình. Trong JavaScript, có 3 từ khóa khai báo biến:

* `var` (ít dùng hiện nay, phạm vi function-scoped).
* `let` (phạm vi block-scoped, có thể gán lại giá trị).
* `const` (phạm vi block-scoped, không thể gán lại giá trị sau khi khởi tạo). Nên dùng `const` khi giá trị không đổi, `let` khi cần thay đổi.

* **Ví dụ:**

```javascript
let age = 30; // Khai báo biến age với let, giá trị 30
const name = "Gemini"; // Khai báo biến name với const, giá trị "Gemini"
age = 31; // Có thể gán lại giá trị cho age
// name = "Bard"; // Lỗi! Không thể gán lại giá trị cho const name
console.log(name + " is " + age + " years old.");
```

### Sử dụng Comments trong JavaScript

Comment (chú thích) trong JavaScript giúp ghi chú, giải thích code, hoặc tạm ẩn code mà không ảnh hưởng đến chương trình.

* **Single-line comment:** `// Đây là comment một dòng`

* **Multi-line comment:**

```javascript
/*
Đây là
comment
nhiều dòng
*/
```

* **Ví dụ:**

```javascript
// Đây là comment giải thích biến name
const name = "Gemini";
/*
Đoạn code này
sẽ in ra lời chào
*/
console.log("Xin chào, " + name + "!");
```

### Một số hàm built-in trong JavaScript

Built-in functions (hàm dựng sẵn) là các hàm có sẵn trong JavaScript để thực hiện các tác vụ phổ biến. Ví dụ:

* `alert()`: Hiển thị hộp thoại thông báo.
* `console.log()`: In thông tin ra console (DevTools).
* `prompt()`: Hiển thị hộp thoại nhập liệu.
* `parseInt()`, `parseFloat()`: Chuyển đổi chuỗi sang số nguyên, số thực.
* `typeof()`: Kiểm tra kiểu dữ liệu của biến.

* **Ví dụ:**

```javascript
alert("Đây là thông báo!"); // Hiển thị thông báo
console.log("Thông tin này in ra console"); // In ra console
let input = prompt("Nhập tên của bạn:"); // Hiển thị hộp thoại nhập liệu
console.log("Bạn đã nhập: " + input);
let numberString = "123";
let number = parseInt(numberString); // Chuyển chuỗi "123" sang số 123
console.log(typeof(number)); // In ra "number"
```

### Làm quen với toán tử trong JavaScript

Toán tử (operator) là ký hiệu thực hiện phép toán trên các giá trị (toán hạng). JavaScript có nhiều loại toán tử:
* Toán tử số học (+, -, \*, /, %, \*\*, ++, --).
* Toán tử gán (=, +=, -=, \*=, /=, %=).
* Toán tử so sánh (==, ===, \!=, \!==, \>, \<, \>=, \<=).
* Toán tử logic (&& - AND, || - OR, \! - NOT).
* Toán tử chuỗi (+ - cộng chuỗi).

### Toán tử số học trong JavaScript

Toán tử số học thực hiện các phép toán cơ bản:

* `+` (cộng), `-` (trừ), `*` (nhân), `/` (chia).
* `%` (chia lấy dư - modulo).
* `**` (lũy thừa - exponentiation).

* **Ví dụ:**

```javascript
let x = 10;
let y = 5;
console.log(x + y); // 15 (cộng)
console.log(x - y); // 5 (trừ)
console.log(x * y); // 50 (nhân)
console.log(x / y); // 2 (chia)
console.log(x % y); // 0 (chia lấy dư)
console.log(x ** y); // 100000 (10 mũ 5)
```

### Toán tử ++  -- với tiền tố & hậu tố (Prefix & Postfix) trong JavaScript

Toán tử tăng/giảm (`++`, `--`) tăng hoặc giảm giá trị biến đi 1.

* **Prefix (++x, --x):** Tăng/giảm giá trị **trước** khi sử dụng giá trị đó trong biểu thức.
* **Postfix (x++, x--):** Tăng/giảm giá trị **sau** khi sử dụng giá trị đó trong biểu thức.

* **Ví dụ:**

```javascript
let a = 5;
let b = ++a; // Prefix: a tăng lên 6 trước, sau đó b = 6
console.log("a:", a, "b:", b); // a: 6 b: 6

let c = 5;
let d = c++; // Postfix: d = 5 trước, sau đó c tăng lên 6
console.log("c:", c, "d:", d); // c: 6 d: 5
```

### Toán tử gán trong JavaScript

Toán tử gán gán giá trị cho biến.

* `=` (gán trực tiếp).
* `+=`, `-=`, `*=`, `/=`, `%=` (gán kết hợp phép toán).

* **Ví dụ:**

```javascript
let num = 10;
num = 20; // Gán trực tiếp num = 20
num += 5; // num = num + 5 (num = 25)
num -= 3; // num = num - 3 (num = 22)
num *= 2; // num = num * 2 (num = 44)
num /= 4; // num = num / 4 (num = 11)
num %= 3; // num = num % 3 (num = 2 - dư của 11 chia 3)
console.log(num); // 2
```

### Toán tử chuỗi (String Operator) trong JavaScript

Toán tử chuỗi chính là toán tử `+` (cộng) dùng để **nối chuỗi** (concatenation).

* **Ví dụ:**

```javascript
let firstName = "Gemini";
let lastName = "AI";
let fullName = firstName + " " + lastName; // Nối chuỗi
console.log(fullName); // Gemini AI
```

### Toán tử so sánh trong Javascript (phần 1)

Toán tử so sánh so sánh hai giá trị và trả về giá trị boolean (`true` hoặc `false`).
* `==` (bằng giá trị - loose equality): So sánh giá trị, có thể ép kiểu dữ liệu.
* `===` (bằng giá trị và kiểu dữ liệu - strict equality): So sánh cả giá trị và kiểu dữ liệu, không ép kiểu. Nên dùng `===` để so sánh chính xác.
* `!=` (không bằng giá trị - loose inequality).
* `!==` (không bằng giá trị hoặc kiểu dữ liệu - strict inequality).
* `>` (lớn hơn), `<` (nhỏ hơn), `>=` (lớn hơn hoặc bằng), `<=` (nhỏ hơn hoặc bằng).

### Kiểu dữ liệu Boolean (Boolean data type) trong JavaScript

Boolean là kiểu dữ liệu logic chỉ có 2 giá trị: `true` (đúng) và `false` (sai). Thường dùng trong câu lệnh điều kiện và toán tử logic.

* **Ví dụ:**

```javascript
let isAdult = true;
let isRaining = false;
console.log(typeof(isAdult)); // "boolean"
console.log(isRaining); // false
```

### Câu lệnh điều kiện If - Else trong JavaScript

Câu lệnh `if...else` thực hiện code khác nhau dựa trên điều kiện đúng hay sai.

* `if (condition) { ... }`: Nếu `condition` đúng (`true`), code trong block `if` được thực hiện.
* `else { ... }`: Nếu `condition` sai (`false`), code trong block `else` được thực hiện (tùy chọn).
* `else if (condition2) { ... }`: Kiểm tra thêm điều kiện nếu điều kiện `if` sai (có thể có nhiều `else if`).

* **Ví dụ:**

```javascript
let age = 18;
if (age >= 18) {
    console.log("Bạn đã đủ tuổi trưởng thành.");
} else {
    console.log("Bạn chưa đủ tuổi trưởng thành.");
}
```

### Toán tử logical trong JavaScript

Toán tử logic kết hợp các biểu thức boolean.

* `&&` (AND - và): `true` nếu **cả hai** toán hạng đều `true`.
* `||` (OR - hoặc): `true` nếu **ít nhất một** toán hạng là `true`.
* `!` (NOT - phủ định): Đảo ngược giá trị boolean (`!true` là `false`, `!false` là `true`).

* **Ví dụ:**

```javascript
let hasLicense = true;
let hasCar = false;
if (hasLicense && hasCar) { // Cả hai phải true
    console.log("Đủ điều kiện lái xe.");
} else if (hasLicense || hasCar) { // Ít nhất một true
    console.log("Có một trong hai điều kiện.");
} else {
    console.log("Không đủ điều kiện.");
}
console.log(!hasLicense); // false (phủ định true)
```

### Kiểu dữ liệu trong JavaScript

JavaScript là ngôn ngữ kiểu dữ liệu động (dynamic typing), kiểu dữ liệu của biến được xác định khi chạy chương trình, không cần khai báo rõ ràng. Các kiểu dữ liệu cơ bản:
* `Number` (số): Số nguyên, số thực.
* `String` (chuỗi): Văn bản.
* `Boolean` (boolean): `true` hoặc `false`.
* `Null`: Giá trị rỗng có chủ ý.
* `Undefined`: Biến đã khai báo nhưng chưa gán giá trị.
* `Symbol` (ES6): Giá trị duy nhất, thường dùng làm key object.
* `Object` (đối tượng): Tập hợp các cặp key-value.

### Toán tử so sánh trong JavaScript (phần 2)

Tiếp tục về toán tử so sánh, tập trung vào sự khác biệt giữa `==` và `===`. Nên dùng `===` và `!==` để so sánh chính xác, tránh các hành vi ép kiểu không mong muốn của `==` và `!=`.

### Toán tử logical và câu lệnh điều kiện If trong JavaScript

Kết hợp toán tử logic và câu lệnh `if` để tạo điều kiện phức tạp hơn.

* **Ví dụ:**

```javascript
let age = 20;
let hasTicket = true;
if (age >= 18 && hasTicket) { // Vừa đủ tuổi, vừa có vé
    console.log("Được vào xem phim.");
} else {
    console.log("Không được vào xem phim.");
}
```

### Chuỗi trong JavaScript

Chuỗi (string) là kiểu dữ liệu văn bản trong JavaScript, được bao quanh bởi dấu nháy đơn (`'...'`), nháy kép (`"..."`) hoặc backtick (\`...\`). Backtick dùng cho template literals (chuỗi template).

* **Ví dụ:**

```javascript
let singleQuoteString = 'Chuỗi nháy đơn';
let doubleQuoteString = "Chuỗi nháy kép";
let templateString = `Chuỗi template literals`; // Backtick
console.log(singleQuoteString);
console.log(doubleQuoteString);
console.log(templateString);
```

### Làm việc với chuỗi trong JavaScript

String methods (phương thức chuỗi) là các hàm có sẵn để thao tác với chuỗi. Ví dụ:

* `length`: Thuộc tính lấy độ dài chuỗi.
* `charAt(index)`: Lấy ký tự tại vị trí index.
* `indexOf(substring)`: Tìm vị trí đầu tiên của substring.
* `lastIndexOf(substring)`: Tìm vị trí cuối cùng của substring.
* `slice(start, end)`: Cắt chuỗi từ vị trí start đến end (không bao gồm end).
* `substring(start, end)`: Tương tự `slice`.
* `toUpperCase()`, `toLowerCase()`: Chuyển chuỗi thành chữ hoa, chữ thường.
* `trim()`: Xóa khoảng trắng đầu và cuối chuỗi.
* `split(delimiter)`: Chia chuỗi thành mảng các chuỗi con dựa trên delimiter.
* `replace(oldValue, newValue)`: Thay thế chuỗi con oldValue bằng newValue.

* **Ví dụ:**

```javascript
let message = "  Hello World!  ";
console.log(message.length); // 15 (độ dài chuỗi)
console.log(message.charAt(0)); // " " (ký tự đầu tiên)
console.log(message.indexOf("World")); // 7 (vị trí của "World")
console.log(message.slice(2, 7)); // "Hello" (cắt từ vị trí 2 đến 6)
console.log(message.toUpperCase()); // "  HELLO WORLD!  "
console.log(message.trim()); // "Hello World!" (xóa khoảng trắng)
console.log(message.split(" ")); // ["", "", "Hello", "World!", "", ""] (chia thành mảng)
console.log(message.replace("World", "JavaScript")); // "  Hello JavaScript!  "
```

### Số và làm việc với kiểu số trong JavaScript

Number methods (phương thức số) là các hàm có sẵn để thao tác với số. Ví dụ:

* `toFixed(digits)`: Định dạng số thập phân với `digits` chữ số sau dấu phẩy.
* `parseInt()`, `parseFloat()`: Chuyển đổi chuỗi sang số nguyên, số thực.
* `isNaN()`: Kiểm tra xem có phải NaN (Not-a-Number) không.
* `Number.isInteger()`: Kiểm tra xem có phải số nguyên không.
* `Math.random()`: Sinh số ngẫu nhiên từ 0 đến \< 1.
* `Math.floor()`, `Math.ceil()`, `Math.round()`: Làm tròn số xuống, lên, gần nhất.
* `Math.max()`, `Math.min()`: Tìm số lớn nhất, nhỏ nhất.

* **Ví dụ:**

```javascript
let pi = 3.14159;
console.log(pi.toFixed(2)); // "3.14" (làm tròn đến 2 chữ số thập phân)
let numString = "42";
let numInt = parseInt(numString); // 42 (chuyển sang số nguyên)
console.log(isNaN("hello")); // true (không phải số)
console.log(Number.isInteger(10)); // true (số nguyên)
console.log(Math.random()); // Số ngẫu nhiên (ví dụ: 0.567...)
console.log(Math.floor(3.9)); // 3 (làm tròn xuống)
console.log(Math.max(1, 5, 2)); // 5 (số lớn nhất)
```

### Mảng trong JavaScript

Mảng (array) là kiểu dữ liệu danh sách, chứa nhiều giá trị theo thứ tự. Các phần tử mảng có thể có kiểu dữ liệu khác nhau. Mảng được khai báo bằng dấu ngoặc vuông `[...]`.

* **Ví dụ:**

```javascript
let colors = ["red", "green", "blue"]; // Mảng chuỗi
let numbers = [1, 2, 3, 4, 5]; // Mảng số
let mixedArray = [1, "hello", true, null]; // Mảng hỗn hợp
console.log(colors[0]); // "red" (phần tử đầu tiên, index 0)
console.log(numbers.length); // 5 (độ dài mảng)
```

### Làm việc với mảng trong JavaScript

Các thao tác cơ bản với mảng:

* Truy cập phần tử: `array[index]`.
* Sửa đổi phần tử: `array[index] = newValue;`.
* Thêm phần tử:
    * `push(element)`: Thêm vào cuối mảng.
    * `unshift(element)`: Thêm vào đầu mảng.
* Xóa phần tử:
    * `pop()`: Xóa phần tử cuối mảng và trả về phần tử đó.
    * `shift()`: Xóa phần tử đầu mảng và trả về phần tử đó.
    * `splice(startIndex, deleteCount, item1, item2, ...)`: Xóa và/hoặc thêm phần tử tại vị trí bất kỳ.

* **Ví dụ:**

```javascript
let fruits = ["apple", "banana", "orange"];
console.log(fruits[1]); // "banana"
fruits[1] = "grape"; // Sửa đổi phần tử
console.log(fruits); // ["apple", "grape", "orange"]
fruits.push("mango"); // Thêm vào cuối
console.log(fruits); // ["apple", "grape", "orange", "mango"]
fruits.unshift("kiwi"); // Thêm vào đầu
console.log(fruits); // ["kiwi", "apple", "grape", "orange", "mango"]
let lastFruit = fruits.pop(); // Xóa cuối
console.log(lastFruit); // "mango"
console.log(fruits); // ["kiwi", "apple", "grape", "orange"]
fruits.splice(1, 2, "pear", "melon"); // Xóa 2 phần tử từ index 1, thêm "pear", "melon"
console.log(fruits); // ["kiwi", "pear", "melon", "orange"]
```

### Hàm trong JavaScript

Hàm (function) là khối code thực hiện một tác vụ cụ thể, có thể tái sử dụng nhiều lần. Giúp code có cấu trúc, dễ đọc, dễ bảo trì.

* **Khai báo hàm:**

```javascript
function functionName(parameter1, parameter2, ...) {
    // Code thực hiện trong hàm
    // ...
    return value; // (tùy chọn, trả về giá trị)
}
```

* **Gọi hàm:** `functionName(argument1, argument2, ...);`

* **Ví dụ:**

```javascript
function add(a, b) { // Hàm cộng hai số
    return a + b;
}

let sum = add(5, 3); // Gọi hàm add với đối số 5 và 3
console.log(sum); // 8
```

### Tham số trong hàm

Tham số (parameter) là biến được khai báo trong định nghĩa hàm, dùng để nhận giá trị đầu vào khi gọi hàm. Đối số (argument) là giá trị thực tế được truyền vào khi gọi hàm.

* **Ví dụ:** (ví dụ trên đã có tham số)

```javascript
function greet(name) { // 'name' là tham số
    console.log("Xin chào, " + name + "!");
}

greet("Gemini"); // "Gemini" là đối số
greet("User"); // "User" là đối số
```

### Return trong hàm JS

Câu lệnh `return` trong hàm dùng để trả về một giá trị từ hàm. Hàm có thể trả về bất kỳ kiểu dữ liệu nào (số, chuỗi, mảng, object...). Nếu không có `return`, hàm trả về `undefined`.

* **Ví dụ:** (ví dụ hàm `add` và `greet` trên đã có return và không return)

```javascript
function square(number) {
    return number * number; // Trả về bình phương của số
}

let result = square(4);
console.log(result); // 16

function sayHello() { // Không có return
    console.log("Hello!");
}

let greeting = sayHello();
console.log(greeting); // undefined (hàm không trả về gì)
```

### Hiểu hơn về function trong JavaScript

Hàm là first-class citizens trong JavaScript: có thể gán cho biến, truyền như đối số cho hàm khác, trả về từ hàm khác. Hàm có thể có tên (named function) hoặc không tên (anonymous function).

### Các loại function trong JavaScript

Các loại function trong JavaScript:

* **Named function:** Hàm có tên, khai báo bằng từ khóa `function`. (ví dụ trên)
* **Anonymous function:** Hàm không tên, thường dùng gán cho biến hoặc làm callback.
* **Arrow function (ES6):** Cú pháp ngắn gọn hơn cho anonymous function.

* **Ví dụ (Anonymous function và Arrow function):**

```javascript
// Anonymous function gán cho biến
let multiply = function(a, b) {
    return a * b;
};
console.log(multiply(3, 7)); // 21

// Arrow function (tương đương hàm multiply ở trên)
let multiplyArrow = (a, b) => a * b;
console.log(multiplyArrow(4, 6)); // 24

// Callback function (anonymous function truyền vào hàm khác)
setTimeout(function() {
    console.log("Hello after 1 second");
}, 1000);

// Callback function (arrow function)
setTimeout(() => {
    console.log("Hello again after 2 seconds");
}, 2000);
```

### Object trong JavaScript

Object (đối tượng) là kiểu dữ liệu phức tạp trong JavaScript, biểu diễn một thực thể có thuộc tính (properties) và phương thức (methods). Object là tập hợp các cặp key-value, key là chuỗi (hoặc Symbol), value có thể là bất kỳ kiểu dữ liệu nào. Object được khai báo bằng dấu ngoặc nhọn `{...}`.

* **Ví dụ:**

```javascript
let person = {
    name: "Gemini", // Thuộc tính name
    age: 2,        // Thuộc tính age
    isRobot: true,  // Thuộc tính isRobot
    greet: function() { // Phương thức greet
        console.log("Xin chào, tôi là " + this.name);
    }
};

console.log(person.name); // "Gemini" (truy cập thuộc tính bằng dấu chấm)
console.log(person["age"]); // 2 (truy cập thuộc tính bằng dấu ngoặc vuông)
person.greet(); // Gọi phương thức greet
```

### Object constructor trong JavaScript

Object constructor (hàm tạo đối tượng) là hàm đặc biệt dùng để tạo ra các object cùng loại (cùng cấu trúc thuộc tính và phương thức). Dùng từ khóa `new` để gọi constructor.

* **Ví dụ:**

```javascript
function Dog(name, breed) { // Constructor Dog
    this.name = name;
    this.breed = breed;
    this.bark = function() {
        console.log("Woof!");
    };
}

let myDog = new Dog("Lucky", "Golden Retriever"); // Tạo object Dog bằng constructor
console.log(myDog.name); // "Lucky"
myDog.bark(); // Gọi phương thức bark
```

### Object prototype(cơ bản) trong JavaScript

Prototype là cơ chế kế thừa trong JavaScript. Mỗi object được tạo ra từ constructor có một prototype. Prototype là một object khác, chứa các thuộc tính và phương thức mà các object con kế thừa. Giúp tái sử dụng code, tiết kiệm bộ nhớ.

### Date object trong JavaScript

Date object (đối tượng Date) dùng để làm việc với ngày và giờ trong JavaScript. Tạo Date object bằng `new Date()`.

* **Ví dụ:**

```javascript
let now = new Date(); // Date object hiện tại
console.log(now); // In ra ngày giờ hiện tại

let specificDate = new Date(2025, 2, 26); // Date object cho ngày 26/03/2025 (tháng bắt đầu từ 0)
console.log(specificDate);

console.log(now.getFullYear()); // Lấy năm
console.log(now.getMonth()); // Lấy tháng (0-11)
console.log(now.getDate()); // Lấy ngày
console.log(now.getHours()); // Lấy giờ
console.log(now.getMinutes()); // Lấy phút
```

## Phần 3: Câu lệnh điều khiển và Vòng lặp

### Câu lệnh rẽ nhánh If, else

(Đã đề cập ở mục 15) Ôn lại và mở rộng về câu lệnh `if...else`, `else if`.

### Câu lệnh rẽ nhánh Switch trong JavaScript

Câu lệnh `switch...case` là một cách khác để rẽ nhánh chương trình dựa trên giá trị của một biểu thức. Thường dùng khi có nhiều trường hợp (case) có thể xảy ra.

* **Ví dụ:**

```javascript
let dayOfWeek = 3; // 1: Thứ Hai, 2: Thứ Ba, ..., 7: Chủ Nhật
let dayName;

switch (dayOfWeek) {
    case 1:
        dayName = "Thứ Hai";
        break;
    case 2:
        dayName = "Thứ Ba";
        break;
    case 3:
        dayName = "Thứ Tư";
        break;
    case 4:
        dayName = "Thứ Năm";
        break;
    case 5:
        dayName = "Thứ Sáu";
        break;
    case 6:
        dayName = "Thứ Bảy";
        break;
    case 7:
        dayName = "Chủ Nhật";
        break;
    default:
        dayName = "Không hợp lệ";
}

console.log("Hôm nay là " + dayName); // Hôm nay là Thứ Tư
```

### Toán tử 3 ngôi(ternary operator) trong JavaScript

Toán tử 3 ngôi (ternary operator) `condition ? valueIfTrue : valueIfFalse` là cú pháp rút gọn của câu lệnh `if...else` khi chỉ có một điều kiện và trả về một trong hai giá trị.

* **Ví dụ:**

```javascript
let age = 15;
let message = age >= 18 ? "Đủ tuổi" : "Chưa đủ tuổi"; // Toán tử 3 ngôi
console.log(message); // "Chưa đủ tuổi"

// Tương đương với if...else:
let message2;
if (age >= 18) {
    message2 = "Đủ tuổi";
} else {
    message2 = "Chưa đủ tuổi";
}
console.log(message2); // "Chưa đủ tuổi"
```

### Vòng lặp trong JavaScript

Vòng lặp (loop) dùng để lặp đi lặp lại một khối code nhiều lần. Các loại vòng lặp trong JavaScript:
* `for` loop.
* `for...in` loop (lặp qua thuộc tính của object).
* `for...of` loop (lặp qua giá trị của iterable object - mảng, chuỗi...).
* `while` loop.
* `do...while` loop.

### Vòng lặp For trong JavaScript

`for` loop có cú pháp: `for (initialization; condition; increment/decrement) { ... }`

* `initialization`: Khởi tạo biến đếm (chạy một lần đầu tiên).
* `condition`: Điều kiện lặp (kiểm tra trước mỗi lần lặp, nếu `true` thì lặp tiếp, `false` thì dừng).
* `increment/decrement`: Tăng/giảm biến đếm sau mỗi lần lặp.

* **Ví dụ:**

```javascript
for (let i = 1; i <= 5; i++) { // Lặp 5 lần, i từ 1 đến 5
    console.log("Lần lặp thứ " + i);
}
```

`for...in` loop lặp qua **thuộc tính (key)** của một object.

* **Ví dụ:**

```javascript
let person = {
    name: "Gemini",
    age: 2,
    city: "Internet"
};

for (let key in person) { // Lặp qua key của object person
    console.log(key + ": " + person[key]);
}
// In ra:
// name: Gemini
// age: 2
// city: Internet
```

### Vòng lặp For/of trong JavaScript

`for...of` loop lặp qua **giá trị** của một **iterable object** (mảng, chuỗi, Map, Set...).

* **Ví dụ:**

```javascript
let colors = ["red", "green", "blue"];

for (let color of colors) { // Lặp qua giá trị của mảng colors
    console.log(color);
}
// In ra:
// red
// green
// blue

let message = "Hello";
for (let char of message) { // Lặp qua ký tự của chuỗi message
    console.log(char);
}
// In ra:
// H
// e
// l
// l
// o
```

### Vòng lặp While trong JavaScript

`while` loop lặp khi điều kiện còn đúng (`true`). Cú pháp: `while (condition) { ... }`

* **Ví dụ:**

```javascript
let count = 1;
while (count <= 5) { // Lặp khi count <= 5
    console.log("Count: " + count);
    count++; // Tăng count sau mỗi lần lặp
}
```

### Vòng lặp Do/while trong JavaScript

`do...while` loop tương tự `while` loop, nhưng code trong block `do` được thực hiện **ít nhất một lần** trước khi kiểm tra điều kiện. Cú pháp: `do { ... } while (condition);`

* **Ví dụ:**

```javascript
let num = 0;
do {
    console.log("Num: " + num);
    num++;
} while (num < 3); // Lặp khi num < 3
// In ra:
// Num: 0
// Num: 1
// Num: 2
```

### Break và Continue trong vòng lặp

* **Tóm tắt:**

* `break`: Thoát khỏi vòng lặp ngay lập tức.
* `continue`: Bỏ qua lần lặp hiện tại và chuyển sang lần lặp tiếp theo.

* **Ví dụ:**

```javascript
for (let i = 1; i <= 10; i++) {
    if (i === 5) {
        break; // Thoát khỏi vòng lặp khi i = 5
    }
    console.log("i (break): " + i); // In ra 1, 2, 3, 4
}

for (let j = 1; j <= 5; j++) {
    if (j === 3) {
        continue; // Bỏ qua lần lặp khi j = 3
    }
    console.log("j (continue): " + j); // In ra 1, 2, 4, 5 (bỏ qua 3)
}
```

### Vòng lặp lồng nhau (Nested loop)

Nested loop (vòng lặp lồng nhau) là vòng lặp bên trong vòng lặp khác. Thường dùng để xử lý dữ liệu đa chiều (ví dụ: ma trận, bảng).

* **Ví dụ:**

```javascript
for (let i = 1; i <= 3; i++) { // Vòng lặp ngoài
    console.log("Vòng lặp ngoài lần " + i);
    for (let j = 1; j <= 2; j++) { // Vòng lặp trong (lặp 2 lần cho mỗi lần lặp ngoài)
        console.log("  Vòng lặp trong lần " + j);
    }
}
// In ra:
// Vòng lặp ngoài lần 1
//   Vòng lặp trong lần 1
//   Vòng lặp trong lần 2
// Vòng lặp ngoài lần 2
//   Vòng lặp trong lần 1
//   Vòng lặp trong lần 2
// Vòng lặp ngoài lần 3
//   Vòng lặp trong lần 1
//   Vòng lặp trong lần 2
```

### Ví dụ mở rộng về vòng lặp

Tổng hợp các ví dụ phức tạp hơn về vòng lặp, có thể kết hợp với điều kiện, mảng, object... để giải quyết các bài toán thực tế.

## Phần 4: Làm việc với Mảng nâng cao

### Làm việc với mảng trong JavaScript

Tiếp tục về Array methods, giới thiệu các phương thức quan trọng để thao tác và xử lý mảng:

* `concat(array2, array3, ...)`: Nối mảng với các mảng khác.
* `join(separator)`: Nối các phần tử mảng thành chuỗi, phân tách bằng separator.
* `slice(startIndex, endIndex)`: Trả về mảng con từ startIndex đến endIndex (không bao gồm endIndex).
* `splice(startIndex, deleteCount, item1, item2, ...)`: (Đã đề cập ở mục 24) Xóa và/hoặc thêm phần tử tại vị trí bất kỳ.
* `sort()`: Sắp xếp mảng (mặc định theo thứ tự bảng chữ cái hoặc số tăng dần). Cần custom function để sắp xếp số đúng cách.
* `reverse()`: Đảo ngược mảng.

* **Ví dụ:**

```javascript
let arr1 = [1, 2, 3];
let arr2 = [4, 5, 6];
let combinedArray = arr1.concat(arr2); // Nối mảng
console.log(combinedArray); // [1, 2, 3, 4, 5, 6]

let fruits = ["apple", "banana", "orange"];
let fruitString = fruits.join(", "); // Nối thành chuỗi
console.log(fruitString); // "apple, banana, orange"

let numbers = [1, 5, 2, 8, 3];
numbers.sort(); // Sắp xếp (mặc định theo chuỗi) -> [1, 2, 3, 5, 8]
numbers.sort((a, b) => a - b); // Sắp xếp số tăng dần
console.log(numbers); // [1, 2, 3, 5, 8]
numbers.reverse(); // Đảo ngược mảng
console.log(numbers); // [8, 5, 3, 2, 1]
```

### Array map method trong JavaScript

`map()` method tạo ra một **mảng mới** bằng cách gọi một function (callback) cho **mỗi phần tử** của mảng ban đầu. Callback function nhận vào phần tử hiện tại và trả về giá trị mới cho phần tử tương ứng trong mảng mới.

* **Ví dụ:**

```javascript
let numbers = [1, 2, 3, 4, 5];
let squaredNumbers = numbers.map(function(number) { // map() với anonymous function
    return number * number; // Bình phương mỗi số
});
console.log(squaredNumbers); // [1, 4, 9, 16, 25]

// Sử dụng arrow function cho ngắn gọn hơn:
let doubledNumbers = numbers.map(number => number * 2); // Nhân đôi mỗi số
console.log(doubledNumbers); // [2, 4, 6, 8, 10]
```

### Phương thức reduce khi làm việc với array

`reduce()` method thực hiện một callback function "reducer" trên mỗi phần tử của mảng, và trả về một **giá trị duy nhất** (không phải mảng mới như `map()`). Thường dùng để tính tổng, tích, hoặc gom nhóm dữ liệu trong mảng.

* **Callback function của `reduce()` nhận 2 tham số chính:**

* `accumulator` (giá trị tích lũy): Giá trị được trả về từ lần gọi callback trước đó (hoặc `initialValue` nếu được cung cấp).
* `currentValue` (giá trị hiện tại): Phần tử mảng đang được xử lý.

* **Cú pháp:** `array.reduce(reducerFunction, initialValue);` (`initialValue` là giá trị khởi tạo cho `accumulator`, tùy chọn).

* **Ví dụ (tính tổng mảng):**

```javascript
let numbers = [1, 2, 3, 4, 5];
let sum = numbers.reduce(function(accumulator, currentValue) { // reduce() với anonymous function
    return accumulator + currentValue; // Cộng dồn vào accumulator
}, 0); // initialValue = 0 (tổng ban đầu = 0)
console.log(sum); // 15 (tổng các số trong mảng)

// Sử dụng arrow function:
let product = numbers.reduce((accumulator, currentValue) => accumulator * currentValue, 1); // Tính tích
console.log(product); // 120 (tích các số trong mảng)
```

### Phương thức reduce khi làm việc với array - phần 2

Tiếp tục về `reduce()`, có thể đi sâu vào các ứng dụng phức tạp hơn như gom nhóm đối tượng trong mảng, flatten mảng đa chiều...

### Phương thức includes

`includes()` method kiểm tra xem một chuỗi có chứa một substring (với chuỗi) hoặc một mảng có chứa một phần tử (với mảng) hay không. Trả về `true` nếu có, `false` nếu không.

* **Ví dụ:**

```javascript
let message = "Hello World";
console.log(message.includes("World")); // true (chuỗi message chứa "World")
console.log(message.includes("JavaScript")); // false

let fruits = ["apple", "banana", "orange"];
console.log(fruits.includes("banana")); // true (mảng fruits chứa "banana")
console.log(fruits.includes("grape")); // false
```

### Đối tượng math

Math object là built-in object cung cấp các hằng số toán học và hàm toán học. Không cần tạo instance (không dùng `new Math()`). Truy cập trực tiếp qua `Math.property` hoặc `Math.method()`.

* **Hằng số:** `Math.PI` (số Pi), `Math.E` (số e), ...
* **Hàm:** `Math.random()`, `Math.floor()`, `Math.ceil()`, `Math.round()`, `Math.max()`, `Math.min()`, `Math.pow()`, `Math.sqrt()`, ... (đã đề cập một số ở mục 22).

* **Ví dụ:**

```javascript
console.log(Math.PI); // 3.141592653589793 (số Pi)
console.log(Math.sqrt(25)); // 5 (căn bậc hai)
console.log(Math.pow(2, 3)); // 8 (2 mũ 3)
console.log(Math.round(4.6)); // 5 (làm tròn gần nhất)
```

### Hiểu về Javascript Callback Functions

Callback function (hàm callback) là hàm được truyền vào làm đối số của một hàm khác, và sẽ được gọi lại (callback) sau khi hàm cha thực hiện xong một tác vụ nào đó (thường là tác vụ bất đồng bộ - asynchronous). Dùng nhiều trong xử lý sự kiện, AJAX, Promises...

* **Ví dụ (setTimeout với callback):**

```javascript
function doSomething(callback) { // Hàm doSomething nhận callback làm đối số
    console.log("Bắt đầu tác vụ...");
    setTimeout(function() { // Giả lập tác vụ bất đồng bộ (ví dụ: gọi API)
        console.log("Tác vụ hoàn thành!");
        callback(); // Gọi callback function sau khi tác vụ xong
    }, 2000);
}

doSomething(function() { // Truyền anonymous function làm callback
    console.log("Callback được gọi!");
});
```

### Callback trong JavaScript

Tiếp tục về callback, có thể đi sâu vào callback hell (callback lồng nhau quá sâu, code khó đọc, khó bảo trì) và cách khắc phục (Promises, async/await).

### Xây dựng phương thức làm việc với array

Có thể nói về việc tạo custom array methods (phương thức mảng tự định nghĩa) bằng cách thêm phương thức vào `Array.prototype`. Tuy nhiên, cách này ít dùng hiện nay vì có thể xung đột với các phương thức chuẩn hoặc thư viện khác. Nên ưu tiên dùng các phương thức mảng có sẵn.

### Xây dựng phương thức forEach

`forEach()` method lặp qua từng phần tử của mảng và thực hiện callback function cho mỗi phần tử. Tương tự `for...of` loop, nhưng ngắn gọn hơn. Không tạo mảng mới, không trả về giá trị, chỉ thực hiện side effects (ví dụ: in ra console, sửa đổi mảng gốc...).

* **Ví dụ:**

```javascript
let colors = ["red", "green", "blue"];
colors.forEach(function(color) { // forEach() với anonymous function
    console.log("Màu: " + color);
});

// Sử dụng arrow function:
colors.forEach(color => console.log("Màu (arrow): " + color));
```

### Xây dựng phương thức filter

`filter()` method tạo ra một **mảng mới** chứa các phần tử thỏa mãn một điều kiện nào đó (được kiểm tra bởi callback function). Callback function trả về `true` nếu phần tử thỏa mãn điều kiện, `false` nếu không.

* **Ví dụ:**

```javascript
let numbers = [1, 2, 3, 4, 5, 6];
let evenNumbers = numbers.filter(function(number) { // filter() với anonymous function
    return number % 2 === 0; // Điều kiện: số chẵn
});
console.log(evenNumbers); // [2, 4, 6] (mảng mới chỉ chứa số chẵn)

// Sử dụng arrow function:
let oddNumbers = numbers.filter(number => number % 2 !== 0); // Lọc số lẻ
console.log(oddNumbers); // [1, 3, 5]
```

### Xây dựng phương thức some

`some()` method kiểm tra xem **ít nhất một** phần tử trong mảng có thỏa mãn điều kiện (callback function) hay không. Trả về `true` nếu có ít nhất một phần tử thỏa mãn, `false` nếu không có phần tử nào thỏa mãn.

* **Ví dụ:**

```javascript
let numbers = [1, 2, 3, 4, 5];
let hasEvenNumber = numbers.some(function(number) { // some() với anonymous function
    return number % 2 === 0; // Điều kiện: số chẵn
});
console.log(hasEvenNumber); // true (mảng numbers có số chẵn)

let allOddNumbers = numbers.some(number => number % 2 !== 0); // Kiểm tra có số lẻ không
console.log(allOddNumbers); // true
```

### Xây dựng phương thức every

`every()` method kiểm tra xem **tất cả** phần tử trong mảng có thỏa mãn điều kiện (callback function) hay không. Trả về `true` nếu **tất cả** phần tử thỏa mãn, `false` nếu có ít nhất một phần tử không thỏa mãn.

* **Ví dụ:**

```javascript
let numbers = [2, 4, 6, 8];
let allEvenNumbers = numbers.every(function(number) { // every() với anonymous function
    return number % 2 === 0; // Điều kiện: số chẵn
});
console.log(allEvenNumbers); // true (tất cả số trong mảng đều chẵn)

let allPositiveNumbers = numbers.every(number => number > 0); // Kiểm tra tất cả số dương
console.log(allPositiveNumbers); // true
```

### Đệ quy là gì? Học về đệ quy trong JavaScript

Đệ quy (recursion) là kỹ thuật lập trình mà một hàm tự gọi lại chính nó. Dùng để giải quyết các bài toán có cấu trúc lặp lại, hoặc bài toán có thể chia nhỏ thành các bài toán con tương tự. Cần có điều kiện dừng (base case) để tránh lặp vô hạn.

* **Ví dụ (tính giai thừa):**

```javascript
function factorial(n) {
    if (n === 0) { // Base case: giai thừa của 0 là 1
        return 1;
    } else {
        return n * factorial(n - 1); // Gọi lại hàm factorial với n-1 (đệ quy)
    }
}

console.log(factorial(5)); // 120 (5! = 5 * 4 * 3 * 2 * 1)
```

## Phần 5: DOM và Events

### HTML DOM là gì?

HTML DOM (Document Object Model) là mô hình biểu diễn cấu trúc HTML dưới dạng cây các đối tượng (nodes). JavaScript có thể truy cập và thao tác với DOM để thay đổi nội dung, cấu trúc, style của trang web.

### HTML DOM và DOM API là gì?

DOM API (Application Programming Interface) là tập hợp các đối tượng, thuộc tính, phương thức do trình duyệt cung cấp để JavaScript tương tác với DOM. Ví dụ: `document.getElementById()`, `element.innerHTML`, `element.style.color`, `element.addEventListener()`.

### DOM Document Object trong JavaScript

`document` object là entry point (điểm bắt đầu) để truy cập DOM từ JavaScript. Đại diện cho toàn bộ trang HTML. Các phương thức và thuộc tính của `document` cho phép truy cập và thao tác với các phần tử HTML trên trang.

### Lấy element trong DOM

Các phương thức chính để lấy element (phần tử HTML) từ DOM:

* `document.getElementById(id)`: Lấy element có `id` attribute tương ứng (trả về 1 element hoặc `null`).
* `document.getElementsByClassName(className)`: Lấy danh sách (HTMLCollection) các element có `class` attribute tương ứng (trả về HTMLCollection rỗng nếu không tìm thấy).
* `document.getElementsByTagName(tagName)`: Lấy danh sách (HTMLCollection) các element có tag name tương ứng (ví dụ: "p", "div", "a"...) (trả về HTMLCollection rỗng nếu không tìm thấy).
* `document.querySelector(selector)`: Lấy **element đầu tiên** phù hợp với CSS selector (trả về 1 element hoặc `null`).
* `document.querySelectorAll(selector)`: Lấy danh sách (NodeList) **tất cả** element phù hợp với CSS selector (trả về NodeList rỗng nếu không tìm thấy). Nên dùng `querySelector` và `querySelectorAll` vì linh hoạt hơn (dùng CSS selector).

* **Ví dụ:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ví dụ DOM Get Element</title>
</head>
<body>
    <h1 id="title">Tiêu đề chính</h1>
    <p class="paragraph">Đoạn văn 1.</p>
    <p class="paragraph">Đoạn văn 2.</p>
    <ul>
        <li>Item 1</li>
        <li>Item 2</li>
    </ul>
    <div id="container">
        <button>Click me</button>
    </div>

    <script>
        let titleElement = document.getElementById("title"); // Lấy theo ID
        console.log(titleElement); // <h1 id="title">...</h1>

        let paragraphElements = document.getElementsByClassName("paragraph"); // Lấy theo class
        console.log(paragraphElements); // HTMLCollection [p.paragraph, p.paragraph]

        let liElements = document.getElementsByTagName("li"); // Lấy theo tag name
        console.log(liElements); // HTMLCollection [li, li]

        let firstParagraph = document.querySelector(".paragraph"); // Lấy element đầu tiên theo CSS selector
        console.log(firstParagraph); // <p class="paragraph">...</p>

        let allParagraphs = document.querySelectorAll(".paragraph"); // Lấy tất cả element theo CSS selector
        console.log(allParagraphs); // NodeList [p.paragraph, p.paragraph]
    </script>
</body>
</html>
```

### Lấy element trong DOM

Tiếp tục về các phương thức lấy element, có thể tập trung vào `querySelector` và `querySelectorAll` và các loại CSS selector có thể dùng (class, id, tag name, attribute selectors, pseudo-classes...).

### Lấy element trong DOM

Có thể đi sâu vào performance khi chọn element, cách tối ưu selector, và sự khác biệt giữa HTMLCollection và NodeList (HTMLCollection là live collection - tự động cập nhật khi DOM thay đổi, NodeList có thể là static hoặc live tùy phương thức lấy).

### Attribute node và Text node trong HTML DOM

Trong DOM tree, mỗi element HTML là một element node. Bên trong element node có thể có attribute nodes (thuộc tính HTML) và text nodes (nội dung text).

### DOM attribute

DOM API cung cấp các phương thức để thao tác với attribute nodes:

* `element.getAttribute(attributeName)`: Lấy giá trị attribute.
* `element.setAttribute(attributeName, value)`: Sửa đổi hoặc thêm attribute.
* `element.removeAttribute(attributeName)`: Xóa attribute.
* `element.hasAttribute(attributeName)`: Kiểm tra xem element có attribute không.

* **Ví dụ:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ví dụ DOM Attribute</title>
</head>
<body>
    <a id="link" href="https://f8.edu.vn" target="_blank">F8</a>

    <script>
        let linkElement = document.getElementById("link");
        console.log(linkElement.getAttribute("href")); // "https://f8.edu.vn"
        linkElement.setAttribute("title", "Học lập trình tại F8"); // Thêm attribute title
        console.log(linkElement.getAttribute("title")); // "Học lập trình tại F8"
        linkElement.removeAttribute("target"); // Xóa attribute target
        console.log(linkElement.hasAttribute("target")); // false
    </script>
</body>
</html>
```

### InnerText & textContent Property

`innerText` và `textContent` properties dùng để lấy hoặc set nội dung text của một element.

* `innerText`: Chỉ lấy text "hiển thị" (sau khi render), không lấy text của các element ẩn (ví dụ: `display: none`).
* `textContent`: Lấy **tất cả** text content, kể cả text của element ẩn. Nên dùng `textContent` vì chuẩn hơn, nhất quán hơn.

* **Ví dụ:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ví dụ innerText & textContent</title>
</head>
<body>
    <div id="content">
        <p>Đoạn văn bản 1.</p>
        <p style="display: none;">Đoạn văn bản 2 (ẩn).</p>
    </div>

    <script>
        let contentElement = document.getElementById("content");
        console.log(contentElement.innerText);
        // Đoạn văn bản 1.
        console.log(contentElement.textContent);
        // Đoạn văn bản 1.
        // Đoạn văn bản 2 (ẩn).
    </script>
</body>
</html>
```

### Thêm element vào element trong DOM

* **Tóm tắt:**

* `element.innerHTML`: Lấy hoặc set **HTML content bên trong** element (dạng chuỗi HTML). Có thể dùng để thêm HTML vào element.
* `element.outerHTML`: Lấy hoặc set **HTML content của chính element và bên trong nó** (dạng chuỗi HTML).

* **Ví dụ:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ví dụ innerHTML & outerHTML</title>
</head>
<body>
    <div id="container">
        <p>Đoạn văn bản ban đầu.</p>
    </div>

    <script>
        let containerElement = document.getElementById("container");
        console.log(containerElement.innerHTML); // "<p>Đoạn văn bản ban đầu.</p>"

        containerElement.innerHTML = "<h2>Tiêu đề mới</h2><p>Đoạn văn bản mới.</p>"; // Set HTML content mới
        console.log(containerElement.innerHTML);
        // "<h2>Tiêu đề mới</h2><p>Đoạn văn bản mới.</p>"

        console.log(containerElement.outerHTML);
        // "<div id="container"><h2>Tiêu đề mới</h2><p>Đoạn văn bản mới.</p></div>"
    </script>
</body>
</html>
```

### Node properties

Node properties (thuộc tính node) cung cấp thông tin về node trong DOM tree. Ví dụ:
* `node.nodeName`: Tên node (tag name cho element node, "\#text" cho text node...).
* `node.nodeType`: Loại node (1: element node, 3: text node...).
* `node.parentNode`: Node cha.
* `node.childNodes`: Danh sách node con (HTMLCollection/NodeList).
* `node.firstChild`, `node.lastChild`, `node.nextSibling`, `node.previousSibling`: Node con đầu, con cuối, node anh em kế tiếp, node anh em trước đó.

### Đối tượng DOM style trong Element node

`element.style` object cho phép truy cập và sửa đổi inline styles (style viết trực tiếp trong attribute `style`) của element từ JavaScript.

* **Ví dụ:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ví dụ DOM Style</title>
</head>
<body>
    <div id="box" style="background-color: lightblue; width: 200px; height: 100px;">
        Khối hộp
    </div>

    <script>
        let boxElement = document.getElementById("box");
        console.log(boxElement.style.backgroundColor); // "lightblue" (lấy style background-color)
        boxElement.style.color = "red"; // Set style color
        boxElement.style.border = "2px solid black"; // Set style border
    </script>
</body>
</html>
```

### ClassList Property

`element.classList` property trả về một đối tượng `DOMTokenList` đại diện cho danh sách class của element. Cung cấp các phương thức để thao tác với class:

* `classList.add(className)`: Thêm class.
* `classList.remove(className)`: Xóa class.
* `classList.toggle(className)`: Thêm class nếu chưa có, xóa class nếu đã có.
* `classList.contains(className)`: Kiểm tra xem element có class không.

* **Ví dụ:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ví dụ classList</title>
    <style>
        .highlight {
            background-color: yellow;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <p id="text">Đoạn văn bản.</p>
    <button id="toggleBtn">Toggle Highlight</button>

    <script>
        let textElement = document.getElementById("text");
        let toggleButton = document.getElementById("toggleBtn");

        toggleButton.addEventListener("click", function() {
            textElement.classList.toggle("highlight"); // Toggle class "highlight"
        });
    </script>
</body>
</html>
```

### DOM events

DOM events (sự kiện DOM) là các hành động xảy ra trên trang web (click chuột, gõ phím, load trang...). JavaScript có thể lắng nghe (listen) và xử lý (handle) các sự kiện này để tạo tương tác.

### DOM events example

Ví dụ về các sự kiện DOM phổ biến:

* `click`: Click chuột.
* `mouseover`, `mouseout`: Chuột di vào, di ra khỏi element.
* `keydown`, `keyup`: Phím được nhấn, phím được nhả.
* `submit`: Form được submit.
* `load`: Trang hoặc resource (ảnh, script...) đã load xong.
* `DOMContentLoaded`: DOM tree đã được parse xong.

* **Ví dụ (sự kiện click):**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ví dụ DOM Event</title>
</head>
<body>
    <button id="myButton">Click me</button>
    <p id="message"></p>

    <script>
        let buttonElement = document.getElementById("myButton");
        let messageElement = document.getElementById("message");

        buttonElement.addEventListener("click", function() { // Lắng nghe sự kiện click
            messageElement.textContent = "Button đã được click!"; // Xử lý sự kiện click
        });
    </script>
</body>
</html>
```

### PreventDefault & StopPropagation

* **Tóm tắt:**

* `event.preventDefault()`: Ngăn chặn hành vi mặc định của sự kiện (ví dụ: ngăn link chuyển trang, ngăn form submit trang).
* `event.stopPropagation()`: Ngăn chặn sự kiện lan truyền lên các element cha (event bubbling).

* **Ví dụ (`preventDefault` trên link):**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ví dụ preventDefault</title>
</head>
<body>
    <a href="https://f8.edu.vn" id="link">Link F8</a>
    <script>
        let linkElement = document.getElementById("link");
        linkElement.addEventListener("click", function(event) {
            event.preventDefault(); // Ngăn link chuyển trang
            alert("Link click bị chặn!");
        });
    </script>
</body>
</html>
```

### Event listener

Event listener (bộ lắng nghe sự kiện) dùng để đăng ký (attach) một function (event handler) để xử lý một sự kiện trên một element.

* `element.addEventListener(eventType, eventHandler, useCapture)`: Đăng ký event listener.
* `element.removeEventListener(eventType, eventHandler, useCapture)`: Gỡ bỏ event listener.

```js
const button = document.querySelector(".btn")
button.addEventListener("click", function(event) {
  console.log("Hello!");
})

// OR using Javascript one-liners
button.addEventListener("click", event => console.log("Hello!"))
```
## Phần 6: JSON, Promise, ES6+

### JSON là gì? Được sử dụng ra sao trong JS?

JSON (JavaScript Object Notation) là định dạng dữ liệu text nhẹ, dễ đọc, dễ parse, dựa trên cú pháp object của JavaScript. Dùng phổ biến để trao đổi dữ liệu giữa server và client trong web development (ví dụ: API).

* Cấu trúc: key-value pairs, key là chuỗi, value có thể là string, number, boolean, null, array, object.

* Ví dụ JSON:

```json
    {
        "name": "Gemini",
        "age": 2,
        "isRobot": true,
        "skills": ["learning", "coding", "talking"]
    }
```

* **JavaScript built-in object `JSON` cung cấp:**

* `JSON.stringify(object)`: Chuyển đổi object JavaScript sang chuỗi JSON.
* `JSON.parse(jsonString)`: Chuyển đổi chuỗi JSON sang object JavaScript.

* **Ví dụ:**

```javascript
let personObject = { name: "Gemini", age: 2 };
let jsonString = JSON.stringify(personObject); // Chuyển object sang JSON string
console.log(jsonString); // '{"name":"Gemini","age":2}'

let parsedObject = JSON.parse(jsonString); // Chuyển JSON string sang object
console.log(parsedObject.name); // "Gemini"
```

### Promise (sync async) trong JavaScript

Promise là object đại diện cho kết quả (thành công hoặc thất bại) của một tác vụ **bất đồng bộ** (asynchronous) và có thể chưa hoàn thành ngay lập tức (ví dụ: gọi API, đọc file...). Giúp xử lý bất đồng bộ một cách dễ đọc, dễ quản lý hơn so với callback.
* **Trạng thái Promise:**
    * `pending` (chờ xử lý): Tác vụ chưa hoàn thành.
    * `fulfilled` (thành công): Tác vụ hoàn thành thành công.
    * `rejected` (thất bại): Tác vụ hoàn thành thất bại.

### Promise (nỗi đau)

Có thể nói về "callback hell" và tại sao Promise ra đời để giải quyết vấn đề callback hell. Promise giúp code bất đồng bộ dễ đọc, dễ maintain hơn bằng cách "chaining" các tác vụ bất đồng bộ tuần tự hoặc song song.

### Promise trong Javascript

Cách tạo Promise: `new Promise((resolve, reject) => { ... });`

* `resolve(value)`: Gọi khi tác vụ thành công, truyền giá trị kết quả.
* `reject(error)`: Gọi khi tác vụ thất bại, truyền lỗi.

* **Cách xử lý kết quả Promise:**

* `.then(onFulfilled)`: Xử lý khi Promise fulfilled (thành công).
* `.catch(onRejected)`: Xử lý khi Promise rejected (thất bại).
* `.finally(onFinally)`: Thực hiện code sau khi Promise fulfilled hoặc rejected (không quan tâm kết quả), thường dùng để cleanup (ví dụ: tắt loading indicator).

* **Ví dụ (Promise đơn giản):**

```javascript
let myPromise = new Promise((resolve, reject) => {
    setTimeout(function() {
        let success = true; // Giả lập tác vụ thành công/thất bại
        if (success) {
            resolve("Dữ liệu thành công!"); // Gọi resolve khi thành công
        } else {
            reject("Lỗi xảy ra!"); // Gọi reject khi thất bại
        }
    }, 2000);
});

myPromise.then(function(result) { // Xử lý khi thành công
    console.log("Thành công:", result); // "Thành công: Dữ liệu thành công!"
}).catch(function(error) { // Xử lý khi thất bại
    console.log("Lỗi:", error); // "Lỗi: Lỗi xảy ra!" (nếu success = false)
}).finally(function() { // Thực hiện sau khi Promise xong (dù thành công hay thất bại)
    console.log("Promise đã hoàn thành.");
});
```

### Promise chain

Promise chaining (chuỗi Promise) cho phép liên kết các tác vụ bất đồng bộ tuần tự. `.then()` có thể trả về một Promise mới, tạo thành chuỗi. Giúp xử lý các tác vụ phụ thuộc lẫn nhau một cách tuần tự.

* **Ví dụ (Promise chain):**

```javascript
function fetchData(url) {
    return new Promise((resolve, reject) => {
        // Giả lập fetch API
        setTimeout(function() {
            let data = "Dữ liệu từ " + url;
            resolve(data);
        }, 1000);
    });
}

fetchData("url1").then(function(data1) { // Gọi API 1
    console.log("Dữ liệu 1:", data1); // Xử lý dữ liệu 1
    return fetchData("url2"); // Trả về Promise mới để gọi API 2
}).then(function(data2) { // Chạy khi Promise trả về từ .then() trước đó fulfilled
    console.log("Dữ liệu 2:", data2); // Xử lý dữ liệu 2
    return fetchData("url3"); // Tiếp tục chain
}).then(function(data3) {
    console.log("Dữ liệu 3:", data3);
}).catch(function(error) { // Bắt lỗi nếu có lỗi ở bất kỳ Promise nào trong chuỗi
    console.log("Lỗi:", error);
});
```

### Promise methods (resolve, reject, all)

Các static methods của `Promise` object:

* `Promise.resolve(value)`: Trả về một Promise đã fulfilled với giá trị `value`.
* `Promise.reject(error)`: Trả về một Promise đã rejected với lỗi `error`.
* `Promise.all(promises)`: Nhận vào một mảng các Promises, trả về một Promise mới fulfilled khi **tất cả** Promises trong mảng fulfilled, hoặc rejected ngay lập tức nếu có **ít nhất một** Promise rejected. Dùng để chạy các tác vụ bất đồng bộ song song và đợi tất cả hoàn thành.

* **Ví dụ (`Promise.all`):**

```javascript
let promise1 = Promise.resolve("Promise 1 thành công");
let promise2 = new Promise(resolve => setTimeout(() => resolve("Promise 2 thành công"), 1000));
let promise3 = Promise.resolve("Promise 3 thành công");

Promise.all([promise1, promise2, promise3]).then(function(results) { // Chạy song song, đợi tất cả xong
    console.log("Tất cả Promises thành công:", results); // ["Promise 1 thành công", "Promise 2 thành công", "Promise 3 thành công"]
}).catch(function(error) {
    console.log("Có lỗi:", error);
});
```

### Học về JavaScript ECMAScript 6

ECMAScript 6 (ES6) hoặc ES2015 là phiên bản JavaScript ra mắt năm 2015, giới thiệu nhiều tính năng mới, hiện đại, giúp code JavaScript mạnh mẽ và dễ viết hơn. Các tính năng ES6 quan trọng: `let`, `const`, arrow function, template literals, classes, modules, destructuring, spread operator...

Sẽ được cập nhật dần bên dưới 

### Let & Const keyword

(Đã đề cập ở mục 5) Ôn lại và so sánh `let` và `const` với `var`. Nên ưu tiên dùng `let` và `const` thay cho `var` vì có phạm vi block-scoped rõ ràng hơn, tránh lỗi hoisting.

### Arrow function trong JavaScript ES6

(Đã đề cập ở mục 29) Ôn lại arrow function, cú pháp ngắn gọn hơn cho anonymous function, đặc biệt hữu ích trong callback functions.

```js
const multiplyByTwo = (num) => {
    return num * 2;
}
```

### Template literals (Template string) trong javascript ES6

Template literals (template string) dùng backtick \`\` để khai báo chuỗi, cho phép nhúng biến trực tiếp vào chuỗi bằng cú pháp `${variable}` (string interpolation), và hỗ trợ chuỗi nhiều dòng dễ dàng.

* **Ví dụ:**

```javascript
let name = "Gemini";
let age = 2;
let message = `Xin chào, tôi là ${name}, ${age} tuổi.
Tôi là một robot.`; // Template literals, chuỗi nhiều dòng
console.log(message);
// Xin chào, tôi là Gemini, 2 tuổi.
// Tôi là một robot.
```

### Classes trong JavaScript ES6

Classes trong ES6 cung cấp cú pháp mới để định nghĩa object và kế thừa, gần gũi hơn với các ngôn ngữ hướng đối tượng khác (nhưng vẫn dựa trên prototype-based inheritance của JavaScript).

* **Ví dụ (Class cơ bản):**

```javascript
class Animal { // Định nghĩa class Animal
    constructor(name) { // Constructor
        this.name = name;
    }

    speak() { // Method speak
        console.log(this.name + " makes a sound.");
    }
}

class Dog extends Animal { // Class Dog kế thừa từ Animal
    constructor(name, breed) {
        super(name); // Gọi constructor của class cha
        this.breed = breed;
    }

    bark() { // Method bark riêng của Dog
        console.log("Woof!");
    }
}

let animal = new Animal("Generic Animal");
animal.speak(); // "Generic Animal makes a sound."

let dog = new Dog("Lucky", "Golden Retriever");
dog.speak(); // "Lucky makes a sound." (kế thừa từ Animal)
dog.bark(); // "Woof!" (method của Dog)
```

### Enhanced object literals trong javascript ES6

Enhanced object literals (object literals cải tiến) trong ES6 cung cấp cú pháp ngắn gọn hơn để tạo object:

* Shorthand property names: Nếu key và value có cùng tên biến, có thể viết tắt `key` thay vì `key: key`.
* Method shorthand: Bỏ từ khóa `function` khi định nghĩa method trong object.
* Computed property names: Key có thể là biểu thức được tính toán trong ngoặc vuông `[...]`.

* **Ví dụ:**

```javascript
let name = "Gemini";
let age = 2;

let person = {
    name, // Shorthand property name (tương đương name: name)
    age,  // Shorthand property name (tương đương age: age)
    greet() { // Method shorthand (bỏ function keyword)
        console.log("Xin chào, tôi là " + this.name);
    },
    ["skill" + "1"]: "learning" // Computed property name (key được tính toán)
};

console.log(person.name); // "Gemini"
person.greet(); // "Xin chào, tôi là Gemini"
console.log(person.skill1); // "learning"
```

### Default parameter values trong JavaScript ES6

Default parameter values (giá trị tham số mặc định) trong ES6 cho phép gán giá trị mặc định cho tham số của hàm. Nếu khi gọi hàm không truyền đối số cho tham số đó, tham số sẽ nhận giá trị mặc định.

* **Ví dụ:**

```javascript
function greet(name = "Guest") { // Tham số name có giá trị mặc định "Guest"
    console.log("Xin chào, " + name + "!");
}

greet("Gemini"); // "Xin chào, Gemini!" (truyền đối số)
greet(); // "Xin chào, Guest!" (không truyền đối số, dùng giá trị mặc định)
```

### Destructuring trong JavaScript ES6

Destructuring (phân rã cấu trúc) trong ES6 cho phép "giải nén" giá trị từ mảng hoặc object vào các biến riêng biệt một cách ngắn gọn.

* **Ví dụ (destructuring mảng):**

```javascript
let colors = ["red", "green", "blue"];
let [firstColor, secondColor, thirdColor] = colors; // Destructuring mảng

console.log(firstColor); // "red"
console.log(secondColor); // "green"
console.log(thirdColor); // "blue"
```

* **Ví dụ (destructuring object):**

```javascript
let person = { name: "Gemini", age: 2, city: "Internet" };
let { name, age } = person; // Destructuring object (lấy thuộc tính name và age)

console.log(name); // "Gemini"
console.log(age); // 2
```

### Spread trong JavaScript ES6

Spread operator (`...`) trong ES6 có nhiều ứng dụng:

* **Copy mảng/object:** Tạo bản sao nông (shallow copy) của mảng hoặc object.
* **Nối mảng:** Nối nhiều mảng thành một mảng mới.
* **Truyền đối số hàm:** Truyền các phần tử của mảng làm đối số riêng lẻ cho hàm.
* **Rest parameters (tham số rest):** Thu thập các đối số còn lại của hàm vào một mảng.

* **Ví dụ (copy mảng, nối mảng):**

```javascript
let arr1 = [1, 2, 3];
let arr2 = [...arr1]; // Copy mảng arr1
console.log(arr2); // [1, 2, 3]
arr2.push(4); // Thay đổi arr2 không ảnh hưởng arr1 (shallow copy)
console.log(arr1); // [1, 2, 3]

let arr3 = [4, 5, 6];
let combinedArray = [...arr1, ...arr3]; // Nối mảng arr1 và arr3
console.log(combinedArray); // [1, 2, 3, 4, 5, 6]
```

### Khái niệm tagged template literals (ít người biết)

Tagged template literals là một tính năng nâng cao của template literals. Cho phép bạn định nghĩa một "tag function" để xử lý template literal theo cách tùy chỉnh. Ít dùng trong thực tế hàng ngày, nhưng hữu ích trong một số trường hợp đặc biệt (ví dụ: sanitizing input, i18n...).

### Module trong JavaScript ES6

Modules trong ES6 cho phép chia code JavaScript thành các file (module) riêng biệt, giúp code có cấu trúc tốt hơn, dễ tái sử dụng, dễ bảo trì.

* `export`: Để export (xuất) các biến, hàm, class từ module.
* `import`: Để import (nhập) các module khác vào module hiện tại.

* **Ví dụ:**

* **`module1.js` (module 1):**

```javascript
    export const message = "Xin chào từ module 1!"; // Export biến
    export function greet(name) { // Export hàm
        console.log(message + " " + name);
    }
```

* **`main.js` (module chính):**

```javascript
    import { message, greet } from './module1.js'; // Import từ module1.js

    console.log(message); // "Xin chào từ module 1!"
    greet("User"); // "Xin chào từ module 1! User"
```

* **Trong HTML, cần thêm `type="module"` vào thẻ `<script>`:**

```html
    <script type="module" src="main.js"></script>
```

### Khái niệm Optional chaining

Optional chaining operator `?.` (ES2020+) giúp truy cập thuộc tính của object một cách an toàn, tránh lỗi khi object hoặc thuộc tính trung gian có thể `null` hoặc `undefined`. Nếu giá trị trước `?.` là `null` hoặc `undefined`, biểu thức trả về `undefined` ngay lập tức, không gây lỗi.

* **Ví dụ:**

```javascript
let user = {
    name: "Gemini",
    address: {
        city: "Internet"
    }
};

console.log(user.address?.city); // "Internet" (truy cập an toàn, nếu address có tồn tại)
console.log(user.profile?.email); // undefined (user.profile không tồn tại, không lỗi)

// Không dùng optional chaining, có thể gây lỗi:
// console.log(user.profile.email); // Lỗi: Cannot read property 'email' of undefined
```

### Fetch

Fetch API là built-in API hiện đại trong JavaScript để thực hiện các request HTTP (gọi API) một cách bất đồng bộ (dựa trên Promise). Thay thế cho `XMLHttpRequest` cũ.

* **Ví dụ (GET request với Fetch API):**

```javascript
fetch('https://jsonplaceholder.typicode.com/todos/1') // Gọi API GET
    .then(response => response.json()) // Parse response body thành JSON (trả về Promise)
    .then(data => { // Chạy khi Promise từ response.json() fulfilled
        console.log(data); // In ra dữ liệu JSON
    })
    .catch(error => { // Bắt lỗi nếu có lỗi trong quá trình fetch hoặc parse JSON
        console.error("Lỗi fetch:", error);
    });
```

### JSON server

JSON Server là thư viện Node.js giúp tạo nhanh REST API giả lập từ file JSON. Dùng để test frontend, làm backend demo, học API... Cài đặt bằng npm: `npm install -g json-server`. Chạy server: `json-server --watch db.json`.

### Phương thức reduce có logic như thế nào?

(Đã đề cập ở mục 51, 52) Ôn lại và đi sâu hơn về logic hoạt động của `reduce()` method, cách accumulator và currentValue thay đổi qua mỗi lần lặp, và các ứng dụng khác nhau của `reduce()`.

