<p align="center"><img src="/images/logo.png" alt=""></p>
<h1 align="center">What the f*ck Python! 😱</h1>
<p align="center">Cùng khám phá và tìm hiểu Python thông qua các đoạn mã khiến bạn bất ngờ.</p>


Các bản dịch tiếng nước ngoài khác: [Tiếng Trung 中文](https://github.com/leisurelicht/wtfpython-cn) | [Thêm bản dịch](https://github.com/satwikkansal/wtfpython/issues/new?title=Add%20translation%20for%20[LANGUAGE]&body=Expected%20time%20to%20finish:%20[X]%20weeks.%20I%27ll%20start%20working%20on%20it%20from%20[Y].)

Bạn có thể tham khảo các đoạn mã với: [Chế độ trực quan](https://colab.research.google.com/github/satwikkansal/wtfpython/blob/master/irrelevant/wtf.ipynb) | [Giao diện dòng lệnh](https://pypi.python.org/pypi/wtfpython)


Python là một ngôn ngữ cấp cao, với các mã được thông dịch thay vì biên dịch như các ngôn ngữ khác như C hay Java. Python có rất nhiều các tính năng giúp việc lập trình dễ dàng, thuận tiện. Tuy nhiên, các đoạn mã viết bằng Python thỉnh thoảng cho ra kết quả không rõ ràng, gây khó hiểu khi mới nhìn vào.


wtfpython được tạo ra với mong muốn giải thích chính xác cách hoạt động của các đoạn mã thoạt nhìn khó hiểu và các tính năng ít được biết tới trong Python.


Một vài ví dụ có thể không làm bạn quá ngạc nhiên, tuy vậy bạn sẽ khám phá được những điều hay ho về Python mà có thể bạn chưa từng biết tới. Học lập trình thông qua những ví dụ như vậy giúp bạn hiểu sâu hơn những thứ nằm bên trong của một ngôn ngữ lập trình, khi đó bạn sẽ thấy hứng thú hơn trong quá trình học.


Nếu độc giả là một lập trình viên có thâm niên, hãy thử thức mình với các đoạn mã sắp tới, cố gắng làm đúng mỗi thử thách ngay trong lần đầu tiên. Độc giả có thể đã thử quả một vài trong số các bài toán trước đó, đọc và làm các bài toán dưới đây có thể giúp bạn ôn lại chúng.


PS: Nếu bạn đã đọc bài này trước đó, bạn có thể muốn xem những thay đổi mới [ở đây](https://github.com/satwikkansal/wtfpython/releases/).



Nào ta bắt đầu ...

# Những nội dung chính
<!-- Generated using "markdown-toc -i README.md --maxdepth 3"-->

<!-- toc -->

- [Cấu trúc của các ví dụ](#structure-of-the-examples)
    + [▶ Some fancy Title](#-some-fancy-title)
- [Cách sử dụng](#usage)
- [👀 Các ví dụ](#-examples)
  * [Section: Strain your brain!](#section-strain-your-brain)
    + [▶ First things first! *](#-first-things-first-)
    + [▶ Strings can be tricky sometimes](#-strings-can-be-tricky-sometimes)
    + [▶ Be careful with chained operations](#-be-careful-with-chained-operations)
    + [▶ How not to use `is` operator](#-how-not-to-use-is-operator)
    + [▶ Hash brownies](#-hash-brownies)
    + [▶ Deep down, we're all the same.](#-deep-down-were-all-the-same)
    + [▶ Disorder within order *](#-disorder-within-order-)
    + [▶ Keep trying... *](#-keep-trying-)
    + [▶ For what?](#-for-what)
    + [▶ Evaluation time discrepancy](#-evaluation-time-discrepancy)
    + [▶ `is not ...` is not `is (not ...)`](#-is-not--is-not-is-not-)
    + [▶ A tic-tac-toe where X wins in the first attempt!](#-a-tic-tac-toe-where-x-wins-in-the-first-attempt)
    + [▶ The sticky output function](#-the-sticky-output-function)
    + [▶ The chicken-egg problem *](#-the-chicken-egg-problem-)
    + [▶ Subclass relationships](#-subclass-relationships)
    + [▶ All-true-ation *](#-all-true-ation-)
    + [▶ The surprising comma](#-the-surprising-comma)
    + [▶ Strings and the backslashes](#-strings-and-the-backslashes)
    + [▶ not knot!](#-not-knot)
    + [▶ Half triple-quoted strings](#-half-triple-quoted-strings)
    + [▶ What's wrong with booleans?](#-whats-wrong-with-booleans)
    + [▶ Class attributes and instance attributes](#-class-attributes-and-instance-attributes)
    + [▶ Non-reflexive class method *](#-non-reflexive-class-method-)
    + [▶ yielding None](#-yielding-none)
    + [▶ Yielding from... return! *](#-yielding-from-return-)
    + [▶ Nan-reflexivity *](#-nan-reflexivity-)
    + [▶ Mutating the immutable!](#-mutating-the-immutable)
    + [▶ The disappearing variable from outer scope](#-the-disappearing-variable-from-outer-scope)
    + [▶ The mysterious key type conversion](#-the-mysterious-key-type-conversion)
    + [▶ Let's see if you can guess this?](#-lets-see-if-you-can-guess-this)
  * [Section: Slippery Slopes](#section-slippery-slopes)
    + [▶ Modifying a dictionary while iterating over it](#-modifying-a-dictionary-while-iterating-over-it)
    + [▶ Stubborn `del` operation](#-stubborn-del-operation)
    + [▶ The out of scope variable](#-the-out-of-scope-variable)
    + [▶ Deleting a list item while iterating](#-deleting-a-list-item-while-iterating)
    + [▶ Lossy zip of iterators *](#-lossy-zip-of-iterators-)
    + [▶ Loop variables leaking out!](#-loop-variables-leaking-out)
    + [▶ Beware of default mutable arguments!](#-beware-of-default-mutable-arguments)
    + [▶ Catching the Exceptions](#-catching-the-exceptions)
    + [▶ Same operands, different story!](#-same-operands-different-story)
    + [▶ Name resolution ignoring class scope](#-name-resolution-ignoring-class-scope)
    + [▶ Needles in a Haystack *](#-needles-in-a-haystack-)
    + [▶ Splitsies *](#-splitsies-)
    + [▶ Wild imports *](#-wild-imports-)
    + [▶ All sorted? *](#-all-sorted-)
    + [▶ Midnight time doesn't exist?](#-midnight-time-doesnt-exist)
  * [Section: The Hidden treasures!](#section-the-hidden-treasures)
    + [▶ Okay Python, Can you make me fly?](#-okay-python-can-you-make-me-fly)
    + [▶ `goto`, but why?](#-goto-but-why)
    + [▶ Brace yourself!](#-brace-yourself)
    + [▶ Let's meet Friendly Language Uncle For Life](#-lets-meet-friendly-language-uncle-for-life)
    + [▶ Even Python understands that love is complicated](#-even-python-understands-that-love-is-complicated)
    + [▶ Yes, it exists!](#-yes-it-exists)
    + [▶ Ellipsis *](#-ellipsis-)
    + [▶ Inpinity](#-inpinity)
    + [▶ Let's mangle](#-lets-mangle)
  * [Section: Appearances are deceptive!](#section-appearances-are-deceptive)
    + [▶ Skipping lines?](#-skipping-lines)
    + [▶ Teleportation](#-teleportation)
    + [▶ Well, something is fishy...](#-well-something-is-fishy)
  * [Section: Miscellaneous](#section-miscellaneous)
    + [▶ `+=` is faster](#--is-faster)
    + [▶ Let's make a giant string!](#-lets-make-a-giant-string)
    + [▶ Minor Ones *](#-minor-ones-)
- [Contributing](#contributing)
- [Acknowledgements](#acknowledgements)
- [🎓 License](#-license)
  * [Surprise your friends as well!](#surprise-your-friends-as-well)
  * [More content like this?](#more-content-like-this)

<!-- tocstop -->

# Cấu trúc của các ví dụ

Tất cả các các ví dụ được trình bày với cấu trúc như sau:
> ### ▶ Một tiêu đề hấp dẫn
>
> ```py
> # Đoạn mã tạo dựng ví dụ.
> # Đoạn mã chủ thể cần khám phá...
> ```
>
> **Kết quả (Các phiên bản Python):**
>
> ```py
> >>> câu lệnh kích hoạt?
> Một vài kết quả bất ngờ, không như mong đợi
> ```
> (Có thể có hay không): Một dòng mô tả kết quả
>
>
> #### 💡 Giải thích:
>
> * Giải thích những điều đang diễn ra và tại sao.
> ```py
> # Đoạn mã tạo dựng ví dụ
> # Trong trường hợp cần thiết, chúng tôi liệt kê thêm nhiều ví dụ khác để giúp bạn hiểu rõ hơn
> ```
> **Kết quả (Các phiên bản Python):**
>
> ```py
> >>> trigger # some example that makes it easy to unveil the magic
> >>> trigger # Một vài ví dụ giúp bạn hiểu các đoạn mã
> # some justified output
> ```

**Lưu ý:** Tất cả các ví dụ đã được chứng minh chạy thành công trên trình thông dịch Python 3.5.2 chế độ tương tác, với các phiên bản Python khác các ví dụ sẽ vẫn chạy bình thường, ngoại trừ một số ví dụ chúng tôi sẽ lưu ý trước phần kết quả.
# Cách dùng các ví dụ

Theo tôi, để học các ví dụ trong bài, bạn nên đọc theo trình tự thời gian, và đối với mỗi ví dụ hãy:
- Đọc kĩ đoạn mã tạo dựng nên ví dụ. Nếu bạn đã lập trình lâu rồi, bạn sẽ đoán được những điều sắp tới ngay.
- Đọc kết quả của các ví dụ và thực hiện hai việc sau:
  + Kiểm tra xem kết quả có giống như bạn nghĩ hay không.
  + Một khi đọc xong, hãy hỏi chính bạn xem mình đã hiểu thông suốt lý do mà có kết quả như vậy chưa.
    - Nếu câu trả lời là "chưa, tôi chưa hiểu" (không sao cả), hít một hơi thật sau, và đọc phần giải thích (nếu bạn vẫn chưa hiểu, hãy tạo một issue [ở dây](https://github.com/satwikkansal/wtfpython/issues/new)).
    - Nếu câu trả lời là "có, tôi đã hiểu", bạn có thể đọc ví dụ tiếp theo.
PS: Bạn có thể đọc WTFPython dùng chế độ dòng lệnh sử dụng [pypi package](https://pypi.python.org/pypi/wtfpython),
```sh
$ pip install wtfpython -U
$ wtfpython
```
---

# 👀 Các ví dụ

## Chương 1: Hack não!

### ▶ Món khai vị! *

<!-- Example ID: d3d73936-3cf1-4632-b5ab-817981338863 -->
<!-- read-only -->

For some reason, the Python 3.8's "Walrus" operator (`:=`) has become quite popular. Let's check it out,
Kí hiệu "con hà mã" ("Walrus" operator), được giới thiệu trong phiên bản Python 3.8 đã trở nên khá phổ biến vì một vài lý do. Hãy thử qua nó xem
1\.

```py
# Phiên bản Python 3.8+

>>> a = "wtf_walrus"
>>> a
'wtf_walrus'

>>> a := "wtf_walrus"
File "<stdin>", line 1
    a := "wtf_walrus"
      ^
SyntaxError: invalid syntax (Lỗi về cú pháp: Cú pháp không hợp lệ)

>>> (a := "wtf_walrus") # This works though
>>> a
'wtf_walrus'
```

2 \.

```py
# Phiên bản Python 3.8+

>>> a = 6, 9
>>> a
(6, 9)

>>> (a := 6, 9)
>>> a
6

>>> a, b = 6, 9 # Phân rã (unpacking) các giá trị, hay còn gọi là câu lệnh gán đa giá trị (multiple assignments)
>>> a, b
(6, 9)
>>> (a, b = 16, 19) # Có 
  File "<stdin>", line 1
    (a, b = 6, 9)
          ^
SyntaxError: invalid syntax (Lỗi cú pháp: cú pháp không hợp lệ)

>>> (a, b := 16, 19) # Câu lệnh này in ra một tuple có 3 phần tử không như mong đợi (đáng lẽ là 2 phần tử 16 và 19)
(6, 16, 19)

>>> a # a được được gán lại giá trị trước đó, nhưng giá trị phía dưới vẫn giữ nguyên, là sao?
6

>>> b 
16
```



#### 💡 Giải thích

**Ôn lại một chút về kí hiệu "con hà mã"**

Kí hiệu con hà mã (`:=`) lần đầu tiên được giới thiệu trong phiên bản Python 3.8, nó hữu dụng khi bạn muốn gán giá trị cho các biến bên trong một biểu diễn (expression).

```py
def some_func():
        # Giả định rằng ta thực hiện một vài phép tính tốn nhiều tài nguyên (thời gian, I/O) ở đây
        # time.sleep(1000)
        return 5

# Thay vì thực hiện việc kiểm tra kết quả trả về của hàm trên,
if some_func():
        print(some_func()) # Và gọi lại hàm đó trong thân điều kiện, nghĩa là thực hiện các tính toán trong hàm 2 lần.
# Hay tốt hơn, ta có thể tiết kiệm một lời gọi hàm thông qua việc lấy về giá trị trả về ở một lần gọi và thực hiện so sánh trên giá trị đó:
a = some_func()
if a:
    print(a)

# Dùng kĩ hiệu con hà mã bạn có thể viết ngắn gọn hơn như dưới đây, phép gán được sử dụng như mệnh đề điều kiện và ta có thể sử dụng biến được gán giá trị trong thân câu điều kiện if:
if a := some_func():
        print(a)
```

**Kết quả (> 3.8):**

```py
5
5
5
```

Sử dụng kí hiệu con hà mã giúp ta rút ngắn được đoạn mã đi một dòng và tránh được việc gọi `some_func` hai lần.
  
- Ta chỉ được sử dụng phép gán có kí hiệu hà mã ở cấp độ cao nhất do đó lỗi cú pháp (`SyntaxError`) trong câu lệnh `a := "wtf_walrus"` xảy ra. Khi ta cho phép gán này vào hai dấu ngoặc đơn `()` thì sẽ không bị lỗi nữa.  

- Thông thường, câu lệnh có dấu bằng `=` sẽ không được phép đặt trong dấu ngoặc đơn. Do vậy câu lệnh `(a, b = 6, 9)` bị lỗi cú pháp. 

- Cú pháp của kí hiệu gán con hà mã như sau: `NAME:= expr`, ở đó `NAME` là một tên biến hợp lệ, và `expr` là một biểu diễn hợp lệ. Do vậy, việc sử dụng các phép gộp (packing) hay phân rã trong trường hợp này sẽ không được hỗ trợ, nghãi là 
  - `(a := 6, 9)` tương đương với `((a := 6), 9)` và buổi diễn cuối cùng là  `(a, 9) ` (ở đó giá trị của  `a` là 6). Bạn có thể kiểm tra lại với các dòng lệnh dưới đây

    ```py
    >>> (a := 6, 9) == ((a := 6), 9)
    True # Biểu diễn bên trái bằng bên phải do phép phân rã không được phép (như đã giải thích phía trên)
    >>> x = (a := 696, 9)
    >>> x
    (696, 9)
    >>> x[0] is a # Cả x[0] và a cùng trỏ về chung một địa chỉ trong bộ nhớ 
    True
    ```

  - Tương tự, `(a, b := 16, 19)` tương đương với `(a, (b := 16), 19)` khi ta có 3 giá trị trong một tuple. 

---

### ▶ Strings thỉnh thoảng có thể khá oái oăm

<!-- Example ID: 30f1d3fc-e267-4b30-84ef-4d9e7091ac1a --->
1\.

```py
>>> a = "some_string"
>>> id(a)
140420665652016
>>> id("some" + "_" + "string") # Để ý rằng cả hai giá trị id đều giống nhau (140420665652016).
140420665652016
```

2\.
```py
>>> a = "wtf"
>>> b = "wtf"
>>> a is b
True # a và b cùng trỏ tới một địa chỉ trong bộ nhớ

>>> a = "wtf!"
>>> b = "wtf!"
>>> a is b
False # a và b không cùng trỏ tới một địa chỉ trong bộ nhớ

```

3\.

```py
>>> a, b = "wtf!", "wtf!"
>>> a is b # Áp dụng cho tất cả các phiên bản Python, ngoại trừ các phiên bản 3.7.x
True # a và b cùng trỏ tới một địa chỉ trong bộ nhớ

>>> a = "wtf!"; b = "wtf!"
>>> a is b # Kết quả là True hoặc False tuỳ thuộc vào môi trường bên chạy đoạn mã (python shell / ipython / as a script)
False
```

```py
# Tạo một file tên some_file.py, chứa ba dòng code dưới đây:
a = "wtf!"
b = "wtf!"
print(a is b)

# Khi file này được chạy kết quả in ra là True

```

4\.

**Kết quả (< Python3.7 )**

```py
>>> 'a' * 20 is 'aaaaaaaaaaaaaaaaaaaa'
True
>>> 'a' * 21 is 'aaaaaaaaaaaaaaaaaaaaa'
False
```

Có gì đó sai sai?

#### 💡 Explanation:
+ The behavior in first and second snippets is due to a CPython optimization (called string interning) that tries to use existing immutable objects in some cases rather than creating a new object every time.
+ After being "interned," many variables may reference the same string object in memory (saving memory thereby).
+ In the snippets above, strings are implicitly interned. The decision of when to implicitly intern a string is implementation-dependent. There are some rules that can be used to guess if a string will be interned or not:
  * All length 0 and length 1 strings are interned.
  * Strings are interned at compile time (`'wtf'` will be interned but `''.join(['w', 't', 'f'])` will not be interned)
  * Strings that are not composed of ASCII letters, digits or underscores, are not interned. This explains why `'wtf!'` was not interned due to `!`. CPython implementation of this rule can be found [here](https://github.com/python/cpython/blob/3.6/Objects/codeobject.c#L19)
  ![image](/images/string-intern/string_intern.png)
+ When `a` and `b` are set to `"wtf!"` in the same line, the Python interpreter creates a new object, then references the second variable at the same time. If you do it on separate lines, it doesn't "know" that there's already `"wtf!"` as an object (because `"wtf!"` is not implicitly interned as per the facts mentioned above). It's a compile-time optimization. This optimization doesn't apply to 3.7.x versions of CPython (check this [issue](https://github.com/satwikkansal/wtfpython/issues/100) for more discussion).
+ A compile unit in an interactive environment like IPython consists of a single statement, whereas it consists of the entire module in case of modules. `a, b = "wtf!", "wtf!"` is single statement, whereas `a = "wtf!"; b = "wtf!"` are two statements in a single line. This explains why the identities are different in `a = "wtf!"; b = "wtf!"`, and also explain why they are same when invoked in `some_file.py`
+ The abrupt change in the output of the fourth snippet is due to a [peephole optimization](https://en.wikipedia.org/wiki/Peephole_optimization) technique known as Constant folding. This means the expression `'a'*20` is replaced by `'aaaaaaaaaaaaaaaaaaaa'` during compilation to save a  few clock cycles during runtime. Constant folding only occurs for strings having a length of less than 20. (Why? Imagine the size of `.pyc` file generated as a result of the expression `'a'*10**10`). [Here's](https://github.com/python/cpython/blob/3.6/Python/peephole.c#L288) the implementation source for the same.
+ Note: In Python 3.7, Constant folding was moved out from peephole optimizer to the new AST optimizer with some change in logic as well, so the fourth snippet doesn't work for Python 3.7. You can read more about the change [here](https://bugs.python.org/issue11549). 

---


### ▶ Be careful with chained operations
<!-- Example ID: 07974979-9c86-4720-80bd-467aa19470d9 --->
```py
>>> (False == False) in [False] # makes sense
False
>>> False == (False in [False]) # makes sense
False
>>> False == False in [False] # now what?
True

>>> True is False == False
False
>>> False is False is False
True

>>> 1 > 0 < 1
True
>>> (1 > 0) < 1
False
>>> 1 > (0 < 1)
False
```

#### 💡 Giải thích:

As per https://docs.python.org/2/reference/expressions.html#not-in


> Nếu a, b, c, ..., y, z là các biểu diễn (expressions) và op1, op2, ..., opN là các phép so sánh, khi đó op1 b op2 c ... y opN z tương đương với op1 b and b op2 c and ... y opN, ngoại trì việc mỗi biểu diễn được thực hiện hay đánh giá nhiều nhât một lần

Trong khi những điều ta thấy phía trên có thể hơi ngớ ngẩn đối với bạn, ta có thể làm những thứ thú vị hơn như `a == b == c` và `0 <= x <= 100`.

* `False is False is False` tương đương `(False is False) and (False is False)`
* `True is False == False` tương đương với `True is False and False == False` và do phần so sánh đầu tiên (`True is False`) cho ra kết quả `False`, do đó kết quả cuối cùng là `False`.
* `1 > 0 < 1` tương đương với `1 > 0 and 0 < 1` và cho ra kết quả là `True`.
* Biểu diễn `(1 > 0) < 1` tương đương với `True < 1` và
  ```py
  >>> int(True)
  1
  >>> True + 1 #làm cho vui thôi, chứ không liên quan
  2
  ```
  do đó, `1 < 1` cho ra kết quả`False`

---

### ▶ How not to use `is` operator
<!-- Example ID: 230fa2ac-ab36-4ad1-b675-5f5a1c1a6217 --->
Ví dụ dươi đây rất nổi tiếng trên Internet
1\.

```py
>>> a = 256
>>> b = 256
>>> a is b
True

>>> a = 257
>>> b = 257
>>> a is b
False
```

2\.

```py
>>> a = []
>>> b = []
>>> a is b
False

>>> a = tuple()
>>> b = tuple()
>>> a is b
True
```

3\.
**Kết quả**

```py
>>> a, b = 257, 257
>>> a is b
True
```

**Kết qủa (Chỉ áp dụng cho Python 3.7.x )**

```py
>>> a, b = 257, 257
>> a is b
False
```

#### 💡 Giải thích:

**Sự khác biệt giữa `is` và `==`**

* `is` kiểm tra xem cả hai phần tử so sánh có trỏ về cùng một đôi tượng (ví dụ, `is` kiểm tra định danh của cả hai thành phần được so sánh có khớp với nhau hay không)
* `==` so sánh giá trị của hai phần tử xem chúng có bằng nhau hay không
* Vì thế `is` được dùng cho việc so sánh tham chiếu và `==` được dùng cho so sánh tham trị. Hãy xem ví dụ dưới đây để hiểu rõ hơn
  ```py
  >>> class A: pass
  >>> A() is A() # Hai đối tượng rỗng nhưng nằm ở hai vị trí khác nhau trong bộ nhớ.
  False
  ```
** `256` là một đối tượng hiện hữu nhưng `257` lại không phải là một đối tượng hiện hữu.

Khi bạn khởi chạy python các số từ `-5` tới `256` sẽ được cấp phát. Những sô nay được sử dụng rất nhiều, do đó việc cấp phát này là hợp lý.
Tham khảo từ https://docs.python.org/3/c-api/long.html

> Cách triển khai hiện hành của Python duy trì một mảng các đối tượng sô nguyên từ -5 tới 256, khi bạn tạo một số nguyên trong dải này bạn sẽ quay trở về lại một tham chiếu tới một đôi tượng tồn tại. Do vậy ta vẫn có thể thay đổi giá trị của 1. 

```py
>>> id(256)
10922528
>>> a = 256
>>> b = 256
>>> id(a)
10922528
>>> id(b)
10922528
>>> id(257)
140084850247312
>>> x = 257
>>> y = 257
>>> id(x)
140084850247440
>>> id(y)
140084850247344
```


Ở đây trình thông dịch không đủ thông minh khi thực thi `y = 257` và nhận ra rằng chúng ta đã tạo một số nguyên có giá trị là `257,` rồi, do đó nó tiếp tục tạo một đôi tượng khác trong bộ nhớ. 

Một tối ưu tương tự áp dụng cho các đối tượng bất biến (**immutable**) khác như là các tuples. Bởi vì lists có thể biến đổi được, do đó ta hiểu tại sao `[] is []` sẽ trả về `False` và `() is ()` sẽ trả về `True`. Điều này giải thích đoạn mã thứ hai. Nào hãy cùng đi qua ví dụ thứ 3.

** Cả `a` và `b` đều trỏ về cùng một đối tượng khi được khởi tạo với cung một giá trị và trên cùng một dòng code**
**Kết quả**

```py
>>> a, b = 257, 257
>>> id(a)
140640774013296
>>> id(b)
140640774013296
>>> a = 257
>>> b = 257
>>> id(a)
140640774013392
>>> id(b)
140640774013488
```


* Trên cùng một dòng code nơi cả a va b được gán cho giá trị `257`, trinh thông dịch Python tạo một đôi tượng mới, sau đó trỏ tới biến thứ hai cùng một lúc. Nếu bạn thực hiện việc gán trên các dòng riêng biệt, Python sẽ không biết rằng đã có săn một đối tượng `257`

* Đây là một tối ưu của trình biên dịch, và áp dụng cụ thể cho môi trường tương tác (interactive environment). Khi bạn nhập hai dòng code trong phiên thôn dịch động, chúng được biên dịch riêng, do đó được tối ưu riêng. Nếu bạn thử ví dụ này trong một file `.py` bạn sẽ không thấy điều trên xảy ra do file code được biên dịch một lần. Tối ưu nay không chỉ giơi hạn cho các số nguyên, nó còn hoạt động được với các kiểu dữ liệu bất biến khác như strings (xem "Strings are tricky example") và floats.
  ```py
  >>> a, b = 257.0, 257.0
  >>> a is b
  True
  ```

* Tại sao ví dụ nay lại không chạy được trên Python 3.7? Đại khái lý do là bởi vì các tối ưu của trình biên dịch áp dụng cho các trường hợp cụ thể (ví dụ. một cách tối ưu có thể thay đổi tuỳ theo phiên bản, hệ điều hành, vân vân). Tôi vân đang tìm hiểu các thay đổi cụ thể trong code triểu khai, bạn có thể xem thêm [tại đây](https://github.com/satwikkansal/wtfpython/issues/100)
---


### ▶ Hash brownies
<!-- Example ID: eb17db53-49fd-4b61-85d6-345c5ca213ff --->
1\.
```py
some_dict = {}
some_dict[5.5] = "JavaScript"
some_dict[5.0] = "Ruby"
some_dict[5] = "Python"
```

**Kết quả:**

```py
>>> some_dict[5.5]
"JavaScript"
>>> some_dict[5.0] # "Python" chiếm lấy khoá (key) của "Ruby"?
"Python"
>>> some_dict[5] 
"Python"

>>> complex_five = 5 + 0j
>>> type(complex_five)
complex
>>> some_dict[complex_five]
"Python"
```

Thế quái nào mà toàn in ra Python?


#### 💡 Giải thích

* Tính duy nhất của các khoá (keys) trong cấu trúc dữ liệu từ điển của được xác định bởi  *sự tương đương*, chứ không phải dựa trên danh tính. Do đó dẫu cho `5`, `5.0`, và `5 + 0j` là các đối tượng riêng biệt có kiểu khác nhau, nhưng bởi vì chúng băng nhau nên không thể tồn tại như một khoá riêng của `dict` (hoặc `set`). Khi bạn thêm các khoá này vào từ điển sau đó tra giá trị của khoá đó dựa trên giả định về sự tương đương thì Python chỉ trả về giá trị của khoá được chèn vào ban đầu (thay vì trả lại lỗi về truy xuất khoá `KeyError`):
  ```py
  >>> 5 == 5.0 == 5 + 0j
  True
  >>> 5 is not 5.0 is not 5 + 0j
  True
  >>> some_dict = {}
  >>> some_dict[5.0] = "Ruby"
  >>> 5.0 in some_dict
  True
  >>> (5 in some_dict) and (5 + 0j in some_dict)
  True
  ```
* Nguyên lý trên cũng áp dụng khi bạn gán giá trị cho khoá. Khi bạn thực hiện phép gán `some_dict[5] = "Python"`, Python tìm phần tử có sẵn trong từ điển có khoá tương đương, trong trường hợp này nè `5.0 -> "Ruby"`, ghi đè lên giá trị của khoá này ngay, và lờ đi khoá tương đương mà bạn mới cung cấp.
  ```py
  >>> some_dict
  {5.0: 'Ruby'}
  >>> some_dict[5] = "Python"
  >>> some_dict
  {5.0: 'Python'}
  ```

* Vậy làm sao để cập nhật khoá `5` vào từ điển (thay vì `5.0`)? Thực sự là chúng ta không thể làm điều đó vơi một thao tác, nhưng ta có thể xoá đi khoá cũ  (`del some_dict[5.0]`), và sau đó thiết lập khoá mới(`some_dict[5]`) để có thể lấy được khoá `5` thay vì `5.0`, tuy nhiên cách này ít ai xài tới lắm.


* Làm thế nào Python tìm khoá `5` trong từ điển có chứa sẵn khoá `5.0`? Nó làm được điều đó mà không phải dò qua mọi phần tử trong từ điển thông qua sử dụng các hàm băm (hash functions), do đó tốn thời gian chạy hằng số (constant time). Khi Python tra  khoá tên `foo` trong một tư điển, đầu tiên nó thực hiện hàm băm `hash(foo)` (với thời gian chạy hằng số). Bởi vì trong Python các đối tượng băng nhau khi chúng có chung một giá trị băm ([đọc thêm ở đây](https://docs.python.org/3/reference/datamodel.html#object.__hash__) here), `5`, `5.0`, and `5 + 0j` have the same hash value.
  ```py
  >>> 5 == 5.0 == 5 + 0j
  True
  >>> hash(5) == hash(5.0) == hash(5 + 0j)
  True
  ```
  **Ghi chú:** Các đối tượng có giá trị băm băng nhau chưa chắc đã bằng nhau. (Vẫn đề này được biết tới với tên gọi [hash collision](https://en.wikipedia.org/wiki/Collision_(computer_science)), và giảm đi hiệu năng với thời gian hằng số qua việc dùng hàm băm.)

---

### ▶ Deep down, we're all the same.
<!-- Example ID: 8f99a35f-1736-43e2-920d-3b78ec35da9b --->
```py
class WTF:
  pass
```

**Kết quả:**
```py
>>> WTF() == WTF() # two different instances can't be equal
False
>>> WTF() is WTF() # identities are also different
False
>>> hash(WTF()) == hash(WTF()) # hashes _should_ be different as well
True
>>> id(WTF()) == id(WTF())
True
```

#### 💡 Giải thích:

* Khi `id` được gọi, Python tạo một đối tượng lớp `WTF` và truyền đối tượng này cho hàm `id`. Hàm `id` lấy `id` của đối tượng (vùng nhớ của đối tượng), và vứt đối tượng này đi. Do đó đối tượng bị tiêu huỷ.
* Khi chúng ta gọi `id` hai lần, Python cấp phát cùng một vùng nhơ cho đối tượng thư hai. Bởi vi (trong CPython) `id` sử dụng vùng nhớ cho id của đối tượng, id của hai đối tượng này là giống nhau.
* Vì vậy, id của đối tượng chỉ duy nhất trong vòng đời của đối tượng đó. Sau khi đối tượng bị tiêu hiểu, hay trước khi nó được tạo, những thứ khác có thể có cùng id với nó.
* Nhưng tại sao phép `is` lại cho ra kết quả `False`? Hãy nhìn ví dụ dưới đây
```py
  class WTF(object):
    def __init__(self): print("I")
    def __del__(self): print("D")
  ```
  **Kết quả:**
  ```py
  >>> WTF() is WTF()
  I
  I
  D
  D
  False
  >>> id(WTF()) == id(WTF())
  I
  D
  I
  D
  True
  ```
  Như bạn quan sát thấy, có sự khác biệt ở thứ tự tiêu hiểu các đối tượng, và đó tạo ra sự khác biệt.
  
---

### ▶ Vô trật tự trong trật tự *
<!-- Example ID: 91bff1f8-541d-455a-9de4-6cd8ff00ea66 --->
```py
from collections import OrderedDict


dictionary[1] = 'a'; dictionary[2] = 'b';

ordered_dict = OrderedDict()
ordered_dict[1] = 'a'; ordered_dict[2] = 'b';

another_ordered_dict = OrderedDict()
another_ordered_dict[2] = 'b'; another_ordered_dict[1] = 'a';

class DictWithHash(dict):
    """
    A dict that also implements __hash__ magic.
    """
    __hash__ = lambda self: 0

class OrderedDictWithHash(OrderedDict):
    """
    An OrderedDict that also implements __hash__ magic.
    """
    __hash__ = lambda self: 0
```

**Kết quả**
```py
>>> dictionary == ordered_dict # Nếu a == b
True
>>> dictionary == another_ordered_dict # and b == c
True
>>> ordered_dict == another_ordered_dict # thế sao c != a ??
False

# ta biết răng set chỉ chứa các phần tử độc nhất,
# thử tạo một set chứa 3 từ điển phía trên xem sao...

>>> len({dictionary, ordered_dict, another_ordered_dict})
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: unhashable type: 'dict' (Lỗi về kiểu: kiểu không thể hash được)

# Lỗi trên xảy ra là điều dê hiểu do từ điển không được tran bị __hash__, 
# sử dụng các lớp bọc (wrapper classes) ta xây dựng phía trên thử xem.
>>> dictionary = DictWithHash()
>>> dictionary[1] = 'a'; dictionary[2] = 'b';
>>> ordered_dict = OrderedDictWithHash()
>>> ordered_dict[1] = 'a'; ordered_dict[2] = 'b';
>>> another_ordered_dict = OrderedDictWithHash()
>>> another_ordered_dict[2] = 'b'; another_ordered_dict[1] = 'a';
>>> len({dictionary, ordered_dict, another_ordered_dict})
1
>>> len({ordered_dict, another_ordered_dict, dictionary}) # xáo trộn thứ tự cá phần tử trong set
2
```

Cái quái gì đang xảy ra?

#### 💡 Giải thích:

- Lý do tại sao quy tắc so sánh bắc cầu không áp dụng được khi so sánh  `dictionary`, `ordered_dict` và `another_ordered_dict` là do cách triển khai phương thức `__eq__` trong lớp `OrderedDict` . Xem thêm [tài liệu](https://docs.python.org/3/library/collections.html#ordereddict-objects)

    >  Các phép so sánh bằng giữa các đối tượng OrderedDict tuôn theo thư tự và được thực hiện như sau. Còn phép so sánh băng giữa cá đối tượng `OrderedDict` và các đối tượng ánh xạ khác (mapping objects) thì không tuân theo thứ tự như là các từ điển thông thường..

- Lý do ở đây là các đối tượng `OrderedDict` được cho phép bị thay thế trực tiếp tại bất cứ vị trí nao một từ điển thông thường được sử dụng.
- Vậy tại sao thay đổi thư tự của các từ điển lại ảnh hưởng tới đối tượng `set` được sinh ra? Câu trả lời là do thiếu sự so sánh nội đối tượng (intrasitive) . Do sets là các tập hợp không có thứ tự của các phần tử độc nhất, thứ tự các phần tử khi chèn vào không có nghĩa lý gì cả. Nhưng trong trường hợp này, nó lại có vấn đề. Hãy tìm hiểu thêm xem sao

    ```py
    >>> some_set = set()
    >>> some_set.add(dictionary) # these are the mapping objects from the snippets above
    >>> ordered_dict in some_set
    True
    >>> some_set.add(ordered_dict)
    >>> len(some_set)
    1
    >>> another_ordered_dict in some_set
    True
    >>> some_set.add(another_ordered_dict)
    >>> len(some_set)
    1

    >>> another_set = set()
    >>> another_set.add(ordered_dict)
    >>> another_ordered_dict in another_set
    False
    >>> another_set.add(another_ordered_dict)
    >>> len(another_set)
    2
    >>> dictionary in another_set
    True
    >>> another_set.add(another_ordered_dict)
    >>> len(another_set)
    2
    ```
    Sự bất nhất ở đây  `another_ordered_dict in another_set` cho kết quả là `False` bởi vì `ordered_dict` đã tồn tại trong `another_set` trước đó, `ordered_dict == another_ordered_dict` trở thành  `False`.
    

---

### ▶ Cố thêm chút nữa... *
<!-- Example ID: b4349443-e89f-4d25-a109-82616be9d41a --->
```py
def some_func():
    try:
        return 'from_try'
    finally:
        return 'from_finally'

def another_func(): 
    for _ in range(3):
        try:
            continue
        finally:
            print("Finally!")

def one_more_func(): # A gotcha!
    try:
        for i in range(3):
            try:
                1 / i
            except ZeroDivisionError:
                # Let's throw it here and handle it outside for loop
                raise ZeroDivisionError("A trivial divide by zero error")
            finally:
                print("Iteration", i)
                break
    except ZeroDivisionError as e:
        print("Zero division error occurred", e)
```

**Kết quả:**

```py
>>> some_func()
'from_finally'

>>> another_func()
Finally!
Finally!
Finally!

>>> 1 / 0
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ZeroDivisionError: division by zero (Ngoại lệ sinh ra bởi chia một số cho số 0)

>>> one_more_func()
Iteration 0

```

#### 💡 Giải thích:

- Khi câu lệnh `return`, `break` hay `continue` được thực hiện trong phần `try` của khối "try…finally", phần `finally` cũng được thực hiện.
- Giá trị trả về của một hàm được xác định bởi câu lệnh `return` cuối cung được thực hiện. Bởi vì phần `finally` luôn được thực hiện, câu lệnh `return` trong phần `finally` sẽ luôn là câu lệnh trả về gia trị cuối cùng.
- Tuy nhiên nếu phần finally thực hiện câu lệnh `return` hay `break` thì phần ngoại lệ tồn tại sẽ bị bỏ qua.

---


### ▶ For what?
<!-- Example ID: 64a9dccf-5083-4bc9-98aa-8aeecde4f210 --->
```py
some_string = "wtf"
some_dict = {}
for i, some_dict[i] in enumerate(some_string):
    i = 10
```

**Kết quả:**
```py
>>> some_dict # An indexed dict appears.
{0: 'w', 1: 't', 2: 'f'}
```

####  💡 Giải thích:

* Câu lệnh `for` được định nghĩa trong [ngữ pháp Python](https://docs.python.org/3/reference/grammar.html) như sau:
  ```
  for_stmt: 'for' exprlist 'in' testlist ':' suite ['else' ':' suite]
  ```

  Ở đó `exprlist` là biến mục tiêu của phép gán. Điều đó co nghĩa là câu lệnh gán `{exprlist} = {next_value}` được **thực hiện đối với mỗi phần tử** trong đối tượng lặp (iterable)
  An interesting example that illustrates this:
  ```py
  for i in range(4):
      print(i)
      i = 10
  ```

  **Kết quả:**
  ```
  0
  1
  2
  3
  ```

  Bạn có nghĩ răng vòng lặp trên chỉ chạy có một lần?

  **💡 Giải thích:**

- Câu lệnh gán `i = 10` không bao giờ ảnh hưởng tới các vòng lặp do cách thức hoạt động của vòng lặp for tron Python. Trước điểm khởi đầu của mỗi vòng lặp, phần tử tiếp theo được đưa ra bởi trình sinh (iterator, trong trường hợp nay là `range(4)`), phần tử này được giải nén ra (unpacked) và gán cho các biến chạy (trong trường hợp nay là `i`)

* Hàm `enumerate(some_string)` sinh ra giá trị mới `i` (biến đếm) và một kí tự từ `some_string` tại mỗi lần lặp. Sau đó nó gán khoá `i` của từ điển `some_dict` cho kí tự đó. Trình tự được thể hiện đơn giản như dưới đây:
  ```py
  >>> i, some_dict[i] = (0, 'w')
  >>> i, some_dict[i] = (1, 't')
  >>> i, some_dict[i] = (2, 'f')
  >>> some_dict
  ```

---

### ▶ Sự khác biệt đến từ thời điểm đánh giá
<!-- Example ID: 6aa11a4b-4cf1-467a-b43a-810731517e98 --->
1\.
```py
array = [1, 8, 15]
# Một biểu diễn generator thông thường
gen = (x for x in array if array.count(x) > 0)
array = [2, 8, 22]
```

**Kết quả:**

```py
>>> print(list(gen)) # Các giá trị khác đi đâu mất rồi?
[8]
```

2\.

```py
array_1 = [1,2,3,4]
gen_1 = (x for x in array_1)
array_1 = [1,2,3,4,5]

array_2 = [1,2,3,4]
gen_2 = (x for x in array_2)
array_2[:] = [1,2,3,4,5]
```

**Kết quả:**
```py
>>> print(list(gen_1))
[1, 2, 3, 4]

>>> print(list(gen_2))
[1, 2, 3, 4, 5]
```

3\.

```py
array_3 = [1, 2, 3]
array_4 = [10, 20, 30]
gen = (i + j for i in array_3 for j in array_4)

array_3 = [4, 5, 6]
array_4 = [400, 500, 600]
```

**Kết quả:**
```py
>>> print(list(gen))
[401, 501, 601, 402, 502, 602, 403, 503, 603]
```

#### 💡 Lý giải

- Trong một biểu diễn [generator](https://wiki.python.org/moin/Generators), câu `in` được thực hiện tại thời điểm khai báo, nhưng câu điều kiện được thực hiện tại thời điểm chạy (runtime).
- Do trước thời điểm chạy, `array` được gán cho giá trị `[2, 8, 22]`, và trong ba số được gán trước đó `1`, `8` and `15`, chỉ có `8` có số lần xuất hiện trong mảng mới và do đó số lần xuât hiện lớn hơn `0`, nên generator chỉ cho ra số `8`.
- Sự khác biệt giữa kết quả của `g1` and `g2` trong phần thứ hai là do cách các biến `array_1` và `array_2` được gán lại các giá trị.
- Trong trường hợp đầu tiên, `array_1` được gán cho một đối tượng mới `[1,2,3,4,5]` và vì câu `in` được thực hiện tại thời điểm khai báo nên nó vẫn trỏ tới đối tượng cũ `[1,2,3,4]` (đối tượng này chưa bị mất đi).
- Trong trường hợp thư hai, phép gán lát cắt (slice assignment) `array_2` cập nhật đối tượng cũ `[1,2,3,4]` thành `[1,2,3,4,5]`. Hiển nhiên cả `g2` và `array_2` đều trỏ tới cung một đối tượng (đối tượng đã được cập nhật thành `[1,2,3,4,5]`).
 - Okay, với những gì ta quan sát trên, co phải giá trị trả về từ `list(g)` trong phần thứ ba phải là `[11, 21, 31, 12, 22, 32, 13, 23, 33]`? (bởi vì `array_3` và `array_4` sẽ giống như `array_1`). Lý do chỉ `array_4` được cập nhật được giải thích ở đây [PEP-289](https://www.python.org/dev/peps/pep-0289/#the-details)
    >Chỉ có vòng for ngoài cùng được thực hiện ngay lập tức, các lệnh khác được trì hoãn cho đến khi generator được chạy.
---


### ▶ `is not ...` không phải là `is (not ...)`

<!-- Example ID: b26fb1ed-0c7d-4b9c-8c6d-94a58a055c0d --->
```py
>>> 'something' is not None
True
>>> 'something' is (not None)
False
```

#### 💡 Giải thích

- `is not` là một toán tử nhị phân đơn, và khi thực hiện sẽ cho kết quả khác với sử dụng `is` và `not` riêng biệt.
- `is not` cho ra kết quả `False` khi các biến ở hai đầu của nó trỏ về cùng một đối tượng , và nếu hai biến này trỏ về khác đối tượng, kết quả sẽ là `True`. Cụ thể, `None` và `something` trỏ về hai biến khác nhau nên kết quả là `True`
- Trong ví dụ trên, `(not None)` sẽ cho ra kết quả `True` bởi vì khi sử dụng trong phép so sánh luận lý `None` tương đương với `False`, do đó dòng mã trên sẽ trở thành `'something' is True`. Cụ thể, do `something` và `True` trỏ về hai đối tượng khác nhau nên kết quả là `False`

---

### ▶ A tic-tac-toe where X wins in the first attempt!
<!-- Example ID: 69329249-bdcb-424f-bd09-cca2e6705a7a --->

```py
# Khởi tạo một hàng
row = [""] * 3 #row i['', '', '']
# Và tạo một bảng gồm các hàng
board = [row] * 3
```

**Kết quả:**

```py
>>> board
[['', '', ''], ['', '', ''], ['', '', '']]
>>> board[0]
['', '', '']
>>> board[0][0]
''
>>> board[0][0] = "X"
>>> board
[['X', '', ''], ['X', '', ''], ['X', '', '']]
```

Chúng ta đã gán `"X"` cho ba vị trí trong bảng này chăng?

#### 💡 Giải thích:

Khi chúng ta khởi tạoi biến `row`, hình mô phỏng dưới đây cho ta biết những gì diễn ra trong bộ nhớ

![image](/images/tic-tac-toe/after_row_initialized.png)


Khi `board` được khởi tạo băng việc nhân bản `row`, minh hoạ phía dưới mô tả những gì diên ra trong bộ nhớ (mỗi thành phần của bảng `board[0]`, `board[1]` và `board[2]` là một tham chiếu tới cung một danh sách trỏ bởi `row`)

![image](/images/tic-tac-toe/after_board_initialized.png)

Chúng ta có thể tránh điều trên xảy ra bằng cách không dùng biến `row` để sinh ra `board`. (Tim hiểu thêm tại (https://github.com/satwikkansal/wtfpython/issues/68) )
```py
>>> board = [['']*3 for _ in range(3)]
>>> board[0][0] = "X"
>>> board
[['X', '', ''], ['', '', ''], ['', '', '']]
```

---

### ▶ The sticky output function
<!-- Example ID: 4dc42f77-94cb-4eb5-a120-8203d3ed7604 --->

1\.

```py
funcs = []
results = []
for x in range(7):
    def some_func():
        return x
    funcs.append(some_func)
    results.append(some_func())  # Chú ý lời gọi hàm ở đây

funcs_results = [func() for func in funcs]
```

**kết quả:**

```py
>>> results
[0, 1, 2, 3, 4, 5, 6]
>>> funcs_results
[6, 6, 6, 6, 6, 6, 6]
```
Ngay cả khi các giá trị `x` khác nhau trong mọi vòng lặp trước khi đặt `some_func` vào trong danh sách `funcs`, tất cả các hàm đều trả về 6.

2\.

```py
>>> powers_of_x = [lambda x: x**i for i in range(10)]
>>> [f(2) for f in powers_of_x]
[512, 512, 512, 512, 512, 512, 512, 512, 512, 512]
```

#### 💡 Lý giải

- Khi định nghia một hàm bên trong một vòng lặp, vòng lặp có biến lặp được sử dụng trong thân hàm, closure của hàm này được giơi hạn cho biến, chư không phải là giá trị. Vì vậy tất cả các ham sử dụng giá trị cuối cung được gán cho biến này để thực hiện tính toán. Để rõ hơn ta thấy được rằng biến lặp `x` (và giá trị của cung của nó nhận được là `6`) trong ví dụ thứ nhất được sử dụng cho tất cả các hàm `func()`, hàm này sẽ luôn trả về giá trị là `6` 

- Để thực hiện được tính toán mong muốn bạn có thể truyền biến lặp như là biến được đặt tên (named variable) cho hàm. **Sao mà nó lại chạy đúng được?** ởi vì việc truyền biến như vậy sẽ định nghĩa lại biến nay bên trong phạm vi của hàm.

    ```py
    funcs = []
    for x in range(7):
        def some_func(x=x):
            return x
        funcs.append(some_func)
    ```

    **Kết quả:**
    ```py
    >>> funcs_results = [func() for func in funcs]
    >>> funcs_results
    [0, 1, 2, 3, 4, 5, 6]
    ```

---

### ▶ Bài toán con gà và quả trứng *
<!-- Example ID: 60730dc2-0d79-4416-8568-2a63323b3ce8 --->
1\.
```py
>>> isinstance(3, int)
True
>>> isinstance(type, object)
True
>>> isinstance(object, type)
True
```

Đâu là lớp cơ bản cuối cùng ? Còn nhiều thứ gây khó hiểu hơn nữa sau đây

2\. 

```py
>>> class A: pass
>>> isinstance(A, A)
False
>>> isinstance(type, type)
True
>>> isinstance(object, object)
True
```

3\.

```py
>>> issubclass(int, object)
True
>>> issubclass(type, object)
True
>>> issubclass(object, type)
False
```


#### 💡 Giải thích

- `type` là một [metaclass](https://realpython.com/python-metaclasses/) trong Python.
- **Mọi thứ** đều là một đối tượng `object` trong Python, bao gồm cả các lớp (classes) cũng như là các hiện thực của chúng (instances).
- Lớp `type` là metaclass của lớp `object`, do đó mọi lớp (gồm cả `type`) thừa hưởng trực tiếp hay gián tiếp từ `object`.
- Không có một lớp nào nằm giữa lớp `object` và `type`. Vấn đề đối với các đoạn mã phía trên nằm ở cách ta tìm các mối quan hệ giữa các lớp trong Python (dùng `issubclass` và `isinstance`). Mỗi quan hệ giữa `object` và `type` không thể được định nghĩa trong Python đơn thuần. Chính xác hơn, nghĩa là,
    + Lớp A là một hiện thực của lớp B, và lớp B là một hiện thực của lớp A.  
    + Lớp A là một hiện thực của chính nó.
- Các mối quan hệ giữa `object` và `type` (ở cả hai cấp độ hiện thực cũng như chính lớp đó) tồn tại là do việc "ăn gian" khi triển khai các lớp này.
---

### ▶ Các mối quan hệ của lơp con (subclass)

<!-- Example ID: 9f6d8cf0-e1b5-42d0-84a0-4cfab25a0bc0 --->
**Kết quả:**
```py
>>> from collections import Hashable
>>> issubclass(list, object)
True
>>> issubclass(object, Hashable)
True
>>> issubclass(list, Hashable)
False
```

Mối quan hệ giữa các lớp con có tính bắc cầu không?(ví dụ, nếu `A` là lớp con của `B`, và `B` là lớp con của `C`, vậy `A` _nên_ là lớp con của `C`)

#### 💡 Lý giải:

* Trong Python mối quan hệ giữa cá lớp con không nhất thiết phải mang tính bắc cầu. Bất cứ ai cũng được phép định nghĩa một lớp `__subclasscheck__` riêng, tuỳ ý trong một siêu lớp (metaclass).
* Khi `issubclass(cls, Hashable)` được gọi, nó chỉ tìm phương thức non-Falsey "`__hash__`"  trong `cls` hoặc bất cư thư gì nó thừa hưởng từ đó.
* Bởi vì `object` là một đối tượng có thể băm (hashable), còn `list` thi không, nên nó phá vỡ tính bắc cầu.
* Giải thích chi tiết có thể xem [ở đây](https://www.naftaliharris.com/blog/python-subclass-intransitivity/).

---

### ▶ All-true-ation *

<!-- Example ID: dfe6d845-e452-48fe-a2da-0ed3869a8042 -->

```py
>>> all([True, True, True])
True
>>> all([True, True, False])
False

>>> all([])
True
>>> all([[]])
False
>>> all([[[]]])
True
```

Lý do vì sao mà lúc thì True mà lúc thì lại False

#### 💡 Giải thích:

- Hàm `all` tương đương như đoạn mã dưới

- ```py
  def all(iterable):
      for element in iterable:
          if not element:
              return False
      return True
  ```

- `all([])` trả về `True` bởi vì danh sách nay rỗng. 
- `all([[]])` trả về `False` bởi vì `not []` là `True` tương đương với `not False` bởi vì danh sách phía trong rỗng.
- `all([[[]]])` và các biến thể đệ quy cao hơn luôn trả về `True` bởi vì `not [[]]`, `not [[[]]]`, tương đương với`not True`.
---

### ▶ Dấu phẩy lạ lùng
<!-- Example ID: 31a819c8-ed73-4dcc-84eb-91bedbb51e58 --->
**Kết quả (< 3.6):**

```py
>>> def f(x, y,):
...     print(x, y)
...
>>> def g(x=4, y=5,):
...     print(x, y)
...
>>> def h(x, **kwargs,):
  File "<stdin>", line 1
    def h(x, **kwargs,):
                     ^
SyntaxError: invalid syntax (Lỗi cú pháp không hợp lệ)

>>> def h(*args,):
  File "<stdin>", line 1
    def h(*args,):
                ^
SyntaxError: invalid syntax (Lỗi cú pháp không hợp lệ)
```

#### 💡 Lý giải:

- Dấu phẩy nằm ở cuối danh sách các tham số của một hàm không phải bao giờ cũng hợp lệ.
-  Trong Python, danh sách tham số được định nghĩa bởi một phần các dấu phẩy nằm phía trước và một phần các dấy phẩy nằm phía sau. Điều nay mâu thuẫn với các tình huống ở đó một dấu phẩy bị mắc kẹt ở giữa danh sách, và chẳng có một luật nào chấp nhận điều này cả.
-  **Chú ý:** Vấn đề về dâu phẩy ở cuối  [đã được sửa trong Python 3.6](https://bugs.python.org/issue9232). Thảo luận [ở đây](https://bugs.python.org/issue9232#msg248399) cung cấp những cách dung khác nhau của dây phẩy ở cuối.

---

### ▶ Strings and the backslashes
<!-- Example ID: 6ae622c3-6d99-4041-9b33-507bd1a4407b --->
**Kết quả:**
```py
>>> print("\"")
"

>>> print(r"\"")
\"

>>> print(r"\")
File "<stdin>", line 1
    print(r"\")
              ^
SyntaxError: EOL while scanning string literal

>>> r'\'' == "\\'"
True
```

#### 💡 Giải thích

- Trong một string thông thường, dấu xuyệc ngược được dùng để "escape" các kí tự có một ý nghĩa đặc biệt (như là dấu trích dẫn đơn, dấu trích dẫn kép, va chính dấu xuyệc ngược).
    ```py
    >>> "wt\"f"
    'wt"f'
    ```
- Đối với một string thô (raw string) (được chỉ định bởi tiếp đầu ngữ `r`), dấu xuyệc ngược.
    ```py
    >>> r'wt\"f' == 'wt\\"f'
    True
    >>> print(repr(r'wt\"f')
    'wt\\"f'

    >>> print("\n")

    >>> print(r"\\n")
    '\\\\n'
    ```
- This means when a parser encounters a backslash in a raw string, it expects another character following it. And in our case (`print(r"\")`), the backslash escaped the trailing quote, leaving the parser without a terminating quote (hence the `SyntaxError`). That's why backslashes don't work at the end of a raw string.
- Có nghĩa là khi một trình phân tích cú pháp gặp một dấu xuyệc ngược tron một string thô, trình này mong đợi một kí tự khác phía sau nó. Và tron trường hợp `print(r"\")`, dấu xuyêcj ngược escape dấu trích dẫn ở đuôi, DỊCH LẠI

---

### ▶ not knot!
<!-- Example ID: 7034deb1-7443-417d-94ee-29a800524de8 --->
```py
x = True
y = False
```

**Kết quả:**
```py
>>> not x == y
True
>>> x == not y
  File "<input>", line 1
    x == not y
           ^
SyntaxError: invalid syntax (Lỗi về cú pháp)
```

#### 💡 Giải thích:

* Thứ tự ưu tiên của các phép toán ảnh hưởng tơi cách một câu lệnh được thực thi, và phép `==` có độ ưu tiên cao hơn phép `not` trong Python.
* Vì vậy `not x == y` tương đương với `not (x == y)` rồi tương đương với `not (True == False)` và kết quả là`True`.
* Nhưng `x == not y` gây ra lỗi cú pháp `SyntaxError` bởi vì Python nghĩ rằng nó sẽ thực hiện `(x == not) y` chứ không phải là `x == (not y)` do đó bạn mới gặp lỗi về cú pháp.
* Trình phân tích cú pháp mong đợi `not` là một phần của phép toán `not in` (bởi vì cả  `==` và `not in` có cùng độ ưu tiên), nhưng do trong trương hợp của chúng ta, trình xử lý không tìm thấy `in` đằng sau `not`, nên nó gây ra `SyntaxError`.

---

### ▶ Các chuỗi rưỡi trích dẫn
<!-- Example ID: c55da3e2-1034-43b9-abeb-a7a970a2ad9e --->
**Kết quả:**
```py
>>> print('wtfpython''')
wtfpython
>>> print("wtfpython""")
wtfpython
>>> # Các câu lệnh phía dưới gặp lỗi cú pháp `SyntaxError` khi thực thi
>>> # print('''wtfpython')
>>> # print("""wtfpython")
  File "<input>", line 3
    print("""wtfpython")
                        ^
SyntaxError: EOF while scanning triple-quoted string literal (Lỗi cú pháp khi sử lý chuỗi được bao bởi dấu trích dẫn)
```

#### 💡 Giải thích:
+ Python hỗ trợ ngầm [ghép chuỗi](https://docs.python.org/2/reference/lexical_analysis.html#string-literal-concatenation), ví dụ,
  ```
  >>> print("wtf" "python")
  wtfpython
  >>> print("wtf" "") # or "wtf"""
  wtf
  ```

+ `'''` và `"""` là các kí hiệu phân cách chuỗi trong Python, chúng tạo ra lỗi SyntaxError bởi vì trình thông dịch Python chơ đợi kí hiệu phân cách kết thúc khi nó dò tìm chuỗi kí tự trích dẫn có ba dấu nháy .
---

### ▶ Có gì sai sai với các giá trị luận lý (booleans)?
<!-- Example ID: 0bba5fa7-9e6d-4cd2-8b94-952d061af5dd --->
1\.

```py
# Một ví dụ tính toán số lượng các giá trị luận lý và
# sô nguyên trong một danh sách lẫn lộn các kiểu phần tử khác nhau.
mixed_list = [False, 1.0, "some_string", 3, True, [], False]
integers_found_so_far = 0
booleans_found_so_far = 0

for item in mixed_list:
    if isinstance(item, int):
        integers_found_so_far += 1
    elif isinstance(item, bool):
        booleans_found_so_far += 1
```

**Kết quả:**
```py
>>> integers_found_so_far
4
>>> booleans_found_so_far
0
```


2\.
```py
>>> some_bool = True
>>> "wtf" * some_bool
'wtf'
>>> some_bool = False
>>> "wtf" * some_bool
''
```

3\.

```py
def tell_truth():
    True = False
    if True == False:
        print("I have lost faith in truth!")
```

**Kết quả (< 3.x):**

```py
>>> tell_truth()
I have lost faith in truth!
```

#### 💡 Lý giải:

* `bool` là lơp con của `int` trong Python
    
    ```py
    >>> issubclass(bool, int)
    True
    >>> issubclass(int, bool)
    False
    ```
    
* Và do vậy, `True` và `False` là các hiện thực (instances) của `int`
  ```py
  >>> isinstance(True, int)
  True
  >>> isinstance(False, int)
  True
  ```

* Giá trị dạng số nguyên của `True` là `1` và của `False` là `0`.
  ```py
  >>> int(True)
  1
  >>> int(False)
  0
  ```

* Xem trên [câu trả lời] trên StackOverflow(https://stackoverflow.com/a/8169049/4354153) để biết lý do.

* Lúc đầu, Python không có kiểu `bool` (người ta dung 0 cho false và các giá trị khác không như 1 cho true).  `True`, `False`, va kiểu `bool` được bổ sung trong cá phiên bản 2.x, nhưng vi lý do hỗ trợ tương thích ngược (backward compatibility), `True` và `False` không thể trơ thành các hăng số (constants). Chúng chỉ là các biến được tích hợp sẵn trong Python, và ta có thể gán lại giá trị cho chúng.

* Python 3 không hỗ trợ tương thích ngược, và do vậy các đoạn mã cuối cung không chạy được trên  Python 3.x!
---

### ▶ Class attributes and instance attributes
<!-- Example ID: 6f332208-33bd-482d-8106-42863b739ed9 --->
1\.
```py
class A:
    x = 1

class B(A):
    pass

class C(A):
    pass
```

**Kết quả:**
```py
>>> A.x, B.x, C.x
(1, 1, 1)
>>> B.x = 2
>>> A.x, B.x, C.x
(1, 2, 1)
>>> A.x = 3
>>> A.x, B.x, C.x # C.x thay đổi, nhưng B.x không thay đổi
(3, 2, 3)
>>> a = A()
>>> a.x, A.x
(3, 3)
>>> a.x += 1
>>> a.x, A.x
(4, 3)
```

2\.
```py
class SomeClass:
    some_var = 15
    some_list = [5]
    another_list = [5]
    def __init__(self, x):
        self.some_var = x + 1
        self.some_list = self.some_list + [x]
        self.another_list += [x]
```

**Kết quả:**

```py
>>> some_obj = SomeClass(420)
>>> some_obj.some_list
[5, 420]
>>> some_obj.another_list
[5, 420]
>>> another_obj = SomeClass(111)
>>> another_obj.some_list
[5, 111]
>>> another_obj.another_list
[5, 420, 111]
>>> another_obj.another_list is SomeClass.another_list
True
>>> another_obj.another_list is some_obj.another_list
True
```

#### 💡 Giải thích:

* Các biến thuộc về lớp và các biến thuộc về các hiện thực của lơp (class instances) được xử lý nội tại như là các từ điển của một đối tượng lớp. Nếu một biến không nằm trong từ điển của lớp hiện hành, nó sẽ được tìm trong các lớp cha. 
* Phép `+=` thay đổi đối tượng có thể biến đổi (mutable) tại chỗ mà khôn cần phải tạo một đối tượng mới. Vì vậy thay đổi thuộc tính cua một hiện thực ảnh hưởng tới thuộc tính của các hiện thực khác và thuộc tính lớp.
---

### ▶ Non-reflexive class method *

<!-- Example ID: 3649771a-f733-413c-8060-3f9f167b83fd -->

```py
class SomeClass:
        def instance_method(self):
                pass
        
        @classmethod
        def class_method(cls):
                pass
```

**Kết quả:**

```py
>>> SomeClass.instance_method is SomeClass.instance_method
True
>>> SomeClass.class_method is SomeClass.class_method
False
>>> id(SomeClass.class_method) == id(SomeClass.class_method)
True
```

#### 💡 Giải thích:

- Lý do là vì `SomeClass.class_method is SomeClass.class_method` trả về `False` là bởi vì decorator `@classmethod`. 

  ```py
  >>> SomeClass.instance_method
  <function __main__.SomeClass.instance_method(self)>
  >>> SomeClass.class_method
  <bound method SomeClass.class_method of <class '__main__.SomeClass'>
  ```

  Mỗi lần truy cập tới `SomeClass.class_method` là lại có một phương thức được bọc mới sinh ra (new bound method) 
-  `id(SomeClass.class_method) == id(SomeClass.class_method)` trả về `True` bởi vì quá trình cấp phát bộ nhớ cho `class_method` lần thứ hai xảy ra tại cung một ví trí với quá trình giải phóng bộ nhớ đầu tiên (Xem lại "Deep Down, we're all the same example" để có lời giải thích rõ hơn). 
---


### ▶ yielding None
<!-- Example ID: 5a40c241-2c30-40d0-8ba9-cf7e097b3b53 --->
```py
some_iterable = ('a', 'b')

def some_func(val):
    return "something"
```

**Kết quả (<= 3.7.x):**

```py
>>> [x for x in some_iterable]
['a', 'b']
>>> [(yield x) for x in some_iterable]
<generator object <listcomp> at 0x7f70b0a4ad58>
>>> list([(yield x) for x in some_iterable])
['a', 'b']
>>> list((yield x) for x in some_iterable)
['a', None, 'b', None]
>>> list(some_func((yield x)) for x in some_iterable)
['a', 'something', 'b', 'something']
```

#### 💡 Giải thích:
- Đây là một bug tồn tại khi CPython xử lý `yield` trong các generators và comprehensions.
- Bạn có thể tham khảo thêm về lỗi này tại đây: https://stackoverflow.com/questions/32139885/yield-in-list-comprehensions-and-generator-expressions
- Báo cáo về bug này: http://bugs.python.org/issue10544
- Theo Python 3.8+  `yield` không được phép nằm bên trong  list comprehension và nếu bạn làm như vậy sẽ tạo ra lỗi cú pháp `SyntaxError`.

---


### ▶ Yielding from... return! *
<!-- Example ID: 5626d8ef-8802-49c2-adbc-7cda5c550816 --->
1\.

```py
def some_func(x):
    if x == 3:
        return ["wtf"]
    else:
        yield from range(x)
```

**Kết quả (> 3.3):**

```py
>>> list(some_func(3))
[]
```

Đáng lẽ phải hiển thị `"wtf"` chứ nhỉ? Có phải là do `yield from`? Cùng tìm hiểu thêm nào,

2\.

```py
def some_func(x):
    if x == 3:
        return ["wtf"]
    else:
        for i in range(x):
          yield i
```

**Kết quả:**

```py
>>> list(some_func(3))
[]
```

Vẫn lại không in ra `"wtf"` .

#### 💡 Giải thích:

+ Từ Python 3.3 trở đi, ta có thể sử dụng `return`  với các giá trị bên trong các generators (Xem thêm [PEP380](https://www.python.org/dev/peps/pep-0380/)). Các [tài liệu chính thức](https://www.python.org/dev/peps/pep-0380/#enhancements-to-stopiteration) cũng nói như vậy,
> "... `return expr` tron một generator tạo ra ngoại lệ `StopIteration(expr)` khi thoát ra từ generator."

+ Trong trường hợp `some_func(3)`, ngoại lệ `StopIteration` được khởi lên ngay từ đầu bởi vì câu lệnh `return`. Ngoại lệ `StopIteration` được tự động bắt lại trong dòng lệnh bao `list(...)` và trong vòng lặp `for`. Do đó, cả hai đoạn mã trên đều trả về một danh sách rỗng.

+ Để có được `["wtf"]` từ generator `some_func` bạn cần bắt ngoại lệ `StopIteration`,

  ```py
  try:
      next(some_func(3))
  except StopIteration as e:
      some_string = e.value
  ```

  ```py
  >>> some_string
  ["wtf"]
  ```

---

### ▶ Tính phản xạ của Nan *
<!-- Example ID: 59bee91a-36e0-47a4-8c7d-aa89bf1d3976 --->

1\.

```py
a = float('inf')
b = float('nan')
c = float('-iNf')  # Các strings này không phân biệt hoa hay thường
d = float('nan')
```

**Kết quả:**

```py
>>> a
inf
>>> b
nan
>>> c
-inf
>>> float('some_other_string')
ValueError: could not convert string to float: some_other_string (Lỗi giá trị: Không thể chuyển đổi từ string sang float)
>>> a == -c # inf==inf
True
>>> None == None # None == None
True
>>> b == d # nhưng nan!=nan
False
>>> 50 / a
0.0
>>> a / a
nan
>>> 23 + b
nan
```

2\.

```py
>>> x = float('nan')
>>> y = x / x
>>> y is y # định danh giống nhau (cùng trỏ về một đối tượng)
True
>>> y == y # Gía trị lại không bằng nhau
False
>>> [y] == [y] # Giá trị bằng nhau khi nằm ở trong một list
True
```



#### 💡 Giải thích:

- `'inf'` và `'nan'` là các strings đặc biệt (không phân biệt hoa thường), khi được chuyển đổi sang kiểu `float` sẽ tương ứng biểu diễn cho giá trị vô hạn "infinity" hay không phải là một số "not a number".

- Theo chuẩn của IEEE thì ` NaN != NaN`, tuân theo quy tắc trên sẽ phá vỡ giả định về tính tương phản của một phần tử trong một tập trong Python ví dụ. nếu `x` là một phần tử của một tập `list`, các phép toán trên các phần tử của tập như là so sánh sẽ dựa trên giải định rằng `x == x`.  Do giả định này nên định danh được so sánh đầu tiên (do nhanh hơn) khi so sánh hai phần tử, và các giá trị được so sánh chỉ khi các định danh không khớp. Ví dụ sau sẽ giúp bạn dễ hiểu hơn
  ```py
  >>> x = float('nan')
  >>> x == x, [x] == [x]
  (False, True)
  >>> y = float('nan')
  >>> y == y, [y] == [y]
  (False, True)
  >>> x == y, [x] == [y]
  (False, False)
  ```
  
 Do các định danh của `x` và `y` khác nhau, do đó giá trị của chúng sẽ được so sánh, mà giá trị của chúng khác nhau trong ví dụ này; nên kết quả trả về là `False`. Cụ thể hơn, theo tiêu chuẩn của IEEE thì `x` f va `y` đểu có giá trị là `nan` khi được chuyển đổi qua float, ` NaN != NaN` nên `x != y`, nhưng khi đặt trong một list thì định danh sẽ đc so sánh trước nên `[x] == [y]`

- Đọc thêm: [Reflexivity, and other pillars of civilization](https://bertrandmeyer.com/2010/02/06/reflexivity-and-other-pillars-of-civilization/)

---

### ▶ Mutating the immutable!

<!-- Example ID: 15a9e782-1695-43ea-817a-a9208f6bb33d --->

Ví dụ dưới đây có vẻ tầm thường nếu bạn hiểu cách các tham chiếu (references) hoạt đông trong Python.
```py
some_tuple = ("A", "tuple", "with", "values")
another_tuple = ([1, 2], [3, 4], [5, 6])
```

**Kết quả:**
```py
>>> some_tuple[2] = "change this"
TypeError: 'tuple' object does not support item assignment (Lỗi về kiểu: đối tượng 'tuple' không hỗ trợ phép gán phần tử)
>>> another_tuple[2].append(1000) # Dòng này không bị lỗi
>>> another_tuple
([1, 2], [3, 4], [5, 6, 1000])
>>> another_tuple[2] += [99, 999]
TypeError: 'tuple' object does not support item assignment (Lỗi về kiểu: đối tượng 'tuple' không hỗ trợ phép gán phần tử)
>>> another_tuple
([1, 2], [3, 4], [5, 6, 1000, 99, 999])
```

Tôi đã nghĩ rằng các tuples thì bất biến (immutable) ...
#### 💡 Giải thích:

* Trích từ https://docs.python.org/2/reference/datamodel.html

    > Các chuỗi bất biến
        Một đối tượng kiểu chuỗi bất biến không thể thay đổi giá trị của nó sau khi được tạo. (Nếu đối tượng này chứa các tham chiếu tới các đối tượng khác, những đối tượng có thể thay đổi được; tuy thế, tập hợp các đối tượng được trỏ trực tiếp bởi một đối tượng bất biến không thể thay đổi .)

* Toán tử `+=` thay đổi list tại chỗ. Phép gán phần tử không thực hiện được, nhưng khi ngoại lệ xảy ra, phần tử đã được thay đổi ngay tại chỗ.

---

### ▶ The disappearing variable from outer scope
<!-- Example ID: 7f1e71b6-cb3e-44fb-aa47-87ef1b7decc8 --->

```py
e = 7
try:
    raise Exception()
except Exception as e:
    pass
```

**Kết quả (Python 2.x):**
```py
>>> print(e)
# Không in ra kết quả nào cả
```

**Kết quả (Python 3.x):**
```py
>>> print(e)
NameError: name 'e' is not defined (Lỗi tên biến không được định nghĩa)
```

#### 💡 Giải thích:

* Source: https://docs.python.org/3/reference/compound_stmts.html#except

  Khi một ngoại lệ được gán sử dụng đích được định nghia bởi `as`, ngoại lệ này được dọn dẹp ở cuối câu `except`. Như vậy thì

  ```py
  except E as N:
      foo
  ```

  sẽ được hiểu như sau

  ```py
  except E as N:
      try:
          foo
      finally:
          del N
  ```

  
    Điều này có nghĩa la ngoại lệ phải được gán cho một cái tên khác để ta có thể tìm thấy nó sau câu except. Các ngoại lệ được dọn dẹp bởi vì với truy lỗi (traceback) được gán cho chúng, chúng hình thành nên một vòng tham chiếu bên trong khung ngăn xếp (stack frame), giữ tất cả các biến cục bộ không bị xoá đi cho đến khi việc thu thập rác tiếp theo tiếp diễn.

* Các câu này không được tính phạm vi trong Python. Mọi thư trong ví dụ nay đều nàm trong cùng một phạm vi, và biến `e` bị xoá đi bởi vì ngoại lệ `except`. Điều tương tự như vậy không đúng với các hàm có các nội phạm vi (inner-scopes) riêng biệt. Ví dụ sau sẽ cho ta thấy:

     ```py
     def f(x):
         del(x)
         print(x)

     x = 5
     y = [5, 4, 3]
     ```

     **Kết quả:**
     ```py
     >>>f(x)
     UnboundLocalError: local variable 'x' referenced before assignment
     >>>f(y)
     UnboundLocalError: local variable 'x' referenced before assignment
     >>> x
     5
     >>> y
     [5, 4, 3]
     ```

* Trong Python 2.x, biến `e` được gán cho một hiện thực `Exception()`, khi bạn in ra biến này, nó không hiển thị gì cả

    **Kết quả (Python 2.x):**
    ```py
    >>> e
    Exception()
    >>> print e
    # Không in ra gì cả!
    ```

---


### ▶ The mysterious key type conversion
<!-- Example ID: 00f42dd0-b9ef-408d-9e39-1bc209ce3f36 --->
```py
class SomeClass(str):
    pass

some_dict = {'s': 42}
```

**Kết quả:**
```py
>>> type(list(some_dict.keys())[0])
str
>>> s = SomeClass('s')
>>> some_dict[s] = 40
>>> some_dict # Giá trị mong đợi: Hai cặp khoá và giá trị khác nhau
{'s': 40}
>>> type(list(some_dict.keys())[0])
str
```

#### 💡 Giải thích:

* Cả đối tượng `s` và string `"s"` khi được băm (hash) sẽ cho ra cùng một giá trị ởi `SomeClass` thừa kế phương thức `__hash__` của lớp `str`.
* `SomeClass("s") == "s"`  bằng `True` bởi vì `SomeClass` cũng thừa kế phương thức `__eq__` từ lớp `str` .
* Bởi vì cả hai đối tượng này khi băm cho ra cùng giá trị và bằng nhau nên chúng được biểu diễn bởi cùng một khoá trong từ điển.
* Để có được kết quả như mong muốn với hai cặp giá khoá và giá trị khác nhau, chúng ta có thể định nghĩa phương thức `__eq__` trong `SomeClass`

  ```py
  class SomeClass(str):
    def __eq__(self, other):
        return (
            type(self) is SomeClass
            and type(other) is SomeClass
            and super().__eq__(other)
        )

    # Khi chúng ta ta định nghĩa một phương thức __eq__ tuỳ chỉnh, Python tự động dừng việc thừa kế
    # và chúng ta cũng cần định nghĩa phươn thức __hash__ ,
    __hash__ = str.__hash__

  some_dict = {'s':42}
  ```

  **Kết quả:**
  ```py
  >>> s = SomeClass('s')
  >>> some_dict[s] = 40
  >>> some_dict
  {'s': 40, 's': 42}
  >>> keys = list(some_dict.keys())
  >>> type(keys[0]), type(keys[1])
  (__main__.SomeClass, str)
  ```

---

### ▶ Let's see if you can guess this?
<!-- Example ID: 81aa9fbe-bd63-4283-b56d-6fdd14c9105e --->
```py
a, b = a[b] = {}, 5
```

**Kết quả:**
```py
>>> a
{5: ({...}, 5)}
```

#### 💡 Giải thích:

* Dựa trên [Python language reference](https://docs.python.org/2/reference/simple_stmts.html#assignment-statements), các câu lệnh gán sẽ có cách khai báo như sau
  ```
  (target_list "=")+ (expression_list | yield_expression)
  ```
  và


> Câu lệnh gán thực thi  (remember that this can be a single expression or a comma-separated list, the latter yielding a tuple) and assigns the single resulting object to each of the target lists, from left to right.

* The `+` in `(target_list "=")+` means there can be **one or more** target lists. In this case, target lists are `a, b` and `a[b]` (note the expression list is exactly one, which in our case is `{}, 5`).

* Phép `+` trong `(target_list "=")+` có nghĩa là có thể có **một hay nhiều hơn** các danh sách mục tiêu. Trong trường hợp này, các danh sách mục tiêu đó là `a, b` và `a[b]` (chú ý rằng c)

* After the expression list is evaluated, its value is unpacked to the target lists from **left to right**. So, in our case, first the `{}, 5` tuple is unpacked to `a, b` and we now have `a = {}` and `b = 5`.

* `a` is now assigned to `{}`, which is a mutable object.

* The second target list is `a[b]` (you may expect this to throw an error because both `a` and `b` have not been defined in the statements before. But remember, we just assigned `a` to `{}` and `b` to `5`).

* Now, we are setting the key `5` in the dictionary to the tuple `({}, 5)` creating a circular reference (the `{...}` in the output refers to the same object that `a` is already referencing). Another simpler example of circular reference could be
  ```py
  >>> some_list = some_list[0] = [0]
  >>> some_list
  [[...]]
  >>> some_list[0]
  [[...]]
  >>> some_list is some_list[0]
  True
  >>> some_list[0][0][0][0][0][0] == some_list
  True
  ```
  Similar is the case in our example (`a[b][0]` is the same object as `a`)

* So to sum it up, you can break the example down to
  ```py
  a, b = {}, 5
  a[b] = a, b
  ```
  And the circular reference can be justified by the fact that `a[b][0]` is the same object as `a`
  ```py
  >>> a[b][0] is a
  True
  ```

---
---

## Section: Slippery Slopes

### ▶ Modifying a dictionary while iterating over it
<!-- Example ID: b4e5cdfb-c3a8-4112-bd38-e2356d801c41 --->
```py
x = {0: None}

for i in x:
    del x[i]
    x[i+1] = None
    print(i)
```

**Kết quả (Áp dụng cho các phiên bản Python 2.7- Python 3.5):**

```
0
1
2
3
4
5
6
7
```

Vòng lặp chạy đúng *tám* lần rồi dừng lại

#### 💡 Giải thích:

* Việc lặp và chỉnh sửa một từ điển cùng một lúc không được hỗ trợ.
* Có tám lần chạy bởi vì tại thời điểm dừng đó là lúc từ điển điều chỉnh kích thước để giữ thêm nhiều khoá hơn (chúng ta có tám phần từ xoá, do đó điều chỉnh kích thước là cần thiết). Đây thực sự là một chi tiết trong triển khai.
* Cách các khoá bị xoá được xử lý và khi nao thì việc điều chỉnh kích thước diễn ra sẽ khác biệt đối với các phiên bản Python khác nhau
* Do đó các phiên bản Python lớn hơn 2.7 và nhỏ hơn 3.5, số lượng cá khoá có thể giữ dao động từ 8 (nhưng khi bạn chạy thì con số này sẽ không thay đổi giữa các lần chạy). Bạn có thể xem thêm các thảo luận khác ở [đây](https://github.com/satwikkansal/wtfpython/issues/53) hoặc trên Stackoverflow tại [đây](https://stackoverflow.com/questions/44763802/bug-in-python-dict)
* Từ phiên bản 3.7.6 trở đi, bạn sẽ gặp ngoại lệ `RuntimeError: dictionary keys changed during iteration` khi bạn cố gắng thử ví dụ trên.
---

### ▶ Stubborn `del` operation
<!-- Example ID: 777ed4fd-3a2d-466f-95e7-c4058e61d78e --->
<!-- read-only -->

```py
class SomeClass:
    def __del__(self):
        print("Deleted!")
```

**Kết quả:**
1\.
```py
>>> x = SomeClass()
>>> y = x
>>> del x # this should print "Deleted!"
>>> del y
Deleted!
```


Có thể bạn đoán được làm sao mà `__del__` không được gọi khi ta cố gắng xoá `x` trong lần đầu tiên. Hãy thử thêm 
2\.
```py
>>> x = SomeClass()
>>> y = x
>>> del x
>>> y # check if y exists Kiểm tra y có tồn tại
<__main__.SomeClass instance at 0x7f98a1a67fc8>
>>> del y # Như lần trước, đáng lẽ kết quả nên là in ra "Deleted!"
>>> globals() # nhưng không, ta không có được kết quả như mong muốn. Cùng kiểm tra tất cả các biến toàn cục và xác nhận 
Deleted!
{'__builtins__': <module '__builtin__' (built-in)>, 'SomeClass': <class __main__.SomeClass at 0x7f98a1a5f668>, '__package__': None, '__name__': '__main__', '__doc__': None}
```

Ok giờ thì nó đã được xoá :confused:

#### 💡 Giải thích:
+ `del x` không gọi trực tiếp `x.__del__()`.
+ Khi `del x` được chạy, Python xoá  tên  `x` khỏi phạm vi hiện hành và giảm biến đếm tham chiếu của đối tượng đi 1. `__del__()` được gọi chỉ khi biến đếm này giảm xuống 0.
+ Tron đoạn mã thứ hai, `__del__()` không được gọi bởi vì câu lệnh trước đó (`>>> y`) tạo một tham chiếu khác tới cùng một đối tượng (cụ thể là, biến `_` trỏ tới giá trị kết quả của một biểu diễn không phải `None` tron REPL), do đó ngăn biến đếm tham chiếu giảm về 0 khi thực hiện `del y`
+ Gọi `globals` (thực ra thì thực hiện bất cứ thứ gì tạo ra kết quả không phải là `None`) làm cho `_` tham chiếu tới kết quả mới, bỏ đi tham chiếu hiện tồn tại. Bây giờ thì biến đếm tham chiếu giảm ve 0 và bạn có thể từ "Deleted!" được hiển thị.
---

### ▶ The out of scope variable
<!-- Example ID: 75c03015-7be9-4289-9e22-4f5fdda056f7 --->
```py
a = 1
def some_func():
    return a

def another_func():
    a += 1
    return a
```

**Kết quả:**
```py
>>> some_func()
1
>>> another_func()
UnboundLocalError: local variable 'a' referenced before assignment (tham chiếu tới 'a' trước khi gán giá trị)
```

#### 💡 Giải thích:
* Khi bạn gán giá trị cho một biến trong một phạm vi, thì biến này trở thành cục bộ cho phạm vi đó. Do đó `a` trở thành cục bộ đối với `another_func`, nhưng nó chưa được khởi tạo trong cùng phạm vi, nên ta gặp lỗi về tham chiếu phía trên.
* Đọc [bài này](http://sebastianraschka.com/Articles/2014_python_scope_and_namespaces.html) để học về cách hoạt động của các không gian tên (namespaces) và việc phân giải phạm vi trong Python.
* Để thay đổi biên bên ngoài phạm vi `a` bên trong hàm `another_func`, sử dụng từ khoá `global`
  ```py
  def another_func()
      global a
      a += 1
      return a
  ```

  **Kết quả:**
  ```py
  >>> another_func()
  2
  ```

---

### ▶ Deleting a list item while iterating
<!-- Example ID: 4cc52d4e-d42b-4e09-b25f-fbf5699b7d4e --->
```py
list_1 = [1, 2, 3, 4]
list_2 = [1, 2, 3, 4]
list_3 = [1, 2, 3, 4]
list_4 = [1, 2, 3, 4]

for idx, item in enumerate(list_1):
    del item

for idx, item in enumerate(list_2):
    list_2.remove(item)

for idx, item in enumerate(list_3[:]):
    list_3.remove(item)

for idx, item in enumerate(list_4):
    list_4.pop(idx)
```

**Kết quả:**
```py
>>> list_1
[1, 2, 3, 4]
>>> list_2
[2, 4]
>>> list_3
[]
>>> list_4
[2, 4]
```

Vì sao lại có kết quả là `[2, 4]`?
#### 💡 Giải thích:

* Thay đổi đối tượng trong khi lặp không phải là một cách làm hay. Cách thực hiện đúng là lặp qua một bản sao của chính đối tượng đó như trường hợp sử dụng `list_3[:]`

     ```py
     >>> some_list = [1, 2, 3, 4]
     >>> id(some_list)
     139798789457608
     >>> id(some_list[:]) # Chú ý rằng Python tạo một đối tượng mới sinh ra từ việc cắt (slice) list.
     139798779601192
     ```

**Sự khác biệt giữa `del`, `remove`, và `pop`:**
* `del var_name` chỉ loại bỏ sự có măt của `var_name` khỏi khô gian tên cục bộ và toàn cục (đó la lý do tại sao `list_1` không bị ảnh hưởng ) 
* `remove` loại bỏ giá trị được khớp đầu tiên, không phải tại một chỉ số cụ thể, ngoại lệ `ValueError` sẽ xảy ra nếu giá trị muốn loại bỏ không tồn tại.
* `pop` loại bỏ phần tử của danh sách ở mỗi chỉ số cụ thể và trả về phần từ đó, `pop` sẽ khởi lên `IndexError` nếu nó nhận một chỉ số không hợp lệ

**Tại sao kết quả lại ra `[2, 4]`?**
- Việc lặp qua danh sách được thực hiện theo từng chỉ số một, và khi chúng ta loại bỏ `1` khỏi `list_2` hay `list_4`, các danh sách này sẽ còn lại `[2, 3, 4]`. Các phần tử còn lại trong list được dịch chuyển sang trái, ví dụ như `2` sẽ có chỉ số là 0, và `3` có chỉ số là 1. Do lần lặp tiếp theo sẽ xử lý phần tử có chỉ số là 1 (`3`), nên phần tử tại chỉ số 0 (`2`) sẽ bị bỏ qua. 

* Xem thêm tại StackOverflow [thread](https://stackoverflow.com/questions/45946228/what-happens-when-you-try-to-delete-a-list-element-while-iterating-over-it) explaining the example
* Và xem thêm ở đây để có các ví dụ liên quan tới các từ điển [thread](https://stackoverflow.com/questions/45877614/how-to-change-all-the-dictionary-keys-in-a-for-loop-with-d-items).

---


### ▶ Lossy zip of iterators *
<!-- Example ID: c28ed154-e59f-4070-8eb6-8967a4acac6d --->

```py
>>> numbers = list(range(7))
>>> numbers
[0, 1, 2, 3, 4, 5, 6]
>>> first_three, remaining = numbers[:3], numbers[3:]
>>> first_three, remaining
([0, 1, 2], [3, 4, 5, 6])
>>> numbers_iter = iter(numbers)
>>> list(zip(numbers_iter, first_three)) 
[(0, 0), (1, 1), (2, 2)]
# so far so good, let's zip the remaining
>>> list(zip(numbers_iter, remaining))
[(4, 3), (5, 4), (6, 5)]
```
Phần tử  `3` trong `numbers` đâu?
#### 💡 Giải thích:

- Theo tài liệu của Python [docs](https://docs.python.org/3.3/library/functions.html#zip), triển khai gần nhất của hàm zip như sau,
    ```py
    def zip(*iterables):
        sentinel = object()
        iterators = [iter(it) for it in iterables]
        while iterators:
            result = []
            for it in iterators:
                elem = next(it, sentinel)
                if elem is sentinel: return
                result.append(elem)
            yield tuple(result)
    ```
- Hàm này nhận vào một số tuỳ ý các đối tượng có thể lặp (iterable objects), thêm mỗi phần tử của các đối tượng này vào danh sách `result` thông qua việc gọi hàm `next` trên đối tượng này, và dưng lại khi đôi tượng này hết các phần tử để lặp   
- Chú ý là khi bất cứ đối tượng lặp nào cạn kiệt đối tượng lặp, các phần tử tồn tại trong danh sách `result` được bỏ qua. Đó là những gì xảy với `3` trong `numbers_iter`
- Để thực hiện đúng, ta cần làm như sau
    ```py
    >>> numbers = list(range(7))
    >>> numbers_iter = iter(numbers)
    >>> list(zip(first_three, numbers_iter))
    [(0, 0), (1, 1), (2, 2)]
    >>> list(zip(remaining, numbers_iter))
    [(3, 3), (4, 4), (5, 5), (6, 6)]
    ```
    Tham số đầu tiên của zip nên là đối tượng có số lượng các phần tử ít nhất.

---

### ▶ Loop variables leaking out!
<!-- Example ID: ccec7bf6-7679-4963-907a-1cd8587be9ea --->
1\.
```py
for x in range(7):
    if x == 6:
        print(x, ': for x inside loop')
print(x, ': x in global')
```

**Kết quả:**
```py
6 : for x inside loop
6 : x in global
```

Nhưng mà `x` chưa bao giờ được định nghĩa bên ngoài vòng lặp...
2\.
```py
# Lần này khởi tạo x trước
x = -1
for x in range(7):
    if x == 6:
        print(x, ': for x inside loop')
print(x, ': x in global')
```

**Kết quả:**
```py
6 : for x inside loop
6 : x in global
```

3\.

**Kết quả (Python 2.x):**
```py
>>> x = 1
>>> print([x for x in range(5)])
[0, 1, 2, 3, 4]
>>> print(x)
4
```

**Kết quả (Python 3.x):**
```py
>>> x = 1
>>> print([x for x in range(5)])
[0, 1, 2, 3, 4]
>>> print(x)
1
```

#### 💡 Giải thích:

- In Python, for-loops use the scope they exist in and leave their defined loop-variable behind. This also applies if we explicitly defined the for-loop variable in the global namespace before. In this case, it will rebind the existing variable.

- Trong Python, vòng lặp for sử dụng 
- The differences in the output of Python 2.x and Python 3.x interpreters for list comprehension example can be explained by following change documented in [What’s New In Python 3.0](https://docs.python.org/3/whatsnew/3.0.html) changelog:

    > "List comprehensions no longer support the syntactic form `[... for var in item1, item2, ...]`. Use `[... for var in (item1, item2, ...)]` instead. Also, note that list comprehensions have different semantics: they are closer to syntactic sugar for a generator expression inside a `list()` constructor, and in particular, the loop control variables are no longer leaked into the surrounding scope."

---

### ▶ Beware of default mutable arguments!
<!-- Example ID: 7d42dade-e20d-4a7b-9ed7-16fb58505fe9 --->

```py
def some_func(default_arg=[]):
    default_arg.append("some_string")
    return default_arg
```

**Kết quả:**
```py
>>> some_func()
['some_string']
>>> some_func()
['some_string', 'some_string']
>>> some_func([])
['some_string']
>>> some_func()
['some_string', 'some_string', 'some_string']
```

#### 💡 Giải thích:

- Các tham số mặc định có kiểu giá trị thay đổi được (mutable) của các hàm trong Python không thực sự được khởi tạo mỗi lần ta gọi hàm. Thay vào đó giá trị trị mới được gán cho chúng được sử dụng với vai trò  giá trị mặc định. Khi ta truyền vào hàm `some_func` giá trị `[]`, giá trị mặc định của biến `default_arg` không được sử dụng, do đó hàm trả về kết quả như  mong đợi

    ```py
    def some_func(default_arg=[]):
        default_arg.append("some_string")
        return default_arg
    ```

    **Kết quả:**
    ```py
    >>> some_func.__defaults__ # Thuộc tính này sẽ cho ta thấy các giá trị mặc định của tham số truyền vào hàm 
    ([],)
    >>> some_func()
    >>> some_func.__defaults__
    (['some_string'],)
    >>> some_func()
    >>> some_func.__defaults__
    (['some_string', 'some_string'],)
    >>> some_func([])
    >>> some_func.__defaults__
    (['some_string', 'some_string'],)
    ```

- Để tránh các bugs liên quan tới các tham số có thể thay đổi giá trị, ta có thể gán cho chúng giá trị mặc định là `None` và sau đó viết mã kiểm tra xem giá trị truyền vào hàm có tương ứng với tham số đó hay không. Ví dụ:

    ```py
    def some_func(default_arg=None):
        if default_arg is None:
            default_arg = []
        default_arg.append("some_string")
        return default_arg
    ```

---

### ▶ Catching the Exceptions
<!-- Example ID: b5ca5e6a-47b9-4f69-9375-cda0f8c6755d --->
```py
some_list = [1, 2, 3]
try:
    # Câu lệnh sau sẽ gây ra ngoại lệ ``IndexError``
    print(some_list[4])
except IndexError, ValueError:
    print("Caught!")

try:
    # Câu lệnh sau sẽ gây ra ngoại lệ ``ValueError``
    some_list.remove(4)
except IndexError, ValueError:
    print("Caught again!")
```

**Output (Python 2.x):**
```py
Caught!

ValueError: list.remove(x): x not in list
```

**Output (Python 3.x):**
```py
  File "<input>", line 3
    except IndexError, ValueError:
                     ^
SyntaxError: invalid syntax
```

#### 💡 Giải thích

* Để thêm nhiều ngoại lệ trên cùng một dòng except, bạn cần truyền vào một tuple với các ngoại lệ được liệt kê bên trong hai dấu ngoặc đơn. Ví dụ,
  ```py
  some_list = [1, 2, 3]
  try:
     # This should raise a ``ValueError``
     some_list.remove(4)
  except (IndexError, ValueError), e:
     print("Caught again!")
     print(e)
  ```
  **Output (Python 2.x):**
  ```
  Caught again!
  list.remove(x): x not in list
  ```
  **Output (Python 3.x):**
  ```py
    File "<input>", line 4
      except (IndexError, ValueError), e:
                                       ^
  IndentationError: unindent does not match any outer indentation level
  ```

* Separating the exception from the variable with a comma is deprecated and does not work in Python 3; the correct way is to use `as`. Example,
* Tách biệt ngoại lệ với biến dùng dấu phẩy đã khôn còn được áp dụng nữa và khi viết như vậy thi code sẽ không chạy trong Python 3; Cách làm đúng là sử dụng `as`. Ví dụ, 
  ```py
  some_list = [1, 2, 3]
  try:
      some_list.remove(4)

  except (IndexError, ValueError) as e:
      print("Caught again!")
      print(e)
  ```
  **Kết quả:**
  ```
  Caught again!
  list.remove(x): x not in list
  ```

---

### ▶ Same operands, different story!
<!-- Example ID: ca052cdf-dd2d-4105-b936-65c28adc18a0 --->
1\.
```py
a = [1, 2, 3, 4]
b = a
a = a + [5, 6, 7, 8]
```

**Kết quả:**
```py
>>> a
[1, 2, 3, 4, 5, 6, 7, 8]
>>> b
[1, 2, 3, 4]
```

2\.
```py
a = [1, 2, 3, 4]
b = a
a += [5, 6, 7, 8]
```

**Kết quả:**
```py
>>> a
[1, 2, 3, 4, 5, 6, 7, 8]
>>> b
[1, 2, 3, 4, 5, 6, 7, 8]
```

#### 💡 Giải thích:

* `a += b` không phải luôn luôn cho ra kết quả giống như `a = a + b`. Các lơp *có thể* triển khai phép *`op=`* khác nhau.

* Biểu diễn `a = a + [5,6,7,8]` sinh ra một danh sách mới và tham chiếu của `a` trỏ tới danh sách mới, và để cho `b` không đổi.
* Biển diễn `a += [5,6,7,8]` thực sự tương đương vơi hàm "mở rộng" áp dụng cho danh sách ơ đó `a` và `b` vẫn trỏ về cùng một danh sách đã được thay đổi ngay tại chỗ.

---

### ▶ Name resolution ignoring class scope
<!-- Example ID: 03f73d96-151c-4929-b0a8-f74430788324 --->
1\.
```py
x = 5
class SomeClass:
    x = 17
    y = (x for i in range(10))
```

**Kết quả:**
```py
>>> list(SomeClass.y)[0]
5
```

2\.
```py
x = 5
class SomeClass:
    x = 17
    y = [x for i in range(10)]
```

**Kết quả (Python 2.x):**
```py
>>> SomeClass.y[0]
17
```

**Kết quả (Python 3.x):**
```py
>>> SomeClass.y[0]
5
```

#### 💡 Giải thích
- Các phạm vi được lồng bên trong định nghĩa của lớp lờ đi các tên (biến) được khai báo ở mức lớp (biến gán với lớp)
- Biễn diễn bộ sinh (generator) có phạm vi riêng của chúng
- Bắt đầu từ Python 3.X, các list comprehensions cũng có phạm riêng của chúng

---

### ▶ Needles in a Haystack *

<!-- Example ID: 52a199b1-989a-4b28-8910-dff562cebba9 --->

I haven't met even a single experience Pythonist till date who has not come across one or more of the following scenarios,
Tôi chưa bao giờ gặp một lập trình viên Python kinh nghiệm nào mà chưa gặp phải một trong những tình huống éo le dưới đây
1\.

```py
x, y = (0, 1) if True else None, None
```

**Kết :**

```py
>>> x, y  # expected (0, 1)
((0, 1), None)
```

2\.

```py
t = ('one', 'two')
for i in t:
    print(i)

t = ('one')
for i in t:
    print(i)

t = ()
print(t)
```

**Output:**

```py
one
two
o
n
e
tuple()
```

3\.

```
ten_words_list = [
    "some",
    "very",
    "big",
    "list",
    "that"
    "consists",
    "of",
    "exactly",
    "ten",
    "words"
]
```

**Output**

```py
>>> len(ten_words_list)
9
```

4\. Not asserting strongly enough

```py
a = "python"
b = "javascript"
```

**Output:**

```py
# An assert statement with an assertion failure message.
>>> assert(a == b, "Both languages are different")
# No AssertionError is raised
```

5\.

```py
some_list = [1, 2, 3]
some_dict = {
  "key_1": 1,
  "key_2": 2,
  "key_3": 3
}

some_list = some_list.append(4) 
some_dict = some_dict.update({"key_4": 4})
```

**Output:**

```py
>>> print(some_list)
None
>>> print(some_dict)
None
```

6\.

```py
def some_recursive_func(a):
    if a[0] == 0:
        return 
    a[0] -= 1
    some_recursive_func(a)
    return a

def similar_recursive_func(a):
        if a == 0:
                return a
        a -= 1
        similar_recursive_func(a)
        return a
```

**Output:**

```py
>>> some_recursive_func([5, 0])
[0, 0]
>>> similar_recursive_func(5)
4
```

#### 💡 Explanation:

* For 1, the correct statement for expected behavior is `x, y = (0, 1) if True else (None, None)`.

* For 2, the correct statement for expected behavior is `t = ('one',)` or `t = 'one',` (missing comma) otherwise the interpreter considers `t` to be a `str` and iterates over it character by character.

* `()` is a special token and denotes empty `tuple`.

* In 3, as you might have already figured out, there's a missing comma after 5th element (`"that"`) in the list. So by implicit string literal concatenation,

  ```py
  >>> ten_words_list
  ['some', 'very', 'big', 'list', 'thatconsists', 'of', 'exactly', 'ten', 'words']
  ```

* No `AssertionError` was raised in 4th snippet because instead of asserting the individual expression `a == b`, we're asserting entire tuple. The following snippet will clear things up,

  ```py
  >>> a = "python"
  >>> b = "javascript"
  >>> assert a == b
  Traceback (most recent call last):
      File "<stdin>", line 1, in <module>
  AssertionError
  
  >>> assert (a == b, "Values are not equal")
  <stdin>:1: SyntaxWarning: assertion is always true, perhaps remove parentheses?
  
  >>> assert a == b, "Values are not equal"
  Traceback (most recent call last):
      File "<stdin>", line 1, in <module>
  AssertionError: Values are not equal
  ```

* As for the fifth snippet, most methods that modify the items of sequence/mapping objects like `list.append`, `dict.update`, `list.sort`, etc. modify the objects in-place and return `None`. The rationale behind this is to improve performance by avoiding making a copy of the object if the operation can be done in-place (Referred from [here](http://docs.python.org/2/faq/design.html#why-doesn-t-list-sort-return-the-sorted-list)).

* Last one should be fairly obvious, mutable object (like `list`) can be altered in the function, and the reassignation of an immutable (`a -= 1`) is not an alteration of the value.

* Being aware of these nitpicks can save you hours of debugging effort in the long run. 

---


### ▶ Splitsies *
<!-- Example ID: ec3168ba-a81a-4482-afb0-691f1cc8d65a --->
```py
>>> 'a'.split()
['a']

# is same as
>>> 'a'.split(' ')
['a']

# but
>>> len(''.split())
0

# isn't the same as
>>> len(''.split(' '))
1
```

#### 💡 Explanation:

- It might appear at first that the default separator for split is a single space `' '`, but as per the [docs](https://docs.python.org/2.7/library/stdtypes.html#str.split)
    >  If sep is not specified or is `None`, a different splitting algorithm is applied: runs of consecutive whitespace are regarded as a single separator, and the result will contain no empty strings at the start or end if the string has leading or trailing whitespace. Consequently, splitting an empty string or a string consisting of just whitespace with a None separator returns `[]`.
    > If sep is given, consecutive delimiters are not grouped together and are deemed to delimit empty strings (for example, `'1,,2'.split(',')` returns `['1', '', '2']`). Splitting an empty string with a specified separator returns `['']`.
- Noticing how the leading and trailing whitespaces are handled in the following snippet will make things clear,
    ```py
    >>> ' a '.split(' ')
    ['', 'a', '']
    >>> ' a '.split()
    ['a']
    >>> ''.split(' ')
    ['']
    ```

---

### ▶ Wild imports *
<!-- Example ID: 83deb561-bd55-4461-bb5e-77dd7f411e1c --->
<!-- read-only -->

```py
# File: module.py

def some_weird_name_func_():
    print("works!")

def _another_weird_name_func():
    print("works!")

```

**Kết quả**

```py
>>> from module import *
>>> some_weird_name_func_()
"works!"
>>> _another_weird_name_func()
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name '_another_weird_name_func' is not defined
```

#### 💡 Giải thích:

- Chúng ta được khuyên là tránh sử dụng các wildcard imports. Vì với chúng, các tên (ví dụ hàm) với dấu gạch chân phía trước sẽ không được import. Điều này gây ra lỗi trong lúc code chạy
- Khi chúng ta dùng `from ... import a, b, c`, lỗi `NameError` sẽ khôn xảy ra nữa.
    ```py
    >>> from module import some_weird_name_func_, _another_weird_name_func
    >>> _another_weird_name_func()
    works!
    ```
- Nếu bạn thực sự muốn sử dụng wildcard imports, bạn se phải định nghĩa biến `__all__` trong module của bạn, biến này sẽ chưa một danh sách các đối tượng công cộng được import khi sử dụng wildcard imports.
    ```py
    __all__ = ['_another_weird_name_func']

    def some_weird_name_func_():
        print("works!")

    def _another_weird_name_func():
        print("works!")
    ```
    **Kết quả**

    ```py
    >>> _another_weird_name_func()
    "works!"
    >>> some_weird_name_func_()
    Traceback (most recent call last):
      File "<stdin>", line 1, in <module>
    NameError: name 'some_weird_name_func_' is not defined (hàm "some_weird_name_func_" không được định nghĩa)
    ```

---

### ▶ All sorted? *

<!-- Example ID: e5ff1eaf-8823-4738-b4ce-b73f7c9d5511 -->

```py
>>> x = 7, 8, 9
>>> sorted(x) == x
False
>>> sorted(x) == sorted(x)
True

>>> y = reversed(x)
>>> sorted(y) == sorted(y)
False
```

#### 💡 Explanation:

- The `sorted` method always returns a list, and comparing lists and tuples always returns `False` in Python. 

- ```py
  >>> [] == tuple()
  False
  >>> x = 7, 8, 9
  >>> type(x), type(sorted(x))
  (tuple, list)
  ```

- Unlike `sorted`, the `reversed` method returns an iterator. Why? Because sorting requires the iterator to be either modified in-place or use an extra container (a list), whereas reversing can simply work by iterating from the last index to the first.

- So during comparison `sorted(y) == sorted(y)`, the first call to `sorted()` will consume the iterator `y`, and the next call will just return an empty list.

  ```py
  >>> x = 7, 8, 9
  >>> y = reversed(x)
  >>> sorted(y), sorted(y)
  ([7, 8, 9], [])
  ```

---

### ▶ Midnight time doesn't exist?
<!-- Example ID: 1bce8294-5619-4d70-8ce3-fe0bade690d1 --->
```py
from datetime import datetime

midnight = datetime(2018, 1, 1, 0, 0)
midnight_time = midnight.time()

noon = datetime(2018, 1, 1, 12, 0)
noon_time = noon.time()

if midnight_time:
    print("Time at midnight is", midnight_time)

if noon_time:
    print("Time at noon is", noon_time)
```

**Output (< 3.5):**

```py
('Time at noon is', datetime.time(12, 0))
```
The midnight time is not printed.

#### 💡 Explanation:

Before Python 3.5, the boolean value for `datetime.time` object was considered to be `False` if it represented midnight in UTC. It is error-prone when using the `if obj:` syntax to check if the `obj` is null or some equivalent of "empty."

---
---



## Section: The Hidden treasures!

This section contains a few lesser-known and interesting things about Python that most beginners like me are unaware of (well, not anymore).

### ▶ Okay Python, Can you make me fly?
<!-- Example ID: a92f3645-1899-4d50-9721-0031be4aec3f --->
Well, here you go

```py
import antigravity
```

**Output:**
Sshh... It's a super-secret.

#### 💡 Explanation:
+ `antigravity` module is one of the few easter eggs released by Python developers.
+ `import antigravity` opens up a web browser pointing to the [classic XKCD comic](http://xkcd.com/353/) about Python.
+ Well, there's more to it. There's **another easter egg inside the easter egg**. If you look at the [code](https://github.com/python/cpython/blob/master/Lib/antigravity.py#L7-L17), there's a function defined that purports to implement the [XKCD's geohashing algorithm](https://xkcd.com/426/).

---

### ▶ `goto`, but why?
<!-- Example ID: 2aff961e-7fa5-4986-a18a-9e5894bd89fe --->

```py
from goto import goto, label
for i in range(9):
    for j in range(9):
        for k in range(9):
            print("I am trapped, please rescue!")
            if k == 2:
                goto .breakout # breaking out from a deeply nested loop
label .breakout
print("Freedom!")
```

**Output (Python 2.3):**
```py
I am trapped, please rescue!
I am trapped, please rescue!
Freedom!
```

#### 💡 Explanation:
- A working version of `goto` in Python was [announced](https://mail.python.org/pipermail/python-announce-list/2004-April/002982.html) as an April Fool's joke on 1st April 2004.
- Current versions of Python do not have this module.
- Although it works, but please don't use it. Here's the [reason](https://docs.python.org/3/faq/design.html#why-is-there-no-goto) to why `goto` is not present in Python.

---

### ▶ Brace yourself!
<!-- Example ID: 5c0c75f2-ddd9-4da3-ba49-c4be7ec39acf --->
If you are one of the people who doesn't like using whitespace in Python to denote scopes, you can use the C-style {} by importing,

```py
from __future__ import braces
```

**Output:**
```py
  File "some_file.py", line 1
    from __future__ import braces
SyntaxError: not a chance
```

Braces? No way! If you think that's disappointing, use Java. Okay, another surprising thing, can you find where's the `SyntaxError` raised in `__future__` module [code](https://github.com/python/cpython/blob/master/Lib/__future__.py)?

#### 💡 Explanation:
+ The `__future__` module is normally used to provide features from future versions of Python. The "future" in this specific context is however, ironic.
+ This is an easter egg concerned with the community's feelings on this issue.
+ The code is actually present [here](https://github.com/python/cpython/blob/025eb98dc0c1dc27404df6c544fc2944e0fa9f3a/Python/future.c#L49) in `future.c` file.
+ When the CPython compiler encounters a [future statement](https://docs.python.org/3.3/reference/simple_stmts.html#future-statements), it first runs the appropriate code in `future.c` before treating it as a normal import statement.

---

### ▶ Let's meet Friendly Language Uncle For Life
<!-- Example ID: 6427fae6-e959-462d-85da-ce4c94ce41be --->
**Output (Python 3.x)**
```py
>>> from __future__ import barry_as_FLUFL
>>> "Ruby" != "Python" # there's no doubt about it
  File "some_file.py", line 1
    "Ruby" != "Python"
              ^
SyntaxError: invalid syntax

>>> "Ruby" <> "Python"
True
```

There we go.

#### 💡 Explanation:
- This is relevant to [PEP-401](https://www.python.org/dev/peps/pep-0401/) released on April 1, 2009 (now you know, what it means).
- Quoting from the PEP-401
  
  > Recognized that the != inequality operator in Python 3.0 was a horrible, finger-pain inducing mistake, the FLUFL reinstates the <> diamond operator as the sole spelling.
- There were more things that Uncle Barry had to share in the PEP; you can read them [here](https://www.python.org/dev/peps/pep-0401/).
- It works well in an interactive environment, but it will raise a `SyntaxError` when you run via python file (see this [issue](https://github.com/satwikkansal/wtfpython/issues/94)). However, you can wrap the statement inside an `eval` or `compile` to get it working,
    ```py
    from __future__ import barry_as_FLUFL
    print(eval('"Ruby" <> "Python"'))
    ```

---

### ▶ Even Python understands that love is complicated
<!-- Example ID: b93cad9e-d341-45d1-999c-fcdce65bed25 --->
```py
import this
```

Nào, **this** là gì thế? `this` là tình yêu :heart:

**Kết quả:**
```
The Zen of Python, by Tim Peters

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!
```

`this` là Thiền của Python!

```py
>>> love = this
>>> this is love
True
>>> love is True
False
>>> love is False
False
>>> love is not True or False
True
>>> love is not True or False; love is love  # Tình yêu thật phức tạp
True
```

#### 💡 Giải thích:

* `this` module in Python is an easter egg for The Zen Of Python ([PEP 20](https://www.python.org/dev/peps/pep-0020)).
* Module `this` trong Python là một quả trứng phục sinh cho Thiền của Python
* And if you think that's already interesting enough, check out the implementation of [this.py](https://hg.python.org/cpython/file/c3896275c0f6/Lib/this.py). Interestingly, **the code for the Zen violates itself** (and that's probably the only place where this happens).
* Và nếu bạn thấy nó hứng thú, hãy xem mã triển khai của [this.py](https://hg.python.org/cpython/file/c3896275c0f6/Lib/this.py). Hấp dẫn thay, **mã của Thiền lại vi phạm chính quy tắc thiền**
* Nói về câu `love is not True or False; love is love`, mỉa mai thay câu nay tự thấy nó co nghĩa (nếu không, hay xnhinf cá ví dụ liên quan tới `is` và `is not`)
---

### ▶ Yes, it exists!
<!-- Example ID: 4286db3d-1ea7-47c9-8fb6-a9a04cac6e49 --->
** Khối `else` của các vòng lặp .** Dưới đây là một ví dụ điển hình:

```py
  def does_exists_num(l, to_find):
      for num in l:
          if num == to_find:
              print("Exists!")
              break
      else:
          print("Does not exist")
```

**Kết quả:**
```py
>>> some_list = [1, 2, 3, 4, 5]
>>> does_exists_num(some_list, 4)
Exists! (Tồn tại)
>>> does_exists_num(some_list, -1)
Does not exist (Không tồn tại)
```

**Khối `else` trong xử lý ngoại lệ.** Một ví dụ,

```py
try:
    pass
except:
    print("Exception occurred!!!")
else:
    print("Try block executed successfully...")
```

**Kết quả:**
```py
Try block executed successfully...
```

#### 💡 Giải thích:
- Khối `else` sau một vòng lặp được thực hiện chỉ khi trong quá trình lặp không có một `break` nào. Bạn có thể nghĩ nó như là một khối "không ngắt" ("nobreak")
- Khối `else` sau một khối try còn được gọi la "khối hoàn tất" đó khi các câu lệnh trong khối này sẽ được thực thi khi khối try hoàn thành trọn vẹn công việc của mình.

---
### ▶ Ellipsis *
<!-- Example ID: 969b7100-ab3d-4a7d-ad7d-a6be16181b2b --->
```py
def some_func():
    Ellipsis
```

**Output**
```py
>>> some_func()
# No output, No Error

>>> SomeRandomString
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'SomeRandomString' is not defined

>>> Ellipsis
Ellipsis
```

#### 💡 Explanation
- In Python, `Ellipsis` is a globally available built-in object which is equivalent to `...`.
    ```py
    >>> ...
    Ellipsis
    ```
- Eliipsis can be used for several purposes,
    + As a placeholder for code that hasn't been written yet (just like `pass` statement)
    + In slicing syntax to represent the full slices in remaining direction
    ```py
    >>> import numpy as np
    >>> three_dimensional_array = np.arange(8).reshape(2, 2, 2)
    array([
        [
            [0, 1],
            [2, 3]
        ],

        [
            [4, 5],
            [6, 7]
        ]
    ])
    ```
    So our `three_dimensional_array` is an array of array of arrays. Let's say we want to print the second element (index `1`) of all the innermost arrays, we can use Ellipsis to bypass all the preceding dimensions
    ```py
    >>> three_dimensional_array[:,:,1]
    array([[1, 3],
       [5, 7]])
    >>> three_dimensional_array[..., 1] # using Ellipsis.
    array([[1, 3],
       [5, 7]])
    ```
    Note: this will work for any number of dimensions. You can even select slice in first and last dimension and ignore the middle ones this way (`n_dimensional_array[firs_dim_slice, ..., last_dim_slice]`)
    + In [type hinting](https://docs.python.org/3/library/typing.html) to indicate only a part of the type (like `(Callable[..., int]` or `Tuple[str, ...]`))
    + You may also use Ellipsis as a default function argument (in the cases when you want to differentiate between the "no argument passed" and "None value passed" scenarios).

---

### ▶ Inpinity
<!-- Example ID: ff473ea8-a3b1-4876-a6f0-4378aff790c1 --->
The spelling is intended. Please, don't submit a patch for this.

**Output (Python 3.x):**
```py
>>> infinity = float('infinity')
>>> hash(infinity)
314159
>>> hash(float('-inf'))
-314159
```

#### 💡 Explanation:
- Hash of infinity is 10⁵ x π.
- Interestingly, the hash of `float('-inf')` is "-10⁵ x π" in Python 3, whereas "-10⁵ x e" in Python 2.

---

### ▶ Let's mangle
<!-- Example ID: 37146d2d-9e67-43a9-8729-3c17934b910c --->
1\.
```py
class Yo(object):
    def __init__(self):
        self.__honey = True
        self.bro = True
```

**Kết quả:**
```py
>>> Yo().bro
True
>>> Yo().__honey
AttributeError: 'Yo' object has no attribute '__honey' (Đối tượng 'Yo' không có thuộc tính '__honey')
>>> Yo()._Yo__honey
True
```

2\.
```py
class Yo(object):
    def __init__(self):
        # Let's try something symmetrical this time
        self.__honey__ = True
        self.bro = True
```

**Kết quả:**
```py
>>> Yo().bro
True

>>> Yo()._Yo__honey__
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
AttributeError: 'Yo' object has no attribute '_Yo__honey__' (Đối tượng 'Yo' không có thuộc tính '_Yo__honey__')
```

Tại sao `Yo()._Yo__honey` lại gây ra lỗi?

3\.

```py
_A__variable = "Some value"

class A(object):
    def some_func(self):
        return __variable # (biến này chưa được khởi tạo)
```

**Kết quả:**
```py
>>> A().__variable
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
AttributeError: 'A' object has no attribute '__variable' (Đối tượng 'A' không có thuộc tính '__variable')

>>> A().some_func()
'Some value'
```


#### 💡 Giải thích:

* [Name Mangling](https://en.wikipedia.org/wiki/Name_mangling) được sử dụng để tránh việc đụng độ về tên (names) giữa các không gian tên (namespaces).
* Trong Python, trình thông dịch thay đổi (mangles) tên của các thành viên của một lớp mà bắt đầu với `__` (hai dấu gạch chân liền nhau hay còn gọi là "dunder") và các tên không thúc với nhiều hơn một dấu gạch chân bằng việc thêm vào `_TênCủaLớp` vào trước đó
* Vì vậy, để truy cập vào thuộc tính `__honey` trong đoạn mã đầu tiên, bạn phải nối `_Yo` vào phía trước, để ngăn việc xung đột với thuộc tính có cùng tên trong lớp khác.
* Nhưng tại sao trong đoạn mã thứ hai mặc dù đã dung tên đúng nhưng ta vẫn không truy cập được vào thuộc tính? Bởi vì cách thức mangling này không áp dụng đối với các tên biến kết thúc với hai dấu gạch chân.
* Đoạn mã thứ ba cũng là kết quả của việc mangling. Tên `__variable` trong câu lệnh `return __variable` được chuyển thành `_A__variable`, và lại vô tình trùng với tên biến được khai báo phía bên ngoài
* Còn nữa, nếu tên bị mangle nhiều hơn 255 kí tự, việc cắt gọn tên sẽ diên ra.

---
---

## Section: Appearances are deceptive!

### ▶ Skipping lines?
<!-- Example ID: d50bbde1-fb9d-4735-9633-3444b9d2f417 --->
**Kết quả:**
```py
>>> value = 11
>>> valuе = 32
>>> value
11
```

Cái quái gì thế?

**Chú ý:** Để làm ra kết quả như trên bạn chỉ cần sao chếp các câu lệnh và dán nó vào file hay shell.

#### 💡 Giải thích

Some non-Western characters look identical to letters in the English alphabet but are considered distinct by the interpreter.
Một vài kí tự không phải là kí tự phương tây trông giống như các kí tự trong bảng chữ cái tiếng Anh nhưng lại được diễn giải khác bởi trình thông idhcj
```py
>>> ord('е') # Kí tự cyrillic 'e' (Ye)
1077
>>> ord('e') # Kí tự latin 'e', được sử dụng trong tiếng Anh và trên các bàn phím chuẩn
101
>>> 'е' == 'e'
False

>>> value = 42 # latin e
>>> valuе = 23 # cyrillic 'e', Python 2.x interpreter would raise a `SyntaxError` here
>>> value
42
```


Hàm tích hợp sẵn `ord()` trả về mã Unicode của một kí tự [code point](https://en.wikipedia.org/wiki/Code_point), và bạn có thể thấy các mã khác nhau cho kí tự  Cyrillic 'e' và kí tự Latin 'e' .

---

### ▶ Teleportation

<!-- Example ID: edafe923-0c20-4315-b6e1-0c31abfc38f5 --->

```py
# Cài đặt thư viên numpy sử dụng `pip install numpy` trước
import numpy as np

def energy_send(x):
    # Khởi tạo một mảng numpy
    np.array([float(x)])

def energy_receive():
    # Trả về một mang numpy rỗng
    return np.empty((), dtype=np.float).tolist()
```

**Kết quả:**
```py
>>> energy_send(123.456)
>>> energy_receive()
123.456
```

Có gì mới ở đây nào ?

#### 💡 Giải thích:

* Chú ý rằng mảng numpy được tạo trong hàm `energy_send` không có được trả vì, vì vậy không gian bộ nhớ được giải phóng.
* `numpy.empty()` trả về phần bộ nhơ tự do tiếp theo mà không khởi tạo lại nó. Phân bộ nhớ nay lại vô tình trung với phần bộ nhớ trước đó được giải phóng (thường xảy ra, nhưng không phải là luôn luôn)

---


### ▶ Well, something is fishy...
<!-- Example ID: cb6a37c5-74f7-44ca-b58c-3b902419b362 --->
```py
def square(x):
    """
    A simple function to calculate the square of a number by addition.
    """
    sum_so_far = 0
    for counter in range(x):
        sum_so_far = sum_so_far + x
  return sum_so_far
```

**Output (Python 2.x):**

```py
>>> square(10)
10
```

Shouldn't that be 100?

**Note:** If you're not able to reproduce this, try running the file [mixed_tabs_and_spaces.py](/mixed_tabs_and_spaces.py) via the shell.

#### 💡 Explanation

* **Don't mix tabs and spaces!** The character just preceding return is a "tab",  and the code is indented by multiple of "4 spaces" elsewhere in the example.
* This is how Python handles tabs:
  
  > First, tabs are replaced (from left to right) by one to eight spaces such that the total number of characters up to and including the replacement is a multiple of eight <...>
* So the "tab" at the last line of `square` function is replaced with eight spaces, and it gets into the loop.
* Python 3 is kind enough to throw an error for such cases automatically.

    **Output (Python 3.x):**
    ```py
    TabError: inconsistent use of tabs and spaces in indentation
    ```

---
---

## Section: Miscellaneous


### ▶ `+=` nhanh hơn
<!-- Example ID: bfd19c60-a807-4a26-9598-4912b86ddb36 --->

```py
# Sử dụng "+" để cộng 3 strings:
>>> timeit.timeit("s1 = s1 + s2 + s3", setup="s1 = ' ' * 100000; s2 = ' ' * 100000; s3 = ' ' * 100000", number=100)
0.25748300552368164
# Sử dụng "+=" để cộng 3 strings:
>>> timeit.timeit("s1 += s2 + s3", setup="s1 = ' ' * 100000; s2 = ' ' * 100000; s3 = ' ' * 100000", number=100)
0.012188911437988281
```

#### 💡 Giải thích:
+ `+=` nhanh hơn `+` khi nối nhiều hơn 2 strings bởi vì string đầu tiên (ví dụ, `s1` trong `s1 += s2 + s3`) không bị huỷ đi khi tạo ra chuỗi kết quả cuối cùng
---

### ▶ Let's make a giant string!
<!-- Example ID: c7a07424-63fe-4504-9842-8f3d334f28fc --->
```py
def add_string_with_plus(iters):
    s = ""
    for i in range(iters):
        s += "xyz"
    assert len(s) == 3*iters

def add_bytes_with_plus(iters):
    s = b""
    for i in range(iters):
        s += b"xyz"
    assert len(s) == 3*iters

def add_string_with_format(iters):
    fs = "{}"*iters
    s = fs.format(*(["xyz"]*iters))
    assert len(s) == 3*iters

def add_string_with_join(iters):
    l = []
    for i in range(iters):
        l.append("xyz")
    s = "".join(l)
    assert len(s) == 3*iters

def convert_list_to_string(l, iters):
    s = "".join(l)
    assert len(s) == 3*iters
```

**Kết quả:**

```py
# Executed in ipython shell using %timeit for better readability of results.
# You can also use the timeit module in normal python shell/scriptm=, example usage below
# timeit.timeit('add_string_with_plus(10000)', number=1000, globals=globals())

>>> NUM_ITERS = 1000
>>> %timeit -n1000 add_string_with_plus(NUM_ITERS)
124 µs ± 4.73 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
>>> %timeit -n1000 add_bytes_with_plus(NUM_ITERS)
211 µs ± 10.5 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)
>>> %timeit -n1000 add_string_with_format(NUM_ITERS)
61 µs ± 2.18 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)
>>> %timeit -n1000 add_string_with_join(NUM_ITERS)
117 µs ± 3.21 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)
>>> l = ["xyz"]*NUM_ITERS
>>> %timeit -n1000 convert_list_to_string(l, NUM_ITERS)
10.1 µs ± 1.06 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)
```

Let's increase the number of iterations by a factor of 10.

```py
>>> NUM_ITERS = 10000
>>> %timeit -n1000 add_string_with_plus(NUM_ITERS) # Linear increase in execution time
1.26 ms ± 76.8 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)
>>> %timeit -n1000 add_bytes_with_plus(NUM_ITERS) # Quadratic increase
6.82 ms ± 134 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)
>>> %timeit -n1000 add_string_with_format(NUM_ITERS) # Linear increase
645 µs ± 24.5 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)
>>> %timeit -n1000 add_string_with_join(NUM_ITERS) # Linear increase
1.17 ms ± 7.25 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)
>>> l = ["xyz"]*NUM_ITERS
>>> %timeit -n1000 convert_list_to_string(l, NUM_ITERS) # Linear increase
86.3 µs ± 2 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)
```

#### 💡 Explanation
- You can read more about [timeit](https://docs.python.org/3/library/timeit.html) or [%timeit](https://ipython.org/ipython-doc/dev/interactive/magics.html#magic-timeit) on these links. They are used to measure the execution time of code pieces.
- Don't use `+` for generating long strings — In Python, `str` is immutable, so the left and right strings have to be copied into the new string for every pair of concatenations. If you concatenate four strings of length 10, you'll be copying (10+10) + ((10+10)+10) + (((10+10)+10)+10) = 90 characters instead of just 40 characters. Things get quadratically worse as the number and size of the string increases (justified with the execution times of `add_bytes_with_plus` function)
- Therefore, it's advised to use `.format.` or `%` syntax (however, they are slightly slower than `+` for very short strings).
- Or better, if already you've contents available in the form of an iterable object, then use `''.join(iterable_object)` which is much faster.
- Unlike `add_bytes_with_plus` because of the `+=` optimizations discussed in the previous example, `add_string_with_plus` didn't show a quadratic increase in execution time. Had the statement been `s = s + "x" + "y" + "z"` instead of `s += "xyz"`, the increase would have been quadratic.
  ```py
  def add_string_with_plus(iters):
      s = ""
      for i in range(iters):
          s = s + "x" + "y" + "z"
      assert len(s) == 3*iters

  >>> %timeit -n100 add_string_with_plus(1000)
  388 µs ± 22.4 µs per loop (mean ± std. dev. of 7 runs, 1000 loops each)
  >>> %timeit -n100 add_string_with_plus(10000) # Quadratic increase in execution time
  9 ms ± 298 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
  ```
- So many ways to format and create a giant string are somewhat in contrast to the [Zen of Python](https://www.python.org/dev/peps/pep-0020/), according to which,
  
    > There should be one-- and preferably only one --obvious way to do it.

---

### ▶ Minor Ones *
<!-- Example ID: f885cb82-f1e4-4daa-9ff3-972b14cb1324 --->
* `join()` is a string operation instead of list operation. (sort of counter-intuitive at first usage)

  **💡 Explanation:** If `join()` is a method on a string, then it can operate on any iterable (list, tuple, iterators). If it were a method on a list, it'd have to be implemented separately by every type. Also, it doesn't make much sense to put a string-specific method on a generic `list` object API.
  
* Few weird looking but semantically correct statements:
  + `[] = ()` is a semantically correct statement (unpacking an empty `tuple` into an empty `list`)
  + `'a'[0][0][0][0][0]` is also a semantically correct statement as strings are [sequences](https://docs.python.org/3/glossary.html#term-sequence)(iterables supporting element access using integer indices) in Python.
  + `3 --0-- 5 == 8` and `--5 == 5` are both semantically correct statements and evaluate to `True`.

* Given that `a` is a number, `++a` and `--a` are both valid Python statements but don't behave the same way as compared with similar statements in languages like C, C++, or Java.
  ```py
  >>> a = 5
  >>> a
  5
  >>> ++a
  5
  >>> --a
  5
  ```

  **💡 Giải thích:**
  + There is no `++` operator in Python grammar. It is actually two `+` operators.
  + `++a` parses as `+(+a)` which translates to `a`. Similarly, the output of the statement `--a` can be justified.
  + This StackOverflow [thread](https://stackoverflow.com/questions/3654830/why-are-there-no-and-operators-in-python) discusses the rationale behind the absence of increment and decrement operators in Python.

* You must be aware of the Walrus operator in Python. But have you ever heard about *the space-invader operator*?
  ```py
  >>> a = 42
  >>> a -=- 1
  >>> a
  43
  ```
  It is used as an alternative incrementation operator, together with another one
  ```py
  >>> a +=+ 1
  >>> a
  >>> 44
  ```
  **💡 Explanation:** This prank comes from [Raymond Hettinger's tweet](https://twitter.com/raymondh/status/1131103570856632321?lang=en). The space invader operator is actually just a malformatted `a -= (-1)`. Which is equivalent to `a = a - (- 1)`. Similar for the `a += (+ 1)` case.
  
* Python has an undocumented [converse implication](https://en.wikipedia.org/wiki/Converse_implication) operator. 
     
     ```py
     >>> False ** False == True
     True
     >>> False ** True == False
     True
     >>> True ** False == True
     True
     >>> True ** True == True
     True
     ```

     **💡 Explanation:** If you replace `False` and `True` by 0 and 1 and do the maths, the truth table is equivalent to a converse implication operator. ([Source](https://github.com/cosmologicon/pywat/blob/master/explanation.md#the-undocumented-converse-implication-operator))
     
* Since we are talking operators, there's also `@` operator for matrix multiplication (don't worry, this time it's for real).

     ```py
     >>> import numpy as np
     >>> np.array([2, 2, 2]) @ np.array([7, 8, 8])
     46
     ```

     **💡 Explanation:** The `@` operator was added in Python 3.5 keeping the scientific community in mind. Any object can overload `__matmul__` magic method to define behavior for this operator.

* From Python 3.8 onwards you can use a typical f-string syntax like `f'{some_var=}` for quick debugging. Example,
    ```py
    >>> some_string = "wtfpython"
    >>> f'{some_string=}'
    "some_string='wtfpython'"
    ``` 

* Python uses 2 bytes for local variable storage in functions. In theory, this means that only 65536 variables can be defined in a function. However, python has a handy solution built in that can be used to store more than 2^16 variable names. The following code demonstrates what happens in the stack when more than 65536 local variables are defined (Warning: This code prints around 2^18 lines of text, so be prepared!):
     
     ```py
     import dis
    exec("""
    def f():
        """ + """
        """.join(["X" + str(x) + "=" + str(x) for x in range(65539)]))

    f()

    print(dis.dis(f))
    ```
     
* Multiple Python threads won't run your *Python code* concurrently (yes, you heard it right!). It may seem intuitive to spawn several threads and let them execute your Python code concurrently, but, because of the [Global Interpreter Lock](https://wiki.python.org/moin/GlobalInterpreterLock) in Python, all you're doing is making your threads execute on the same core turn by turn. Python threads are good for IO-bound tasks, but to achieve actual parallelization in Python for CPU-bound tasks, you might want to use the Python [multiprocessing](https://docs.python.org/2/library/multiprocessing.html) module.

* Sometimes, the `print` method might not print values immediately. For example,

     ```py
     # File some_file.py
     import time
     
     print("wtfpython", end="_")
     time.sleep(3)
     ```

     This will print the `wtfpython` after 3 seconds due to the `end` argument because the output buffer is flushed either after encountering `\n` or when the program finishes execution. We can force the buffer to flush by passing `flush=True` argument.

* List slicing with out of the bounds indices throws no errors
  ```py
  >>> some_list = [1, 2, 3, 4, 5]
  >>> some_list[111:]
  []
  ```

* Slicing an iterable not always creates a new object. For example,
    ```py
    >>> some_str = "wtfpython"
    >>> some_list = ['w', 't', 'f', 'p', 'y', 't', 'h', 'o', 'n']
    >>> some_list is some_list[:] # False expected because a new object is created.
    False
    >>> some_str is some_str[:] # True because strings are immutable, so making a new object is of not much use.
    True
    ```

* `int('١٢٣٤٥٦٧٨٩')` returns `123456789` in Python 3. In Python, Decimal characters include digit characters, and all characters that can be used to form decimal-radix numbers, e.g. U+0660, ARABIC-INDIC DIGIT ZERO. Here's an [interesting story](http://chris.improbable.org/2014/8/25/adventures-in-unicode-digits/) related to this behavior of Python.

* You can separate numeric literals with underscores (for better readability) from Python 3 onwards.

     ```py
     >>> six_million = 6_000_000
     >>> six_million
     6000000
     >>> hex_address = 0xF00D_CAFE
     >>> hex_address
     4027435774
     ```

* `'abc'.count('') == 4`. Here's an approximate implementation of `count` method, which would make the things more clear
  ```py
  def count(s, sub):
      result = 0
      for i in range(len(s) + 1 - len(sub)):
          result += (s[i:i + len(sub)] == sub)
      return result
  ```
  The behavior is due to the matching of empty substring(`''`) with slices of length 0 in the original string.

---
---

# Đóng góp

Bạn có thể đóng góp cho wtfpython theo những cách dưới đây

- Cho chúng tôi biết những ví dụ mới
- Dịch wtfpython sang các ngôn gnuwx khác (Xem tại [issues labeled translation](https://github.com/satwikkansal/wtfpython/issues?q=is%3Aissue+is%3Aopen+label%3Atranslation))
- Minor corrections like pointing out outdated snippets, typos, formatting errors, etc.
- Sửa các lỗi phụ khác như các đoạn mã bị lỗi thời, các lỗi cú pháp, lỗi định dạng, vân vân.
- Identifying gaps (things like inadequate explanation, redundant examples, etc.)
- Tìm những thiếu sót (ví dụ như giải thích chưa cặn kẽ, các ví dụ không cần thiết, vân vân.)
- Bất cứ đề xuất sáng tạo nào cũng làm cho wtfpython thú vị và hữu dụng hơn

Please see [CONTRIBUTING.md](/CONTRIBUTING.md) for more details. Feel free to create a new [issue](https://github.com/satwikkansal/wtfpython/issues/new) to discuss things.

PS: Please don't reach out with backlinking requests, no links will be added unless they're highly relevant to the project.

# Lời cám ơn

Ý tưởng và thiết kế của wtfpython lấy cảm hứng từ dự án tuyệt vời của Denys Dovhan's [wtfjs](https://github.com/denysdovhan/wtfjs). Cùng với đó là sự hỗ trợ tuyệt vời của những người yêu Python, giúp cho wtfpython có được như ngày hôm nay.

#### Một vài liên kết hay khác!
* https://www.youtube.com/watch?v=sH4XF6pKKmk
* https://www.reddit.com/r/Python/comments/3cu6ej/what_are_some_wtf_things_about_python
* https://sopython.com/wiki/Common_Gotchas_In_Python
* https://stackoverflow.com/questions/530530/python-2-x-gotchas-and-landmines
* https://stackoverflow.com/questions/1011431/common-pitfalls-in-python
* https://www.python.org/doc/humor/
* https://github.com/cosmologicon/pywat#the-undocumented-converse-implication-operator
* https://www.codementor.io/satwikkansal/python-practices-for-efficient-code-performance-memory-and-usability-aze6oiq65
* https://github.com/wemake-services/wemake-python-styleguide/search?q=wtfpython&type=Issues
* WFTPython discussion threads on [Hacker News](https://news.ycombinator.com/item?id=21862073) and [Reddit](https://www.reddit.com/r/programming/comments/edsh3q/what_the_fck_python_30_exploring_and/).

# 🎓 License

[![WTFPL 2.0][license-image]][license-url]

&copy; [Satwik Kansal](https://satwikkansal.xyz)

[license-url]: http://www.wtfpl.net
[license-image]: https://img.shields.io/badge/License-WTFPL%202.0-lightgrey.svg?style=flat-square

## Chia sẻ cho bạn bè!

Nếu bạn thích wtfpython, bạn có thể chia sẻ các liên kết dưới đây cho bạn bè,

[Twitter](https://twitter.com/intent/tweet?url=https://github.com/satwikkansal/wtfpython&text=If%20you%20really%20think%20you%20know%20Python,%20think%20once%20more!%20Check%20out%20wtfpython&hashtags=python,wtfpython) | [Linkedin](https://www.linkedin.com/shareArticle?url=https://github.com/satwikkansal&title=What%20the%20f*ck%20Python!&summary=If%20you%20really%20thing%20you%20know%20Python,%20think%20once%20more!) | [Facebook](https://www.facebook.com/dialog/share?app_id=536779657179021&display=page&href=https%3A%2F%2Fgithub.com%2Fsatwikkansal%2Fwtfpython&quote=If%20you%20really%20think%20you%20know%20Python%2C%20think%20once%20more!)  

## Bạn có cần bản pdf của wtf hay không?

I've received a few requests for the pdf (and epub) version of wtfpython. You can add your details [here](https://satwikkansal.xyz/wtfpython-pdf/) to get them as soon as they are finished.

Tôi nhận được một vài yêu cầu cho phiên bản pdf (và epub) của wtfpython. Nếu bạn muốn, bạn có thể thêm thông tin chi tiết của mình ở đây [here](https://satwikkansal.xyz/wtfpython-pdf/) để có phiên bản pdf sớm nhất.

**That's all folks!** For upcoming content like this, you can add your email [here](https://www.satwikkansal.xyz/content-like-wtfpython/).

*PS: On a sidenote, consider donating a dollar to [plant a tree](https://teamtrees.org/).*
