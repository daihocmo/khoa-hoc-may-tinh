# Tự học ReactJS cũng rất là nhanh
Dựa trên khóa học của F8

## Phần 1: Giới thiệu ReactJS và Môi trường

### 1\. ReactJS là gì | Tại sao nên học ReactJS | Khóa học ReactJS miễn phí

* **Tóm tắt:** ReactJS là một thư viện JavaScript mã nguồn mở để xây dựng giao diện người dùng (UI). Được phát triển bởi Facebook, ReactJS nổi bật với các ưu điểm:
    * **Component-based:**  Xây dựng UI từ các thành phần độc lập, tái sử dụng.
    * **Declarative:**  Mô tả UI mong muốn, React tự động cập nhật DOM khi dữ liệu thay đổi.
    * **Virtual DOM:** Tăng hiệu năng bằng cách chỉ cập nhật những phần DOM thực sự thay đổi.
    * **Cộng đồng lớn:**  Nhiều tài liệu, thư viện hỗ trợ, dễ dàng tìm kiếm giúp đỡ.
    * **Việc làm rộng mở:**  ReactJS là một trong những thư viện/framework frontend phổ biến nhất hiện nay.

### 2\. SPA/MPA là gì | Khái niệm SPA |  ReactJS

* **Tóm tắt:** Phân biệt giữa SPA (Single Page Application - Ứng dụng Một Trang) và MPA (Multi Page Application - Ứng dụng Nhiều Trang):
    * **MPA:** Mỗi trang là một file HTML riêng biệt, khi chuyển trang trình duyệt tải lại toàn bộ trang.
    * **SPA:**  Tải một trang HTML duy nhất ban đầu, sau đó cập nhật nội dung động bằng JavaScript mà không cần tải lại trang. ReactJS thường dùng để xây dựng SPA, mang lại trải nghiệm mượt mà hơn cho người dùng.

### 3\. Arrow function trong JavaScript ES6 | Khái niệm arrow function

* **Tóm tắt:**  (Ôn lại từ Javascript cơ bản) Arrow function là cú pháp ngắn gọn hơn để viết function trong JavaScript ES6. Cú pháp: `(parameters) => expression` hoặc `(parameters) => { statements }`.

### 4\. Module trong JavaScript ES6

* **Tóm tắt:** (Ôn lại từ Javascript cơ bản)  Module trong ES6 giúp chia code JavaScript thành các file riêng biệt, dễ quản lý và tái sử dụng. Sử dụng `export` để xuất và `import` để nhập module.

### 5\. Enhanced object literals trong javascript ES6

* **Tóm tắt:** (Ôn lại từ Javascript cơ bản) Enhanced object literals cung cấp cú pháp ngắn gọn hơn để tạo object trong ES6, bao gồm shorthand property names, method shorthand, và computed property names.

### 6\. Spread trong JavaScript ES6

* **Tóm tắt:** (Ôn lại từ Javascript cơ bản) Spread operator (`...`) dùng để copy mảng/object, nối mảng, truyền đối số hàm, và rest parameters.

### 7\. Destructuring trong JavaScript ES6

* **Tóm tắt:** (Ôn lại từ Javascript cơ bản) Destructuring giúp "giải nén" giá trị từ mảng hoặc object vào các biến riêng biệt một cách ngắn gọn.

### 8\. document.createElement() để làm gì | Phương thức createElement

* **Tóm tắt:** `document.createElement(tagName)` là phương thức DOM API của JavaScript để tạo mới một element HTML. Tuy nhiên, trong ReactJS, chúng ta **ít khi** sử dụng trực tiếp `document.createElement()`. Thay vào đó, ReactJS cung cấp cách tiếp cận **declarative** hơn thông qua JSX và React Elements.

### 9\. Lưu ý! React đã có version 18 | Video bổ sung khóa học ReactJS F8

* **Tóm tắt:**  Lưu ý rằng React đã có phiên bản 18 (tại thời điểm khóa học). Khóa học có thể sử dụng phiên bản React cũ hơn (17), nhưng các khái niệm cơ bản vẫn tương tự. Có một số thay đổi và cải tiến trong React 18 (ví dụ: Concurrent Rendering) nhưng không ảnh hưởng lớn đến việc học cơ bản.

### 10\. Thêm React vào Website | Github, NPMJS, UNPKG là gì?

* **Tóm tắt:** Các cách thêm ReactJS vào website:
    * **Trực tiếp từ CDN (UNPKG):**  Thêm thẻ `<script>` vào HTML để tải ReactJS từ CDN (Content Delivery Network) như UNPKG. Dễ dàng cho mục đích học tập hoặc dự án nhỏ.
    * **Sử dụng NPM và Webpack (hoặc Create React App):**  Dùng cho dự án lớn, chuyên nghiệp. Cần cài đặt NodeJS, NPM (Node Package Manager), và bundler (Webpack) để quản lý thư viện, build code.
    * **Github:**  Nền tảng lưu trữ và quản lý code, nơi ReactJS và nhiều thư viện khác được phát triển và chia sẻ.
    * **NPMJS:**  Website và registry chính thức cho các package (thư viện) JavaScript, bao gồm ReactJS.

