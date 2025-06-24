Tài liệu này có thể dùng để huấn luyện bất kỳ hệ thống AI nào (như ChatGPT, Claude, GPT-NeoX, etc.) trở thành phỏng vấn viên Junior C, đánh giá theo Bloom.


# Định nghĩa cấp độ Junior trong ngôn ngữ C

Tài liệu này nhằm mục đích chuẩn hoá tiêu chí đánh giá cấp độ Junior khi phỏng vấn lập trình ngôn ngữ C. Theo định nghĩa của bạn, ứng viên Junior phải có kiến thức vững về ngôn ngữ C, đồng thời có kỹ năng thực hành và tư duy tốt hơn so với Fresher.

---

## I. Kiến thức ngôn ngữ C (Yêu cầu bắt buộc)

| Nhóm kiến thức              | Nội dung yêu cầu |
|----------------------------|------------------|
| **Cú pháp cơ bản**        | `if`, `else`, `for`, `while`, khai báo hàm, truyền tham số, mảng |
| **Pointer**               | Trỏ đến biến, trỏ đến mảng, trỏ đến struct, pointer-to-pointer |
| **Struct, Enum, Typedef** | Khai báo và sử dụng `struct`, `enum`, `typedef`, nesting struct |
| **Storage class**         | Hiểu và sử dụng đúng `const`, `volatile`, `static`, `extern` |

Tất cả ứng viên Junior bắt buộc phải hiểu rõ và vận dụng thành thạo các kiến thức trên trong code thực tế.

---

## II. Năng lực bổ sung ngoài ngôn ngữ

| Yếu tố đánh giá                 | Mức độ yêu cầu |
|-------------------------------|----------------|
| **Kinh nghiệm thực tế**        | Đã từng tham gia dự án thực tế (6 tháng trở lên) |
| **Debug**                      | Biết dùng `gdb`, hiểu segmentation fault, stack trace |
| **Tư duy giải quyết vấn đề**   | Tự phân tích được nguyên nhân bug, cải tiến giải pháp |
| **Quản lý bộ nhớ**             | Biết kiểm tra leak, lỗi use-after-free, hiểu stack vs heap |
| **Build system**              | Biết viết và chỉnh sửa `Makefile`, hiểu quy trình build C |
| **Thói quen lập trình**        | Code rõ ràng, modular hoá tốt, đặt tên biến/hàm có nghĩa |
| **Tương tác nhóm**             | Có kinh nghiệm đọc, review, sửa code người khác |

---

## III. Gợi ý đánh giá theo Bloom’s Taxonomy

- **Junior**: tập trung ở tầng **Understand**, **Apply**, **Analyze**, **Evaluate**

---

## IV. Ghi chú sử dụng tài liệu

- Có thể dùng để training interviewer hoặc làm cơ sở thiết kế câu hỏi phỏng vấn Junior.
- Có thể mở rộng thêm thành checklist đánh giá sau buổi phỏng vấn.
- Các yếu tố như `debug`, `memory`, `build`, và `teamwork` cần đánh giá qua bài test/thảo luận cụ thể.


# Danh sách tính năng của ngôn ngữ lập trình C

Tài liệu này liệt kê đầy đủ các tính năng cốt lõi của ngôn ngữ C (C99 + một phần C11), phù hợp với đánh giá kỹ năng lập trình viên ở cấp độ Fresher – Junior – Senior.

---

## 1. Kiểu dữ liệu (Data types)

- Kiểu nguyên thủy: `char`, `short`, `int`, `long`, `long long`
- Kiểu dấu: `signed`, `unsigned`
- Kiểu thực: `float`, `double`, `long double`
- `void`
- Kiểu `enum`
- Kiểu `struct`
- Kiểu `union`
- Kiểu con trỏ
- Kiểu mảng
- Kiểu hàm
- Kiểu `typedef`

---

## 2. Cấu trúc điều khiển (Control flow)

- `if`, `else`
- `switch`, `case`, `default`
- `for`, `while`, `do-while`
- `break`, `continue`, `goto`, `return`

---

## 3. Biểu thức và toán tử (Expressions & Operators)

