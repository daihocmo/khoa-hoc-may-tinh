# Cấu trúc dữ liệu và giải thuật

Hướng dẫn này sẽ tập trung vào việc giúp bạn hiểu về cấu trúc dữ liệu và thuật toán. Về phần áp dụng thì bạn lên LeetCode, Hackerrank hoặc bất cứ nền tảng nào. Bạn cũng có thể sử dụng Algorithms Visualizer để có thể xem cách thuật toán vận hành.

## Kiến thức nền tảng

### Toán rời rạc

Đọc hết trong cuốn Giáo trình toán rời rạc - [Tổ hợp và đồ thị](http://math.ac.vn/training/images/TTDaotao/VinIF/Toanroirac_NHThach.pdf). Một số các chủ đề có thể kể đến:

- Các quy tắc đếm cơ bản: [Các quy tắc đếm cơ bản - Trường THPT chuyên Hà Nội - Amsterdam](https://www.google.com/search?q=https://hnams.edu.vn/data/uploads/files/Toan/Toan%252011/Toan%252011%2520NC/Chuong%25202/Bai%25201/Cac%2520quy%2520tac%2520dem%2520co%2520ban.pdf)
- Xác suất: [Chương 4: Xác suất - Tài liệu học tập](https://www.google.com/search?q=https://voer.edu.vn/m/chuong-4-xac-suat-e8139)
- Hoán vị & Tổ hợp: [Hoán vị - Chỉnh hợp - Tổ hợp - ToanMath.vn](https://www.google.com/search?q=https://toanmath.vn/hoan-vi-chinh-hop-to-hop/)
- Lý thuyết đồ thị: [Chương 1: Các khái niệm cơ bản về lý thuyết đồ thị - Tài liệu Bách Khoa](https://www.google.com/search?q=https://tailieubk.com/2016/10/chuong-1-cac-khai-niem-co-ban-ve-ly-thuyet-do-thi/)

### Đại cương

Được trích dẫn từ series [Algorithms Design Techniques](https://viblo.asia/s/algorithms-design-techniques-3vKjR8XkK2R) trên Viblo.

1.  [Cùng ôn lại các khái niệm về Cấu trúc dữ liệu, Giải thuật, Độ phức tạp thuật toán.](https://viblo.asia/p/cung-on-lai-cac-khai-niem-ve-cau-truc-du-lieu-giai-thuat-do-phuc-tap-thuat-toan-Eb85oVy6l2G)
2.  [Tìm hiểu về giải thuật Đệ Quy](https://viblo.asia/p/tim-hieu-ve-giai-thuat-de-quy-3Q75wVVQlWb)
3.  [Tìm hiểu về giải thuật Chia để Trị (Divide and Conquer)](https://viblo.asia/p/tim-hieu-ve-giai-thuat-chia-de-tri-divide-and-conquer-vyDZOkmkZwj)

Muốn "cưỡi ngựa xem hoa" một chút, đọc [8 kiểu cấu trúc dữ liệu mà mọi lập trình viên cần phải biết](https://viblo.asia/p/8-kieu-cau-truc-du-lieu-ma-moi-lap-trinh-vien-can-phai-biet-yMnKMmdEK7P)

### Lập trình "cơ bản"

Bạn có thể viết bằng mã giả (pseudocode) hoặc một ngôn ngữ bất kì, thường là Java hoặc Python.

### Tài nguyên khác

Phần lớn các bài viết được dẫn nguồn tới Viblo, và đây là một số nguồn bằng Tiếng Việt khác

  - [VNOI Wiki - Thuật toán](https://wiki.vnoi.info/)
  - [Chuong Le Hoang - DSA](https://lhchuong.wordpress.com/category/data-structures-algorithms/)
  - [Nguyễn Tuấn](https://chidokun.github.io/categories/gi%E1%BA%A3i-thu%E1%BA%ADt/)

## Cấu trúc dữ liệu

### Arrays và Linked Lists

  - **Arrays:** [Mảng (Array) trong C++ và ứng dụng](https://www.google.com/search?q=https://viblo.asia/p/mang-array-trong-c-va-ung-dung-naQjzvYkZWA)
  - **Linked Lists:** [LinkedList trong Java và các thao tác cơ bản](https://www.google.com/search?q=https://viblo.asia/p/linkedlist-trong-java-va-cac-thao-tac-co-ban-dje5Vj99lWj)

### Stacks và Queues

  - [ Ngăn xếp và Hàng đợi (Stack & Queue) ](https://viblo.asia/p/ngan-xep-va-hang-doi-stack-queue-yMnKM6MQZ7P) - Bài đọc trên Viblo
  - [Stack](https://www.youtube.com/watch?v=BxxG5aFEtBE&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=10&pp=iAQB) và [Stack Implementations](https://www.youtube.com/watch?v=bLafmb5KeWE&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=11&pp=iAQB) của Ông Dev
  - [Queue](https://www.youtube.com/watch?v=qpqSiYjS9-4&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=13&pp=iAQB) và [Queue Implementations](https://www.youtube.com/watch?v=EFdvAXaPYVY&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=14&pp=iAQB)

### Cây

  - Cây
      - [Tree là gì? Lý thuyết về Binary Tree](https://viblo.asia/p/chuong-6-trees-1-tree-la-gi-ly-thuyet-ve-binary-tree-obA46PM9LKv)
      - [Treeee](https://www.youtube.com/watch?v=eHoATJEDtww&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=16&pp=iAQB) - Video của ông Dev
  - Cây nhị phân
      - [Tree là gì? Lý thuyết về Binary Tree](https://viblo.asia/p/chuong-6-trees-1-tree-la-gi-ly-thuyet-ve-binary-tree-obA46PM9LKv)
      - [ Cấu trúc dữ liệu và thuật toán \#17: Binary Tree (DS\&A) ](https://www.youtube.com/watch?v=yjjFggRKHLw&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=18)
  - Cây tìm kiếm nhị phân:
      - [Cây tìm kiếm nhị phân](https://viblo.asia/p/chuong-6-trees-7cay-tim-kiem-nhi-phanbinary-search-trees-bsts-W13VMgkQJY7)
      - [ Cấu trúc dữ liệu và thuật toán \#18: Binary Search Tree (BST - DS\&A) ](https://www.youtube.com/watch?v=mQMpamkUgW8&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=18) và xem [video code của Ông Dev](https://www.youtube.com/watch?v=GhKJcr1Fri8&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=19)
  - B-tree
      - [Cấu trúc dữ liệu B+Tree và ứng dụng trong bài toán xử lý tập có thứ tự](https://viblo.asia/p/cau-truc-du-lieu-btree-va-ung-dung-trong-bai-toan-xu-ly-tap-co-thu-tu-Ljy5VWQjKra)
  - AVL trees: [Cây AVL - Lý thuyết và cài đặt](https://www.google.com/search?q=https://freetuts.net/cay-avl-ly-thuyet-va-cai-dat-1027.html)
  - Duyệt cây nhị phân (Tree traversal: inorder, preorder, postorder)
      - Đọc: [Lý thuyết về Duyệt cây nhị phân](https://viblo.asia/p/chuong-6-trees-2-ly-thuyet-ve-duyet-cay-nhi-phan-n1j4l36MVwl)
      - Video: [ 2. Duyệt cây ](https://www.youtube.com/watch?v=_6ZlEdC6hA8)

### Hash Tables và Sets:

  - **Hash Tables:** [Tìm hiểu về cấu trúc dữ liệu HashTable](https://www.google.com/search?q=https://viblo.asia/p/tim-hieu-ve-cau-truc-du-lieu-hashtable-dje5Vj99lWj)
  - **Sets:** [Set trong C++](https://www.google.com/search?q=https://viblo.asia/p/set-trong-c-YOWZnVw8KQ0)

Trích từ kho video của ông Dev:

  - [ Cấu trúc dữ liệu và thuật toán \#20: Hash table, hash function ](https://www.youtube.com/watch?v=uKIFNzqX2a8&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=20)
  - [ Cấu trúc dữ liệu và thuật toán \#21: Hashtable Separate Chaining](https://www.youtube.com/watch?v=kBS3xQTVzVg&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=21)
  - [ Cấu trúc dữ liệu và thuật toán \#23: Hashtable Open Addressing](https://www.youtube.com/watch?v=UhBql4zi_nk&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=23)
  - [ Cấu trúc dữ liệu và thuật toán \#24: Hashtable Linear Probing | DS\&A ](https://www.youtube.com/watch?v=i9e3pqoav5Q&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=25)
  - [ Cấu trúc dữ liệu và thuật toán \#25: Hashtable Quadratic Probing | DS\&A ](https://www.youtube.com/watch?v=0AW6TJM9yFA&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=26)
  - [ Cấu trúc dữ liệu và thuật toán \#26: Hashtable Double Hashing | DS\&A ](https://www.youtube.com/watch?v=Ix1PJgPvdVc&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=26)
  - [ Cấu trúc dữ liệu và thuật toán \#27: HT Open Addressing Removal | DS\&A ](https://youtu.be/dHTVTsJ6kDM)

### Đồ thị

  - Adjacency matrix and adjacency list representation: [Biểu diễn đồ thị trong C++ (Adjacency Matrix và Adjacency List)](https://www.google.com/search?q=https://viblo.asia/p/bieu-dien-do-thi-trong-c-adjacency-matrix-va-adjacency-list-dje5Vj99lWj)
  - Graph traversal (BFS, DFS)
      - BFS:
          - Bài đọc: [ Data Structure & Algorithm - Graph Algorithms - Breadth First Search (BFS) ](https://viblo.asia/p/data-structure-algorithm-graph-algorithms-breadth-first-search-bfs-gwd43kMM4X9)
      - DFS:
          - Bài đọc: [ Data Structure & Algorithm - Graph Algorithms - Depth First Search (DFS) ](https://viblo.asia/p/data-structure-algorithm-graph-algorithms-depth-first-search-dfs-qPoL7zyXJvk)
  - Bài toán cây khung nhỏ nhất (Kruskal's, Prim's)
      - Đọc [Bài toán cây khung nhỏ nhất ](https://viblo.asia/p/bai-toan-cay-khung-nho-nhat-W13VMoP8JY7) - Bài viết này đã bao gồm cả về bài toán Kruskal và bài toán Prim.
      - Kruskal:
          - Bài đọc: [ Thuật toán Kruskal: Tìm cây khung nhỏ nhất ](https://chidokun.github.io/2021/08/kruskal-algorithm/)
      - Prim:
          - Bài đọc: [ Thuật toán Prim tìm cây khung nhỏ nhất trong đồ thị ](https://viblo.asia/p/thuat-toan-prim-tim-cay-khung-nho-nhat-trong-do-thi-Ljy5VBX95ra)
  - Thuật toán tìm đường đi ngắn nhất (Dijkstra's, Bellman-Ford)
      - [Thuật toán Dijkstra và ứng dụng](https://viblo.asia/p/thuat-toan-dijkstra-va-ung-dung-aWj53zgQl6m)
      - [ Thuật toán Bellman Ford và ứng dụng ](https://viblo.asia/p/thuat-toan-bellman-ford-va-ung-dung-aWj53zxwl6m)

## Giải thuật

### Thuật toán sắp xếp

Ta sẽ tập trung học sắp xếp dựa trên so sánh (Comparison-based sorting. Bao gồm: Bubble Sort, Selection Sort, Insertion Sort, Merge Sort, Heap Sort, Quick Sort) và sắp xếp không dựa trên so sánh (Non-comparison based sorting. Bao gồm Counting Sort, Radix Sort).

  - Bubble Sort
      - [Thuật toán sắp xếp nổi bọt (bubble sort) ](https://viblo.asia/p/thuat-toan-sap-xep-noi-bot-bubble-sort-m68Z0exQlkG)
      - Video [ Bubble Sort Algorithm | Thuật toán sắp xếp Bubble ](https://www.youtube.com/watch?v=KsbdeXLau08&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=43)
  - Selection Sort
      - Bài đọc: [ Thuật Toán Selection Sort Đơn Giản ](https://viblo.asia/p/thuat-toan-selection-sort-don-gian-3Q75wVBelWb)
      - Video: [ Thuật Toán Sắp Xếp Chọn (Selection Sort)](https://www.youtube.com/watch?v=efJr9woV-74)
  - Insertion Sort
      - Bài đọc: [ Thuật Toán Insertion Sort Đơn Giản ](https://viblo.asia/p/thuat-toan-insertion-sort-don-gian-bWrZnVapZxw)
      - Video: [ Insertion Sort Algorithm | Thuật toán sắp xếp chèn ](https://www.youtube.com/watch?v=IWT-Uoz_Sb8&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=43)
  - Merge Sort
      - Bài đọc: [ Merge Sort ](https://viblo.asia/p/merge-sort-38X4ENAoJN2)
      - Video:
          - [ Merge Sort Algorithm \#1: Giới thiệu CONCEPT | Thuật toán sắp xếp "theo dân gian là Trộn @@" ](https://www.youtube.com/watch?v=f2nTwlZiuMI&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=45)
          - [ Merge Sort Algorithm \#2: Đời HỢP rồi TAN | Thuật toán sắp xếp "theo dân gian là Trộn @@" ](https://www.youtube.com/watch?v=Pq5y-MzBdWs&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=46)
  - Heap Sort
      - Bài đọc: [ Sắp xếp vun đống ](https://viblo.asia/p/sap-xep-vun-dong-63vKjeYk52R)
      - Video: [ Heap Sort Algorithm | Thuật toán sắp xếp vun đống @@ ](https://www.youtube.com/watch?v=Dr6DdLDsE-4&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=48)
  - Quicksort
      - Bài đọc: [ Thuật toán sắp xếp nhanh (Quick sort) ](https://viblo.asia/p/thuat-toan-sap-xep-nhanh-quick-sort-eW65G6ROlDO)
      - Video: [ Quick Sort Algorithm | Thuật toán sắp xếp nhanh ](https://www.youtube.com/watch?v=x1BMc7MEjnk&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=44)
  - Counting Sort
      - Bài đọc: [Sắp xếp bằng đếm phân phối (Counting Sort) ](https://viblo.asia/p/sap-xep-bang-dem-phan-phoi-counting-sort-Qbq5Q63LKD8)
      - Video: [ [Bài 4] Đếm Phân phối | Counting sort ](https://www.youtube.com/watch?v=Z8bXkmxEXlI)
  - Radix Sort
      - Bài đọc: [ Tìm hiểu về Radix sort và cách implement thuật toán này trong Swift ](https://viblo.asia/p/tim-hieu-ve-radix-sort-va-cach-implement-thuat-toan-nay-trong-swift-E375zk0PKGW)
      - Video: [ Radix Sort Algorithm | Thuật toán sắp xếp theo cơ số ](https://www.youtube.com/watch?v=e4Oide9BsH8&list=PLoaAbmGPgTSNMAzkKBHkh2mLuBk54II5L&index=50) - Video

Đọc thêm:

  - [So sánh các thuật toán sắp xếp](https://viblo.asia/p/so-sanh-cac-thuat-toan-sap-xep-YWOZrAyyKQ0)
  - [Tản mạn về các thuật toán Sorting](https://viblo.asia/p/tan-man-ve-cac-thuat-toan-sorting-gDVK2o0AZLj)

### Thuật toán tìm kiếm

  - Linear Search: [Thuật toán tìm kiếm tuyến tính (Linear Search) trong C++](https://www.google.com/search?q=https://viblo.asia/p/thuat-toan-tim-kiem-tuyen-tinh-linear-search-trong-c-YbJlXJ7elWj)
  - Binary Search: [Thuật toán tìm kiếm nhị phân (Binary Search)](https://www.google.com/search?q=https://viblo.asia/p/thuat-toan-tim-kiem-nhi-phan-binary-search-Eb85oVy6l2G)
  - Interpolation Search: [Tìm kiếm nội suy (Interpolation Search)](https://www.google.com/search?q=https://freetuts.net/tim-kiem-noi-suy-interpolation-search-2840.html)
  - Các thuật toán tìm kiếm nâng cao (Ternary Search, Exponential Search):
      - **Ternary Search:** [Tìm kiếm tam phân (Ternary Search)](https://www.google.com/search?q=https://freetuts.net/tim-kiem-tam-phan-ternary-search-2841.html)
      - **Exponential Search:** [Exponential Search](https://www.google.com/url?sa=E&source=gmail&q=https://www.geeksforgeeks.org/exponential-search/) (Bài viết tiếng Anh, bạn có thể tìm thêm tài liệu tiếng Việt nếu cần)

### Advanced Graph Algorithms:

  - Topological Sort: [Thuật toán sắp xếp Topo (Topological Sort)](https://www.google.com/search?q=https://viblo.asia/p/thuat-toan-sap-xep-topo-topological-sort-dje5Vj99lWj)
  - Strongly Connected Components (Tarjan's algorithm): [Thuật toán Tarjan tìm các thành phần liên thông mạnh](https://www.google.com/search?q=https://vnoi.info/wiki/algo/graph/tarjan-scc)
  - Maximum Flow (Ford-Fulkerson algorithm): [Bài toán luồng cực đại và thuật toán Ford-Fulkerson](https://www.google.com/search?q=https://vnoi.info/wiki/algo/graph/max-flow)

### Dynamic Programming:

  - Memoization and tabulation: [Memoization và Tabulation trong Dynamic Programming](https://www.google.com/search?q=https://viblo.asia/p/memoization-va-tabulation-trong-dynamic-programming-naQjzvYkZWA)
  - Solving problems using dynamic programming (Knapsack problem, Longest Common Subsequence, Matrix Chain Multiplication)
  - [Tất cả những gì bạn cần là quy hoạch động](https://viblo.asia/p/tat-ca-nhung-gi-ban-can-la-quy-hoach-dong-jvElaqVDlkw)

<!-- end list -->

3.  Backtracking:

<!-- end list -->

  - Solving constraint satisfaction problems (N-Queens, Sudoku, Subset Sum)
  - Pruning the search space
  - **Backtracking:** [Thuật toán Backtracking (quay lui) và ứng dụng](https://www.google.com/search?q=https://viblo.asia/p/thuat-toan-backtracking-quay-lui-va-ung-dung-naQjzvYkZWA)

<!-- end list -->

4.  Greedy Algorithms:

<!-- end list -->

  - Activity Selection Problem, Huffman Coding, Fractional Knapsack Problem
  - **Greedy Algorithms:** [Thuật toán tham lam (Greedy Algorithm)](https://www.google.com/search?q=https://viblo.asia/p/thuat-toan-tham-lam-greedy-algorithm-naQjzvYkZWA)

### Tài nguyên

Theo như một bình luận trên Reddit thì:

> So there are some that try to advocate for standardizing pseudocode, but personally I think it's a terrible idea. If the code doesn't actually run, how can you be sure it's unambiguous and correct? There are famous examples of pseudocode in textbooks and papers having subtle bugs in them.

Nên có thêm một số phần mềm hỗ trợ trực quan hóa thuật toán, hai công cụ mà mình khá thích là:

- [https://tobinatore.github.io/algovis/](https://tobinatore.github.io/algovis/)
- [https://www.cs.usfca.edu/\~galles/visualization/Algorithms.html](https://www.cs.usfca.edu/~galles/visualization/Algorithms.html)
- [https://tira.mooc.fi/spring-2025/chap16/](https://tira.mooc.fi/spring-2025/chap16/)