### 11\. Phương thức React.createElement() của thư viện ReactJS

* **Tóm tắt:** `React.createElement(type, [props], ...children)` là hàm cốt lõi của ReactJS để tạo ra **React Element**. React Element là một object mô tả UI, không phải DOM thật.
    * `type`:  Loại element (tag name như 'div', 'span', hoặc React Component).
    * `props`:  Props (thuộc tính) của element, truyền dữ liệu từ component cha xuống con.
    * `children`:  Các React Element con.

* **Ví dụ:**

```javascript
// Tạo React Element tương đương <h1 id="title">Xin chào React!</h1>
const titleElement = React.createElement(
    'h1',
    { id: 'title' },
    'Xin chào React!'
);
```

### 12\. React-DOM là gì? | Tại sao cần React-DOM?

* **Tóm tắt:** `react-dom` là một package riêng biệt đi kèm với ReactJS. Chức năng chính của `react-dom` là **render** (hiển thị) React Element lên DOM thật của trình duyệt.
    * `ReactDOM.render(reactElement, containerNode)` (React 17 trở về trước): Render React Element vào một DOM node (containerNode).
    * `ReactDOM.createRoot(containerNode).render(reactElement)` (React 18 trở lên):  Sử dụng `createRoot` để tạo root và render.

### 13\. Sử dụng ReactDOM Version 18 | Video bổ sung khóa học ReactJS F8

* **Tóm tắt:** Hướng dẫn cách sử dụng `ReactDOM.createRoot` trong React 18 để render ứng dụng React.

### 14\. JSX là gì? Tại sao cần JSX? | JSX ReactJS

* **Tóm tắt:** JSX (JavaScript XML) là một mở rộng cú pháp cho JavaScript, cho phép viết code HTML-like trực tiếp trong file JavaScript. JSX giúp code React dễ đọc, dễ viết, gần gũi hơn với HTML. JSX **không phải** là HTML thật, mà được Babel biên dịch thành các lệnh gọi `React.createElement()`.

* **Ví dụ (JSX):**

```jsx
// JSX code
const jsxElement = <h1 id="title">Xin chào JSX!</h1>;

// Tương đương với React.createElement():
const reactElement = React.createElement(
    'h1',
    { id: 'title' },
    'Xin chào JSX!'
);
```

### 15\. Sử dụng JSX render Arrays | Giải đáp JSX | JSX FQA

* **Tóm tắt:**  Cách render mảng các phần tử JSX. Cần đảm bảo mỗi phần tử trong mảng có một prop `key` duy nhất để React có thể theo dõi và cập nhật hiệu quả.

* **Ví dụ (render mảng JSX):**

```jsx
const items = ['Item 1', 'Item 2', 'Item 3'];
const list = (
    <ul>
    {items.map((item, index) => (
        <li key={index}>{item}</li> // Thêm key prop cho mỗi li
    ))}
    </ul>
);
```

### 16\. React element types | React components

* **Tóm tắt:**  React Element có 2 loại chính:
    * **DOM Element:**  Đại diện cho các tag HTML thông thường (ví dụ: `<h1>`, `<div>`, `<p>`). Được tạo ra bằng cách truyền string tag name vào `React.createElement()` hoặc viết tag HTML trong JSX.
    * **Component Element:**  Đại diện cho React Component (tự định nghĩa). Được tạo ra bằng cách truyền React Component vào `React.createElement()` hoặc viết tag component trong JSX (ví dụ: `<MyComponent />`).

### 17\. Props là gì? | Dùng props khi nào? | Khái niệm Props

* **Tóm tắt:** Props (properties) là cơ chế để truyền dữ liệu từ **component cha xuống component con**. Props là object chứa các thuộc tính, được truyền vào component con như attribute HTML. Component con nhận props và sử dụng để render UI. Props là **read-only** (chỉ đọc) từ bên trong component con.

* **Ví dụ (truyền props):**

```jsx
// Component cha
function ParentComponent() {
    return (
    <ChildComponent name="Gemini" age={2} /> // Truyền props name và age cho ChildComponent
    );
}

// Component con
function ChildComponent(props) { // Component con nhận props
    return (
    <div>
        <p>Tên: {props.name}</p> {/* Sử dụng props.name */}
        <p>Tuổi: {props.age}</p>   {/* Sử dụng props.age */}
    </div>
    );
}
```

### 18\. DOM events? | Làm việc với JSX - phần 1

* **Tóm tắt:**  Cách xử lý DOM events (sự kiện DOM) trong JSX.  Trong JSX, event handlers được đặt trực tiếp vào element như attribute, với tên event dạng `onEventName` (ví dụ: `onClick`, `onChange`, `onSubmit`). Giá trị của event handler là một function.

* **Ví dụ (xử lý sự kiện click):**