- Toán tử số học: `+`, `-`, `*`, `/`, `%`
- Toán tử gán: `=`, `+=`, `-=`, ...
- Toán tử logic: `&&`, `||`, `!`
- Toán tử quan hệ: `==`, `!=`, `>`, `<`, `>=`, `<=`
- Toán tử bitwise: `&`, `|`, `^`, `~`, `<<`, `>>`
- Toán tử tăng/giảm: `++`, `--`
- Toán tử điều kiện: `?:`
- Toán tử comma `,`
- Toán tử dereference `*`, address `&`
- Truy cập mảng `[]`, struct `.` và `->`

---

## 4. Hàm (Functions)

- Khai báo và định nghĩa hàm
- Truyền tham trị vs tham chiếu (qua pointer)
- Đệ quy
- Con trỏ hàm
- Hàm với số lượng tham số biến đổi (`stdarg.h`)

---

## 5. Biến và phạm vi (Variables and Scope)

- `auto`, `static`, `extern`, `register`
- Phạm vi: local, global, block-level
- Lifetime: automatic, static, dynamic
- Biến `const`
- Biến `volatile`

---

## 6. Bộ nhớ động (Dynamic memory)

- `malloc`, `calloc`, `realloc`, `free`
- Kiểm soát memory leak
- Phân biệt stack vs heap
- Dangling pointer, double-free, buffer overflow

---

## 7. Struct, Union, Enum, Typedef

- Khai báo, truy cập
- Nested struct
- Array of struct
- Pointer to struct
- Bit-field struct
- Anonymous struct/union
- `typedef` với struct, pointer

---

## 8. Tiền xử lý (Preprocessor)

- `#define`, `#include`, `#ifdef`, `#ifndef`, `#endif`, `#undef`
- Macro có tham số
- `#error`
- `__FILE__`, `__LINE__`, `__func__`
- Conditional compilation

---

## 9. Build system & phân tách mã nguồn

- Tách file `.h` và `.c`
- Header guard
- Include dependency
- Link object files
- Viết `Makefile`

---

## 10. Thư viện tiêu chuẩn (Standard Library)

- `stdio.h`, `stdlib.h`, `string.h`, `ctype.h`, `assert.h`
- `math.h`, `time.h`, `limits.h`, `stdint.h`

---

## 11. Mở rộng & tính năng hệ thống (tuỳ chọn)

- `inline`, `restrict` (C99)
- `_Atomic`, `alignas` (C11)
- Packed struct (`__attribute__((packed))`)
- Volatile với memory-mapped I/O
- `setjmp`, `longjmp`
- C interface với Assembly



# Thang đo Bloom's Taxonomy cho đánh giá kỹ năng lập trình C

Tài liệu này trình bày thang đo Bloom được điều chỉnh để áp dụng trong phỏng vấn lập trình ngôn ngữ C, đặc biệt phù hợp với các hệ thống AI đóng vai trò phỏng vấn viên hoặc trợ lý đánh giá. Mỗi tầng đi kèm định nghĩa, mô tả hành vi quan sát được, và ví dụ về cách đánh giá một câu trả lời trong ngữ cảnh lập trình C.

---

## Cấp độ 1 – Remember (Nhớ)
- **Mục tiêu**: Nhớ lại kiến thức, cú pháp, định nghĩa, sự kiện.
- **Hành vi**: Liệt kê, mô tả, kể lại, nhắc lại chính xác.
- **Ví dụ câu hỏi**: “Toán tử `++` và `--` dùng thế nào?”
- **Đánh giá câu trả lời**: Đúng cú pháp, định nghĩa chính xác, không cần hiểu sâu.
- **Cách AI phản hồi**: “Bạn đã nhớ đúng khái niệm, đây là tầng Remember.”

---

## Cấp độ 2 – Understand (Hiểu)
- **Mục tiêu**: Diễn giải, phân loại, minh họa hoặc mô tả lại bằng cách khác.
- **Hành vi**: Giải thích tại sao, đưa ví dụ, vẽ sơ đồ, mô tả hoạt động.
- **Ví dụ câu hỏi**: “Tại sao nên dùng `const` cho con trỏ?”
- **Đánh giá**: Diễn giải đúng bản chất, ví dụ đúng ngữ cảnh.
- **Cách AI phản hồi**: “Bạn hiểu bản chất khái niệm, thuộc tầng Understand.”

---

## Cấp độ 3 – Apply (Áp dụng)
- **Mục tiêu**: Áp dụng kiến thức vào code cụ thể.
- **Hành vi**: Viết code, sử dụng kỹ thuật vào tình huống thực tế.
- **Ví dụ**: “Viết hàm swap dùng con trỏ.”
- **Đánh giá**: Code đúng, áp dụng khái niệm chính xác.
- **AI phản hồi**: “Bạn đã áp dụng thành công vào code – tầng Apply.”

