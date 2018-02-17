---
layout: single
classes: wide
category: demo
permalink: /categories/demo/demo-4
tags:
  - Demo 
  - math
  - công thức
  - MathJax
  - LaTeX
title: "Demo 4: Soạn thảo công thức toán học"
excerpt: "Công thức là 1 cách biểu diễn tường minh cho một vấn đề." 
---
---

Do là một trang Blog định hướng các bài viết chủ yếu thuộc chủ đề Toán học nên việc soạn thảo các công thức là một yêu cầu không thể thiếu. Dựa trên nhu cầu đó, AMC's Blog được tích hợp thêm tính năng soạn thảo các công thức Toán học bằng [MathJax engine](https://www.mathjax.org/), một công cụ giúp người viết soạn thảo các công thức với định dạng LaTeX, một định dạng được dùng phổ biến trong các tài liệu về khoa học kỹ thuật. Mọi công thức bạn viết ra sẽ luôn được đặt trong 2 dấu `$$`:

```latex
$$...$$
```

Dưới đây là 1 vài ví dụ về soạn thảo công thức bằng MathJax:

Khai triển chuỗi Taylor bậc n của hàm số $$f(x)$$ tại a :

$$ 
f(x)=\sum_{n=0}^{\infty}\frac{f^{(n)}(a)}{n!}(x-a)^n 
= f(a)+\frac{f^{'}(a)}{1!}(x-a)+\frac{f^{''}(a)}{2!}(x-a)^2+\frac{f^{'''}(a)}{3!}(x-a)^3+...
$$

```latex
# MathJax
$$ f(x)=\sum_{n=0}^{\infty}\frac{f^{(n)}(a)}{n!}(x-a)^n 
= f(a)+\frac{f^{'}(a)}{1!}(x-a)+\frac{f^{''}(a)}{2!}(x-a)^2+\frac{f^{'''}(a)}{3!}(x-a)^3+... 
$$
```

Khai triển chuỗi Maclaurin của hàm số $$e^x$$:`
$$ 
e^x=\sum_{n=0}^{\infty}\frac{x^n}{n!} 
= 1+\frac{x}{1!}+\frac{x^2}{2!}+\frac{x^3}{3!}+...
$$

```latex
# MathJax
$$ 
e^x=\sum_{n=0}^{\infty}\frac{x^n}{n!} 
= 1+\frac{x}{1!}+\frac{x^2}{2!}+\frac{x^3}{3!}+...
$$
```

Một nguyên hàm cơ bản:

$$ 
\int\frac{dx}{\sqrt{a^2-x^2}}=arcsin\frac{x}{|a|}+C 
$$

```latex
# MathJax
$$ 
\int\frac{dx}{\sqrt{a^2-x^2}}=arcsin\frac{x}{|a|}+C
$$
```

Một ma trận tham số:

$$
  \left[\begin{array}{rrr|r}
    x & y & z & 1   \\ 
    x & 2y & 3z & 6  \\ 
    3x & 2y & z &  6
  \end{array}\right]
$$

```latex
$$
  \left[\begin{array}{rrr|r}
    x & y & z & 1   \\ 
    x & 2y & 3z & 6  \\ 
    3x & 2y & z &  6
  \end{array}\right]
$$
```

Và còn nhiều cách soạn thảo công thức hơn nữa với MathJax. 

Có thể lúc này bạn đang cảm thấy hơi bối rối trước những điều trên, một phần có lẽ vì chưa biết về MathJax hoặc LaTeX trước đây, một phần có lẽ vì bạn chưa quen với việc viết những công thức Toán học bằng *"code"* như thế này, những thứ này quả thật khác xa với những công việc thường ngày của bạn. Có thể bạn không tin, nhưng đây chính là cách các nhà khoa học hay những kỹ sư hiện nay vẫn đang thường xuyên sử dụng để ghi chép những nghiên cứu, những tính toán thường ngày của họ. Hãy cứ thử làm quen với cách làm việc này, bạn sẽ khám phá ra nhiều điều thú vị và hữu ích.

Chắc chắn rằng sẽ rất khó khăn cho người mới bắt đầu, do vậy mình liệt kê một số tài liệu tham khảo cũng như công cụ giúp bạn làm quen dễ hơn với MathJax và LaTeX:

1. <https://math.meta.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference>. Đây là trang tham khảo giúp bạn học nhanh về cú pháp cũng như những ứng dụng của MathJax trong việc soạn thảo những công thức trong những chủ đề kiến thức khác nhau trong toán học.
2. <https://oeis.org/wiki/List_of_LaTeX_mathematical_symbols>. Đây là trang giúp bạn tra cứu cú pháp của những ký hiệu toán học được sử dụng trong LaTeX.
3. <https://www.codecogs.com/latex/eqneditor.php> và <http://www.sciweavers.org/free-online-latex-equation-editor>. Đây là 2 trang Web giúp bạn soạn thảo LaTeX online với nhiều ký hiệu và công thức được hỗ trợ. Mình rất khuyến khích các bạn mới bắt đầu sử dụng 2 trang này để soạn thảo công thức để giảm thiểu tối đa sai sót.