```jsx
function MyButton() {
    function handleClick() {
    alert('Button đã được click!');
    }

    return (
    <button onClick={handleClick}> {/*  onClick event handler */}
        Click me
    </button>
    );
}
```

### 19\. Tạo Components | Làm việc với JSX - Phần 2

* **Tóm tắt:**  Component là khối xây dựng cơ bản của ReactJS. Có 2 loại component chính:
    * **Function Component:**  Component là một function JavaScript, trả về JSX.  Thường dùng Hooks để quản lý state và lifecycle.
    * **Class Component (ít dùng hơn trong React hiện đại):** Component là một class ES6 kế thừa từ `React.Component`. Có state và lifecycle methods.

* **Ví dụ (Function Component):**

```jsx
function WelcomeMessage(props) { // Function Component, nhận props
    return <h1>Xin chào, {props.name}!</h1>;
}
```

### 20\. Children props & Render props | Làm việc với JSX - Phần 3

* **Tóm tắt:**
    * **Children props:**  Prop đặc biệt `children` dùng để truyền nội dung (React Elements) vào giữa cặp thẻ mở và đóng của component.
    * **Render props (ít dùng trong React hiện đại):**  Một kỹ thuật để component cha điều khiển cách component con render UI, bằng cách truyền một function (render prop) xuống component con.  Thường được thay thế bằng Higher-Order Components (HOCs) hoặc Hooks.

* **Ví dụ (children props):**

```jsx
// Component Container, nhận children props
function Container(props) {
    return (
    <div className="container">
        {props.children} {/* Render children props */}
    </div>
    );
}

// Sử dụng Container component
function App() {
    return (
    <Container> {/* Truyền nội dung vào Container component */}
        <p>Đây là nội dung bên trong Container.</p>
        <button>Nút bấm</button>
    </Container>
    );
}
```

### 21\. NodeJS là gì? Sử dụng NodeJS trong ReactJS? | cài đặt NodeJS

* **Tóm tắt:** NodeJS là môi trường runtime JavaScript phía server. Trong ReactJS, NodeJS cần thiết để:
    * **Chạy các công cụ build:**  NPM, Yarn, Create React App, Webpack...
    * **Phát triển backend (tùy chọn):**  Có thể dùng NodeJS để xây dựng backend cho ứng dụng React (ví dụ: API server).

### 22\. Hãy cài đúng React & ReactDOM 17 ở bài sau | Video bổ sung

* **Tóm tắt:**  Hướng dẫn cài đặt React và ReactDOM phiên bản 17 (phiên bản được sử dụng trong khóa học). Tuy nhiên, nếu bạn học sau này, nên cài phiên bản React mới nhất (ví dụ: 18) và tham khảo tài liệu cập nhật.

### 23\. Tạo dự án với React và Webpack | React JS

* **Tóm tắt:**  Hướng dẫn cách tự cấu hình dự án React từ đầu với Webpack (module bundler). Webpack giúp đóng gói code JavaScript, CSS, assets... thành bundle để trình duyệt có thể hiểu được.  Tuy nhiên, việc cấu hình Webpack khá phức tạp cho người mới bắt đầu.

### 24\. Nâng cấp React & ReactDOM từ version 17 lên 18 | ReactJS

* **Tóm tắt:** Hướng dẫn nâng cấp dự án React từ phiên bản 17 lên 18.

### 25\. Thư viện Create React App | Cài đặt thư viện cho Windows và MacOS

* **Tóm tắt:** Create React App (CRA) là công cụ chính thức của Facebook để tạo nhanh dự án ReactJS. CRA đã cấu hình sẵn Webpack, Babel, các công cụ cần thiết, giúp người mới bắt đầu dễ dàng tạo và chạy dự án React mà không cần lo lắng về cấu hình phức tạp.

### 26\. Hiểu rõ hơn về NPM, NPX và YARN | Cài đặt thư viện cho dự án

* **Tóm tắt:**  Các công cụ quản lý package (thư viện) JavaScript:
    * **NPM (Node Package Manager):**  Trình quản lý package mặc định của NodeJS.
    * **Yarn:**  Một trình quản lý package khác, tương tự NPM, có thể nhanh hơn trong một số trường hợp.
    * **NPX (Node Package eXecutor):**  Công cụ đi kèm NPM, dùng để chạy các package command-line (ví dụ: `npx create-react-app my-app`).

### 27\. CRA Folder Structure | Cấu trúc thư mục dự án | Create react app

* **Tóm tắt:**  Giải thích cấu trúc thư mục mặc định của dự án Create React App:
    * `node_modules`:  Thư mục chứa các thư viện (packages) đã cài đặt.
    * `public`:  Thư mục chứa các file public (ví dụ: `index.html`, favicon, assets tĩnh).
    * `src`:  Thư mục chứa code source của ứng dụng React (components, styles, logic...).
    * `package.json`:  File cấu hình dự án (dependencies, scripts...).
    * `package-lock.json` (hoặc `yarn.lock`):  File ghi lại phiên bản chính xác của các dependencies.