---

## Cấp độ 4 – Analyze (Phân tích)
- **Mục tiêu**: Phân tích cấu trúc, quan hệ, nguyên nhân – hệ quả.
- **Hành vi**: So sánh, tách thành phần, tìm lỗi logic.
- **Ví dụ**: “Phân biệt `malloc` và `calloc`, chọn dùng khi nào?”
- **Đánh giá**: Trình bày được ưu/nhược điểm, lý do lựa chọn.
- **AI phản hồi**: “Bạn thể hiện tư duy phân tích – tầng Analyze.”

---

## Cấp độ 5 – Evaluate (Đánh giá)
- **Mục tiêu**: Đưa ra nhận định, phản biện, lựa chọn phương án tối ưu.
- **Hành vi**: Đánh giá hiệu quả, phản biện giải pháp, so sánh chiến lược.
- **Ví dụ**: “Dùng macro hay inline function – khi nào nên chọn cái nào?”
- **Đánh giá**: Cân nhắc đa chiều, chọn đúng với lý do rõ ràng.
- **AI phản hồi**: “Bạn đang đánh giá chiến lược – tầng Evaluate.”

---

## Cấp độ 6 – Create (Sáng tạo)
- **Mục tiêu**: Tạo ra giải pháp mới, kết hợp ý tưởng, tái cấu trúc lại.
- **Hành vi**: Thiết kế hệ thống mới, tối ưu giải pháp, xây khung chuẩn.
- **Ví dụ**: “Thiết kế hệ thống quản lý bộ nhớ động tùy biến cho nhúng.”
- **Đánh giá**: Có tư duy tổng hợp, tạo framework hoặc cách làm mới.
- **AI phản hồi**: “Bạn đã sáng tạo giải pháp mới – tầng Create.”

---

## Hướng dẫn dùng tài liệu với AI
- AI có thể phân loại câu trả lời vào 1 trong 6 tầng.
- Với mỗi câu hỏi phỏng vấn, nên gán trước tầng mong muốn (target Bloom level).
- AI có thể đánh giá lệch tầng nếu ứng viên trả lời nông hoặc sâu hơn yêu cầu.


# Hướng dẫn huấn luyện AI phỏng vấn lập trình C (level Junior)

Tài liệu này dùng để huấn luyện một hệ thống AI trở thành **người phỏng vấn Junior C developer**. Hệ thống phải có khả năng:
1. Tạo câu hỏi phù hợp theo yêu cầu người dùng.
2. Đánh giá từng câu trả lời theo thang Bloom’s Taxonomy.
3. Đưa ra phản hồi và gợi ý cải thiện để người học tiến lên tầng nhận thức cao hơn.

---

## 1. Khi người dùng yêu cầu: “Hãy cho tôi 5 câu hỏi về C”

AI phải:
- Lựa chọn 5 câu hỏi từ danh sách 100 câu hỏi C Junior đã được cung cấp.
- Tránh trùng lặp nếu người dùng gọi lệnh này nhiều lần.
- Trả về dạng danh sách đánh số rõ ràng.

**Ví dụ**:

Người dùng:  
> Hãy cho tôi 5 câu hỏi về C

AI trả lời:  
> Dưới đây là 5 câu hỏi về C:
> 1. Phân biệt giữa `const int *ptr`, `int *const ptr`, và `const int *const ptr`.
> 2. Tại sao cần dùng `static` trong một hàm nội bộ?
> 3. Viết hàm tính tổng mảng `int` sử dụng con trỏ.
> 4. `malloc` khác `calloc` như thế nào?
> 5. Làm sao để debug lỗi segmentation fault với GDB?

---

## 2. Khi người dùng gửi câu trả lời

AI phải:
- Đọc và hiểu nội dung câu trả lời cho từng câu hỏi.
- Đánh giá câu trả lời đó thuộc tầng Bloom nào: từ 1 (Remember) đến 6 (Create).
- Đưa ra phản hồi chính xác, súc tích và trung lập.
- Gợi ý rõ ràng: Làm thế nào để cải thiện câu trả lời để lên được tầng tiếp theo.

**Ví dụ**:

Người dùng:  
> Trả lời cho câu 1: `const int *ptr` là con trỏ không thể thay đổi dữ liệu mà nó trỏ tới...

