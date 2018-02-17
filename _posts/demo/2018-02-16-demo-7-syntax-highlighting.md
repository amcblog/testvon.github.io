---
layout: single
#classes: wide
category: demo
permalink: /categories/demo/demo-7
tags:
  - Demo 
  - syntax highlighting
title: "Demo 7: Syntax Highlighting"
excerpt: "Syntax Highlighting giúp code của bạn dễ đọc và dễ tìm lỗi hơn." 
---
---
Đoạn mã C++ được hiển thị có sử dụng syntax highlighting và đánh số dòng:
{% highlight cpp linenos %}
#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;

static const char chuoikytu [] =
"0123456789"
"abcdefghijklmnopqrstuvwxyz"
"ABCDEFGHIJKLMNOPQRSTUVWXYZ"
"!@#$%^&/?()_-+;:.|~×÷`" ;

int size = sizeof(chuoikytu) - 1;

int main()
{
    int length = 8;
    srand(time(0));
    for (int i = 0; i < length; i++)
    {
        cout << chuoikytu [rand() % size];
    }
    return 0;
}
{% endhighlight %}