## Phần 2: Hooks - Quản lý State và Lifecycle

### 28\. Hooks là gì? | Khái niệm Hooks - React Hooks

* **Tóm tắt:** Hooks là các function đặc biệt trong React, cho phép **function component** có thể "hook vào" các tính năng của React trước đây chỉ có ở class component (ví dụ: state, lifecycle methods). Hooks giúp code function component mạnh mẽ hơn, dễ tái sử dụng logic, và code ngắn gọn hơn. Hooks **chỉ hoạt động** bên trong function component hoặc custom hooks.

### 29\. useState trong React hook | React hook 2021

* **Tóm tắt:** `useState` hook là hook cơ bản nhất, dùng để thêm **state** (trạng thái) vào function component.
    * `const [state, setState] = useState(initialState);`
        * `state`:  Biến state, giá trị hiện tại của state.
        * `setState`:  Function để cập nhật state. Khi `setState` được gọi, component sẽ re-render (render lại UI).
        * `initialState`:  Giá trị khởi tạo của state.

* **Ví dụ (useState):**

```jsx
import React, { useState } from 'react';

function Counter() {
    const [count, setCount] = useState(0); // Khai báo state 'count' khởi tạo 0

    const handleIncrement = () => {
    setCount(count + 1); // Cập nhật state count, component re-render
    };

    return (
    <div>
        <p>Count: {count}</p>
        <button onClick={handleIncrement}>Increment</button>
    </div>
    );
}
```

### 30\. Two-way binding | Ràng buộc hai chiều | React hooks

* **Tóm tắt:** Two-way binding (ràng buộc hai chiều) là kỹ thuật liên kết dữ liệu giữa UI và state component. Khi UI (ví dụ: input field) thay đổi, state tự động cập nhật, và ngược lại. Trong React, two-way binding thường được thực hiện kết hợp `useState` hook và controlled components.

* **Ví dụ (two-way binding với useState):**

```jsx
import React, { useState } from 'react';

function InputField() {
    const [inputValue, setInputValue] = useState(''); // State cho giá trị input

    const handleInputChange = (event) => {
    setInputValue(event.target.value); // Cập nhật state khi input thay đổi
    };

    return (
    <div>
        <input
        type="text"
        value={inputValue}         // Giá trị input được liên kết với state
        onChange={handleInputChange} // Xử lý sự kiện onChange
        />
        <p>Bạn đã nhập: {inputValue}</p>
    </div>
    );
}
```

### 31\. Todolist with useState() | Xây dựng ứng dụng todolist | React hooks

* **Tóm tắt:**  Thực hành xây dựng ứng dụng Todolist đơn giản sử dụng `useState` hook để quản lý danh sách todo, thêm, xóa, sửa todo.

### 32\. Tìm hiểu về thuật ngữ Mounted & Unmounted

* **Tóm tắt:**  Lifecycle của component trong React:
    * **Mounting:**  Component được tạo và chèn vào DOM lần đầu tiên.
    * **Updating:**  Component được render lại khi props hoặc state thay đổi.
    * **Unmounting:** Component bị xóa khỏi DOM.

### 33\. React useEffect hook chi tiết dành cho người mới | React JS

* **Tóm tắt:** `useEffect` hook là hook quan trọng nhất để xử lý **side effects** (tác dụng phụ) trong function component. Side effects là các tác vụ tương tác với "thế giới bên ngoài" React component, ví dụ:
    * Gọi API (fetch data).
    * DOM manipulation (thay đổi DOM trực tiếp - ít dùng trong React).
    * Timer functions (setTimeout, setInterval).
    * Logging.

* **Cú pháp:** `useEffect(callback, [dependencies]);`
    * `callback`:  Function chứa side effect code, sẽ được chạy sau mỗi lần render (hoặc sau lần render đầu tiên, tùy thuộc vào `dependencies`).
    * `dependencies` (tùy chọn): Mảng các giá trị dependencies. React sẽ so sánh các giá trị này sau mỗi lần render.
        * Nếu `dependencies` **không được truyền**: `callback` chạy sau **mỗi lần render**.
        * Nếu `dependencies` là **mảng rỗng `[]`**: `callback` chỉ chạy **một lần sau lần render đầu tiên** (tương tự `componentDidMount` trong class component).
        * Nếu `dependencies` là **mảng có giá trị**: `callback` chạy khi lần render đầu tiên và khi **bất kỳ giá trị nào trong `dependencies` thay đổi** (tương tự `componentDidUpdate` trong class component).

* **Ví dụ (useEffect với mảng rỗng `[]` - chạy một lần sau render đầu tiên):**

```jsx
import React, { useState, useEffect } from 'react';

function MyComponent() {
    const [data, setData] = useState(null);

    useEffect(() => {
    // Gọi API fetch data khi component mounted (render lần đầu)
    fetch('https://api.example.com/data')
        .then(response => response.json())
        .then(data => setData(data));
    }, []); // Mảng dependencies rỗng -> chỉ chạy một lần sau render đầu

    if (!data) {
    return <p>Loading...</p>;
    }

    return (
    <div>
        {/* Render data */}
        <p>Data: {data.value}</p>
    </div>
    );
}
```

