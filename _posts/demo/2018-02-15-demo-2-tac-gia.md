---
layout: single
#classes: wide
category: demo
author: test
permalink: /categories/demo/demo-2
tags: 
  - Demo
  - Tác giả   
title: "Demo 2: Cập nhật thông tin tác giả"
excerpt: "Trở thành 1 tác giả viết bài trên AMC's Blog" 
---
---
AMC's Blog được xây dựng dựa trên nền tảng Jekyll. Jekyll cung cấp cách lưu trữ dữ liệu bằng [data files](https://jekyllrb.com/docs/datafiles/), dựa vào đó ta có thể cập nhật và lưu trữ thông tin của nhiều tác giả khác nhau. AMC's Blog do vậy là 1 trang Blog hỗ trợ đa tác giả.

Nếu 1 tác giả mới đăng ký viết bài trên AMC's Blog, để cập nhật thông tin tác giả, ta làm theo các bước sau:

**Bước 1:**

Tạo và thêm vào file `_data/authors.yml` thông tin tác giả theo định dạng sau, lưu ý rằng mọi biến được sử dụng cho đối tượng `author:` trong file `_config.yml` đều có thể sử dụng (ví dụ: `name`, `avatar`, `bio`, `email`, `facebook`, ...)

```yaml
# /_data/authors.yml

von:
  name: "Von"
  uri: "https://iamvon.github.io"
  email: "tuanpm.amc@gmail.com"
  bio: "Code runs my life."
  avatar: "assets/img/admin.png"
  facebook: "this.is.von"

test:
  name: "Test"
  email: "test@gmail.com"
  bio: "Hi, i'm a Test"
  avatar: "assets/img/amc.png"
  facebook: "appliedmathclub"
```
**Bước 2:**

Để cập nhật thông tin tác giả cho một bài viết nào đó, ta khai báo tên của tác giả đó (tên đối tượng trong file `_data/authors.yml`) vào đoạn mã YAML cấu hình ở đầu bài viết đó:

```yaml
author: test
```

Như ví dụ trên đây ta đã cập nhật Test là tác giả của bài viết này.