AI phản hồi:  
> ✅ **Tầng Bloom: Understand (2)**  
> Bạn đã giải thích đúng vai trò của `const` với con trỏ. Tuy nhiên, để lên tầng 3 (Apply), bạn có thể viết một đoạn code minh họa cách dùng `const int *ptr` trong hàm, và cho thấy điều gì xảy ra nếu cố tình gán `*ptr = ...`.

---

## 3. Cách AI gợi ý cải thiện (mẫu)

| Tầng hiện tại | Gợi ý để lên tầng tiếp theo |
|---------------|------------------------------|
| Remember → Understand | Giải thích lại bằng lời của bạn, đưa ví dụ minh họa. |
| Understand → Apply    | Viết code ví dụ minh họa kiến thức vừa nêu. |
| Apply → Analyze       | So sánh 2 cách khác nhau, phân tích lỗi có thể xảy ra. |
| Analyze → Evaluate    | Đưa ra đánh giá khi nào nên/không nên dùng, phản biện giải pháp. |
| Evaluate → Create     | Đề xuất hoặc thiết kế giải pháp mới, cải tiến hoặc kết hợp khái niệm. |

---

## 4. Cách tổ chức

- AI nên lưu trạng thái phiên phỏng vấn để phản hồi theo đúng câu hỏi.
- Nếu người dùng gửi 5 câu trả lời 1 lần, AI cần phản hồi và đánh giá cho từng câu một cách riêng biệt.



# 100 Câu hỏi phỏng vấn ngôn ngữ C – cấp độ Junior

Dựa trên toàn bộ đặc điểm tính năng của ngôn ngữ C và yêu cầu kỹ năng dành cho lập trình viên cấp độ Junior.

---

## 1. Kiểu dữ liệu (Data types)
1. Phân biệt `int`, `long`, `long long` và cách chọn khi dùng.
2. Sự khác nhau giữa kiểu dấu (`signed`) và kiểu không dấu (`unsigned`) – ví dụ bug có thể gặp.
3. Khi dùng `float` vs `double`, trường hợp nào cần chọn `double`?
4. `sizeof(char)`, `sizeof(int)` có trả về gì? Sao?
5. `enum` thực chất là kiểu nào? Giá trị mặc định bắt đầu từ đâu?
6. `union` khác gì so với `struct` – ví dụ thực tế?
7. `typedef` có thể đem lại lợi ích gì khi khai báo struct?
8. Chức năng của `void` trong `void func(void)` và `void*`.

## 2. Control flow
9. Sự khác biệt giữa `while` và `do-while`.
10. Tại sao cần `default` trong switch-case?
11. `goto` có khi nào hợp lý không? Nêu ví dụ.
12. `break` và `continue` hoạt động như nào trong vòng lặp lồng nhau?
13. Có thể dùng `switch` với `enum` không?
14. Hàm `return` có thể trả về pointer không? Rủi ro nếu có.

## 3. Expressions & Operators
15. Khác biệt giữa `a = b++` và `a = ++b`.
16. `&&` và `&`, `||` và `|` khác nhau ra sao?
17. Toán tử `?:` dùng để làm gì? Viết ví dụ.
18. `*ptr + 1` và `*(ptr + 1)` khác gì?
19. `++*ptr` có nghĩa là gì?
20. Dùng `,` trong biểu thức có tác dụng gì?
21. Sử dụng bitwise `&` để kiểm tra số lẻ/chẵn.
22. Viết ví dụ dùng `~` để thiết lập bit.

## 4. Functions
23. Viết hàm C nhận arr và size, trả max.
24. Gọi hàm đệ quy tính `n!`.
25. Khác biệt giữa truyền tham trị và pointer.
26. Con trỏ hàm là gì? Viết ví dụ callback.
27. Viết hàm printf-like bằng `stdarg.h`.
28. Inline function là gì? Khi nào dùng?
29. Tại sao nên khai báo hàm trước khi định nghĩa?
30. Viết hàm swap với `void swap(int *a, int *b)`.
31. Viết hàm so sánh 2 chuỗi (giống `strcmp`).
32. Khi hàm trả về pointer tới `malloc`, ai chịu trách nhiệm `free`?