### 34\. useEffect() with dependencies | React hooks 2021 | React JS

* **Tóm tắt:**  Đi sâu hơn về `useEffect` hook với `dependencies`. Giải thích cách React theo dõi dependencies và khi nào `callback` function được chạy lại.

### 35\. useEffect() with DOM events | React hooks 2021 | React JS

* **Tóm tắt:**  Sử dụng `useEffect` để đăng ký và hủy đăng ký DOM events (ví dụ: `window.addEventListener`, `document.addEventListener`).  Cần cleanup event listener khi component unmounted để tránh memory leaks.

* **Ví dụ (useEffect với DOM event - scroll event):**

```jsx
import React, { useState, useEffect } from 'react';

function ScrollIndicator() {
    const [scrollY, setScrollY] = useState(0);

    useEffect(() => {
    const handleScroll = () => {
        setScrollY(window.scrollY); // Cập nhật scrollY state khi scroll
    };

    window.addEventListener('scroll', handleScroll); // Đăng ký event listener

    return () => { // Cleanup function (chạy khi component unmounted)
        window.removeEventListener('scroll', handleScroll); // Hủy đăng ký event listener
    };
    }, []); // Mảng dependencies rỗng -> chỉ đăng ký và hủy đăng ký một lần

    return (
    <div>
        <p>Scroll Y: {scrollY}</p>
    </div>
    );
}
```

### 36\. useEffect() with timer functions | Làm việc với setInterval & setTimeout

* **Tóm tắt:**  Sử dụng `useEffect` để làm việc với timer functions (`setTimeout`, `setInterval`). Cần cleanup timer (clear timeout/interval) khi component unmounted để tránh memory leaks và các hành vi không mong muốn.

* **Ví dụ (useEffect với setInterval - cập nhật thời gian):**

```jsx
import React, { useState, useEffect } from 'react';

function Timer() {
    const [time, setTime] = useState(new Date());

    useEffect(() => {
    const intervalId = setInterval(() => { // Thiết lập interval
        setTime(new Date()); // Cập nhật time state mỗi giây
    }, 1000);

    return () => { // Cleanup function (chạy khi component unmounted)
        clearInterval(intervalId); // Xóa interval
    };
    }, []); // Mảng dependencies rỗng -> chỉ thiết lập và xóa interval một lần

    return (
    <div>
        <p>Current Time: {time.toLocaleTimeString()}</p>
    </div>
    );
}
```

### 37\. useEffect() with preview avatar | Hàm dọn dẹp Cleanup function

* **Tóm tắt:**  Ví dụ thực tế sử dụng `useEffect` và cleanup function để preview avatar (ảnh đại diện) khi người dùng chọn file ảnh. Cleanup function có thể dùng để hủy các tác vụ bất đồng bộ đang chạy (ví dụ: hủy fetch request) hoặc giải phóng tài nguyên.

### 38\. useEffect() with fake Chat App | Xử lý các chức năng thời gian thực

* **Tóm tắt:**  Ví dụ phức tạp hơn sử dụng `useEffect` để xây dựng một ứng dụng chat giả lập, xử lý các chức năng thời gian thực (ví dụ: nhận tin nhắn mới sau mỗi khoảng thời gian).

### 39\. useLayoutEffect() hook | Phân biệt useEffect và useLayoutEffect | React JS

* **Tóm tắt:** `useLayoutEffect` hook tương tự `useEffect`, nhưng callback function của `useLayoutEffect` được chạy **đồng bộ** (synchronously) **ngay sau khi DOM được cập nhật, nhưng trước khi trình duyệt vẽ lại màn hình**. `useEffect` chạy **bất đồng bộ** (asynchronously) **sau khi trình duyệt đã vẽ lại màn hình**.
    * **`useLayoutEffect`:**  Chạy trước khi trình duyệt vẽ, có thể chặn rendering, dùng cho các tác vụ cần đo lường layout, DOM manipulation trước khi hiển thị lên màn hình (ví dụ: tính toán vị trí, kích thước element...). Cẩn thận khi dùng vì có thể ảnh hưởng đến performance.
    * **`useEffect`:**  Chạy sau khi trình duyệt vẽ, không chặn rendering, dùng cho hầu hết các side effects thông thường (gọi API, timer, event listener...). **Nên ưu tiên dùng `useEffect`**.

### 40\. useRef() hook | Cách sử dụng useRef() hook

* **Tóm tắt:** `useRef` hook dùng để tạo ra một **reference** (tham chiếu) đến một giá trị nào đó, giá trị này được giữ nguyên giữa các lần re-render của component. `useRef` trả về một object có thuộc tính `.current`, có thể được gán bất kỳ giá trị nào.
    * **Ứng dụng chính:**
        * Truy cập trực tiếp DOM element (ví dụ: focus vào input, gọi method của element).
        * Lưu trữ các giá trị mutable (có thể thay đổi) mà không gây re-render component (ví dụ: timer ID, giá trị đếm...).

* **Ví dụ (useRef để focus input):**

```jsx
import React, { useRef, useEffect } from 'react';

function FocusInput() {
    const inputRef = useRef(null); // Tạo ref, initial value null

    useEffect(() => {
    inputRef.current.focus(); // Focus vào input khi component mounted
    }, []);

    return (
    <input type="text" ref={inputRef} placeholder="Nhập gì đó..." /> {/* Gán ref cho input element */}
    );
}
```

### 41\. React.memo() HOC | Phương thức memo trong react | React JS

* **Tóm tắt:** `React.memo()` là một Higher-Order Component (HOC - component bậc cao) dùng để **memoize** (ghi nhớ) một function component. Memoization giúp **tối ưu hiệu năng** bằng cách **tránh re-render component nếu props không thay đổi**.  `React.memo()` chỉ so sánh props (shallow comparison).

* **Ví dụ (React.memo):**

```jsx
import React from 'react';

// Component con, được memoize
const MyComponent = React.memo(function MyComponent(props) {
    console.log('MyComponent re-rendered!'); // Log khi component re-render
    return <p>Value: {props.value}</p>;
});

function ParentComponent() {
    const [count, setCount] = useState(0);

    return (
    <div>
        <MyComponent value={count} /> {/* Truyền count prop */}
        <button onClick={() => setCount(count + 1)}>Increment Count</button>
    </div>
    );
}
```

### 42\. useCallback() hook | Tránh tạo ra hàm mới không cần thiết với useCallback()

* **Tóm tắt:** `useCallback` hook dùng để **memoize** (ghi nhớ) một **callback function**. Trả về một phiên bản memoized của callback function.  Giúp **tối ưu hiệu năng**, đặc biệt khi truyền callback function xuống các component con được memoize (`React.memo()`) hoặc dùng trong `useEffect` dependencies.  `useCallback` chỉ memoize function khi dependencies không thay đổi.

* **Cú pháp:** `const memoizedCallback = useCallback(callback, [dependencies]);`

* **Ví dụ (useCallback):**

```jsx
import React, { useState, useCallback } from 'react';

const MyButton = React.memo(({ onClick, label }) => {
    console.log('MyButton re-rendered!');
    return <button onClick={onClick}>{label}</button>;
});

function ParentComponent() {
    const [count1, setCount1] = useState(0);
    const [count2, setCount2] = useState(0);

    // Memoize incrementCount1 callback function
    const incrementCount1 = useCallback(() => {
    setCount1(count1 + 1);
    }, [count1]); // Dependency là count1

    // incrementCount2 không được memoize (tạo mới mỗi lần render)
    const incrementCount2 = () => {
    setCount2(count2 + 1);
    };

    return (
    <div>
        <MyButton label={`Count 1: ${count1}`} onClick={incrementCount1} /> {/* Truyền memoized callback */}
        <MyButton label={`Count 2: ${count2}`} onClick={incrementCount2} /> {/* Truyền non-memoized callback */}
    </div>
    );
}
```

### 43\. useMemo() hook | Tránh thực hiện lại 1 logic không cần thiết với useMemo()

* **Tóm tắt:** `useMemo` hook dùng để **memoize** (ghi nhớ) kết quả của một **expensive calculation** (tính toán tốn kém). Trả về giá trị đã được memoize. Giúp **tối ưu hiệu năng** bằng cách **tránh thực hiện lại tính toán nếu dependencies không thay đổi**. `useMemo` chỉ tính toán lại giá trị khi dependencies thay đổi.

* **Cú pháp:** `const memoizedValue = useMemo(() => expensiveCalculation(), [dependencies]);`

* **Ví dụ (useMemo):**

```jsx
import React, { useState, useMemo } from 'react';

function FibonacciCalculator() {
    const [number, setNumber] = useState(5);

    // Memoize kết quả tính Fibonacci
    const fibonacciResult = useMemo(() => {
    console.log('Calculating Fibonacci...'); // Log khi tính toán Fibonacci
    function fibonacci(n) {
        if (n <= 1) return n;
        return fibonacci(n - 1) + fibonacci(n - 2);
    }
    return fibonacci(number); // Expensive calculation
    }, [number]); // Dependency là number

    return (
    <div>
        <input
        type="number"
        value={number}
        onChange={(e) => setNumber(parseInt(e.target.value))}
        />
        <p>Fibonacci({number}) = {fibonacciResult}</p>
    </div>
    );
}
```

### 44\. useReducer() hook | Khi nào sử dụng useReducer()?

* **Tóm tắt:** `useReducer` hook là một hook nâng cao hơn `useState`, dùng để quản lý **complex state logic** (logic state phức tạp) hoặc khi state có **nhiều state transitions** (chuyển đổi trạng thái). `useReducer` tương tự `useState` nhưng quản lý state thông qua **reducer function** (hàm reducer) và **dispatch actions** (gửi action). Lấy cảm hứng từ Redux.