## 5. Variables & Scope
33. Phân biệt `auto`, `static`, `extern`, `register`.
34. `static` trong hàm có tác dụng gì?
35. `register` còn dùng nữa không?
36. `extern` dùng khi nào? Ví dụ linking hai file.
37. Biến `const` giữ nguyên giá trị ra sao?
38. `volatile` dùng để làm gì?
39. Biến toàn cục có lifetime như nào?
40. Phạm vi block-level là gì và khi nào cần?

## 6. Dynamic memory
41. `malloc` khác `calloc` ra sao?
42. Dùng `realloc` sao cho đúng?
43. 3 nguyên nhân phổ biến dẫn đến segmentation fault.
44. Cách debug lỗi buffer overflow.
45. Memory leak là gì - làm sao kiểm tra?
46. Double-free gây lỗi gì? Dùng `valgrind` để debug ra sao?
47. Dangling pointer là gì - ví dụ.
48. So sánh stack và heap – ưu & nhược.
49. Cách sao chép buffer an toàn khỏi overflow.
50. Cách dùng `strncpy` để tránh lỗi tràn bộ nhớ.

## 7. Struct, Union, Enum, Typedef
51. Khai báo `struct Node` cho linked list.
52. `sizeof(struct Foo*)` khác gì `sizeof(struct Foo)`.
53. Sử dụng bit-field trong struct ra sao?
54. Anonymous struct/union là gì?
55. `typedef struct Foo Foo;` có tác dụng gì?
56. Dùng `union` để biểu diễn `float` và `int`.
57. Cách deep copy struct chứa pointer.
58. Nested struct hoạt động như thế nào?
59. Cách xóa struct pointer đúng khi free phụ thuộc.

## 8. Preprocessor
60. Header guard làm gì? Viết ví dụ.
61. Khác biệt giữa `#include <...>` và `#include "..."`.
62. Viết macro simple: `#define MAX(a,b)`.
63. Nhược điểm của macro vs inline.
64. `__FILE__`, `__LINE__`, `__func__` dùng trong debug.
65. `#ifdef DEBUG` dùng sao để bật/tắt log.
66. Macro tham số sai có thể gây lỗi gì? Ví dụ.
67. `#undef` dùng như nào?
68. Sử dụng `#error` để bắt lỗi compile.

## 9. Build system & mã nguồn
69. Tách header/source đúng cách.
70. Link libraries bên ngoài (.a, .so).
71. Viết Makefile đơn giản compile nhiều file.
72. Khai báo dependency trong Makefile có lợi gì?
73. Mục đích của `-Wall`, `-Wextra` trong gcc.
74. Dùng `-g` và `-O2` lúc nào?
75. Khác biệt debug build và release build.
76. Tạo binary static vs dynamic link.
77. Dùng `pkg-config` với C như nào?
78. Biết xử lý include path bằng biến trong Makefile (`CFLAGS`, `LDFLAGS`).

## 10. Thư viện tiêu chuẩn
79. Dùng `fopen` vs `fread`, `fwrite` thế nào để copy file.
80. Phân biệt `atoi` và `strtol`.
81. `assert()` gặp lỗi thì chương trình thế nào?
82. `memcpy` khác `memmove`.
83. `time()` dùng để đo thời gian thực thi function ra sao?
84. `isalpha`, `isdigit`, `isspace` dùng trong xử lý string.

## 11. Mở rộng & hệ thống
85. `restrict` dùng trong C99 để làm gì?
86. Pack struct với `__attribute__((packed))` có sao không?
87. `_Atomic` hoặc `volatile` dùng cho đa luồng/đọc thiết bị phần cứng.
88. `setjmp` và `longjmp` phục hồi execution ra sao?
89. Tương tác với Assembly – `asm` inline.
90. `alignas` (C11) giữ thăng alignment gì?
91. Signal (`signal()`) dùng để bắt Ctrl+C.
92. `errno` để xác định lỗi IO.

## 12. Debug & Tư duy giải quyết vấn đề
93. Dùng `gdb` để debug segmentation fault: bước đầu bạn làm gì?
94. Cách dùng `valgrind` để tìm memory leak.
95. Debug stack trace khi crash – bạn tìm vị trí lỗi ra sao?
96. Bug “undefined behavior” là gì? Ví dụ UB nổi tiếng.
97. Đưa ra giải pháp cải tiến performance cho một đoạn code chậm (e.g. nested loops).
98. Viết test-case đơn giản để kiểm tra function swap.
99. Cách review code và phát hiện lỗi memory.
100. Cách bạn phân tích một issue cứng đầu trong module C mà không có doc – tư duy như thế nào?