* **Cú pháp:** `const [state, dispatch] = useReducer(reducer, initialArg, init);`
    * `reducer(state, action)`: Hàm reducer, nhận state hiện tại và action, trả về state mới.
    * `initialArg`:  Initial state hoặc giá trị khởi tạo để truyền vào `init` function.
    * `init(initialArg)` (tùy chọn): Function để khởi tạo initial state một cách lazy (chỉ chạy một lần đầu).
    * `state`:  State hiện tại.
    * `dispatch(action)`: Function để gửi action tới reducer, kích hoạt cập nhật state.

* **Ví dụ (useReducer):**

```jsx
import React, { useReducer } from 'react';

// Reducer function
const counterReducer = (state, action) => {
    switch (action.type) {
    case 'INCREMENT':
        return { count: state.count + 1 };
    case 'DECREMENT':
        return { count: state.count - 1 };
    default:
        return state;
    }
};

const initialState = { count: 0 };

function CounterWithReducer() {
    const [state, dispatch] = useReducer(counterReducer, initialState); // useReducer hook

    return (
    <div>
        <p>Count: {state.count}</p>
        <button onClick={() => dispatch({ type: 'INCREMENT' })}>Increment</button> {/* Dispatch INCREMENT action */}
        <button onClick={() => dispatch({ type: 'DECREMENT' })}>Decrement</button> {/* Dispatch DECREMENT action */}
    </div>
    );
}
```

### 45\. Todo App with useReducer() hook | Hiểu rõ hơn về useReducer()

* **Tóm tắt:**  Thực hành xây dựng ứng dụng Todolist sử dụng `useReducer` hook để quản lý state phức tạp hơn (ví dụ: thêm, xóa, sửa, toggle completed, filter todo).

### 46\. useReducer() recap | React hooks 2021 | React JS

* **Tóm tắt:**  Tổng kết và ôn lại `useReducer` hook, so sánh với `useState`, khi nào nên dùng `useReducer`.

### 47\. React Context & useContext() hook | Khái niệm useContext()

* **Tóm tắt:** React Context API cung cấp cách chia sẻ dữ liệu (state) **toàn cục** (global state) cho toàn bộ cây component **mà không cần truyền props qua nhiều tầng component**.  `useContext` hook giúp function component truy cập context value.

* **Các bước sử dụng Context:**
    1. **Tạo Context:** `const MyContext = React.createContext(defaultValue);`
    2. **Provider:**  Component cha bọc các component con cần truy cập context, cung cấp value bằng prop `value`: `<MyContext.Provider value={contextValue}>...</MyContext.Provider>`.
    3. **Consumer (useContext hook):** Component con sử dụng `useContext(MyContext)` để truy cập `contextValue`.

* **Ví dụ (Context và useContext):**

```jsx
import React, { createContext, useContext, useState } from 'react';

// 1. Tạo Context
const ThemeContext = createContext('light'); // Default value 'light'

function App() {
    const [theme, setTheme] = useState('light');

    const toggleTheme = () => {
    setTheme(theme === 'light' ? 'dark' : 'light');
    };

    return (
    // 2. Provider, cung cấp theme value
    <ThemeContext.Provider value={theme}>
        <Toolbar />
        <button onClick={toggleTheme}>Toggle Theme</button>
    </ThemeContext.Provider>
    );
}

function Toolbar() {
    return (
    <div>
        <ThemedButton />
    </div>
    );
}

function ThemedButton() {
    // 3. Consumer (useContext hook), truy cập theme value
    const theme = useContext(ThemeContext);

    return (
    <button className={theme}>Themed Button</button>
    );
}
```

### 48\. Global State with Context + useReducer |  Trạng thái toàn cục

* **Tóm tắt:**  Kết hợp Context API và `useReducer` hook để tạo **global state management** (quản lý state toàn cục) mạnh mẽ. Context cung cấp cơ chế chia sẻ state, `useReducer` quản lý logic cập nhật state phức tạp. Mô hình tương tự Redux (nhưng đơn giản hơn).

### 49\. useImperativeHandle() hook | React JS

* **Tóm tắt:** `useImperativeHandle` hook là hook nâng cao, dùng để **customizing the ref** được expose (phơi bày) ra ngoài component con khi component cha sử dụng `ref` để truy cập component con. Thường dùng khi cần kiểm soát imperative (mệnh lệnh) component con từ component cha (ví dụ: focus input, gọi method của component con), nhưng **hạn chế sử dụng**, nên ưu tiên declarative approach (điều khiển component con qua props).

## Phần 3: Styling và Routing

### 50\. Sử dụng CSS trong dự án ReactJS | CSS in React

* **Tóm tắt:** Các cách styling CSS trong ReactJS:
    * **Inline Styles:**  Viết style trực tiếp trong attribute `style` của JSX element. Style là object JavaScript.
    * **External CSS Files:**  Import file CSS vào component. Class names trong CSS file có thể bị trùng nhau giữa các component (global scope).
    * **CSS Modules:**  Giải pháp để CSS có scope theo component, tránh xung đột class names. File CSS module có đuôi `.module.css`. Import class names từ CSS module vào component như object.
    * **CSS-in-JS Libraries:**  Thư viện viết CSS trực tiếp trong JavaScript (ví dụ: Styled Components, Emotion).

### 51\. CSS module là gì? | Sử dụng CSS module như thế nào?

* **Tóm tắt:**  CSS Modules (đã đề cập ở mục trên) là một cách để viết CSS có scope theo component. Khi sử dụng CSS Modules, mỗi class name trong CSS file sẽ được "hash" (băm) thành một tên class duy nhất, tránh xung đột class names giữa các component.

* **Ví dụ (CSS Modules):**

    * **`MyComponent.module.css`:**

    ```css
    .title {
        color: blue;
        font-size: 24px;
    }

    .container {
        border: 1px solid black;
        padding: 10px;
    }
    ```

    * **`MyComponent.js`:**

    ```jsx
    import React from 'react';
    import styles from './MyComponent.module.css'; // Import styles object

    function MyComponent() {
        return (
        <div className={styles.container}> {/* Sử dụng styles.container */}
            <h1 className={styles.title}>Hello CSS Modules</h1> {/* Sử dụng styles.title */}
            <p>This is a CSS Module example.</p>
        </div>
        );
    }
    ```

### 52\. Thư viện clsx và classnames | Sử dụng nhiều class & class động trong ReactJS

* **Tóm tắt:**  Thư viện `clsx` và `classnames` giúp quản lý class names trong ReactJS dễ dàng hơn, đặc biệt khi có nhiều class names hoặc class names thay đổi động dựa trên điều kiện.

* **Ví dụ (`classnames`):**

```jsx
import classNames from 'classnames';

function MyComponent(props) {
    const { isActive, isLarge } = props;

    const classes = classNames('my-component', { // Class cố định 'my-component'
    'active': isActive,        // Class 'active' chỉ thêm khi isActive là true
    'large': isLarge,          // Class 'large' chỉ thêm khi isLarge là true
    'disabled': !isActive && !isLarge // Class 'disabled' thêm khi cả isActive và isLarge đều false
    });

    return (
    <div className={classes}> {/* Sử dụng classes */}
        {/* ... */}
    </div>
    );
}
```

### 53\. Install SASS để dùng SCSS | Cài đặt và sử dụng SCSS trong dự án

* **Tóm tắt:** SCSS (Sassy CSS) là một CSS preprocessor, mở rộng CSS với các tính năng mạnh mẽ hơn (variables, nesting, mixins, functions...). Cần cài đặt SASS compiler để biên dịch file SCSS thành CSS. Trong ReactJS, có thể dùng SCSS kết hợp với CSS Modules.

### 54\. React Router V6 | Thư viện React router dom | Định tuyến trong ReactJS

* **Tóm tắt:** React Router DOM là thư viện routing phổ biến nhất cho ReactJS, giúp xây dựng SPA với nhiều "trang" (views) khác nhau, nhưng vẫn giữ nguyên trải nghiệm SPA (không tải lại trang khi chuyển "trang"). React Router V6 là phiên bản mới nhất, có nhiều cải tiến.

* **Các khái niệm chính trong React Router V6:**
    * **BrowserRouter:**  Component router cho web browser, dùng History API để quản lý URL.
    * **Routes, Route:**  Component `Routes` chứa các `Route` components. `Route` định nghĩa mapping giữa path (đường dẫn URL) và component hiển thị.
    * **Link, NavLink:**  Component để tạo link điều hướng giữa các "trang" trong SPA. `NavLink` là phiên bản đặc biệt của `Link`, có thể active class khi link active.
    * **useNavigate hook:**  Hook để điều hướng programmatically (ví dụ: sau khi submit form, chuyển trang...).
    * **useParams hook:**  Hook để lấy parameters từ URL path (ví dụ: `/users/:userId`).

* **Ví dụ (React Router V6 cơ bản):**

```jsx
import React from 'react';
import { BrowserRouter, Routes, Route, Link } from 'react-router-dom';

function Home() {
    return <h2>Home Page</h2>;
}

function About() {
    return <h2>About Page</h2>;
}

function App() {
    return (
    <BrowserRouter> {/* BrowserRouter bọc ứng dụng */}
        <nav>
        <ul>
            <li>
            <Link to="/">Home</Link> {/* Link to="/" */}
            </li>
            <li>
            <Link to="/about">About</Link> {/* Link to="/about" */}
            </li>
        </ul>
        </nav>

        <Routes> {/* Routes chứa các Route */}
        <Route path="/" element={<Home />} /> {/* Route cho path="/" render Home component */}
        <Route path="/about" element={<About />} /> {/* Route cho path="/about" render About component */}
        </Routes>
    </BrowserRouter>
    );
}
```
