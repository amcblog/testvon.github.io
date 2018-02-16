---
layout: single
category: demo
permalink: /categories/demo/demo-1
tags: 
  - Demo
  - Cách đăng bài 
title: "Demo 1: Cách đăng bài trên Blog"
excerpt: "Cách đăng 1 bài viết đúng chuẩn định dạng Jekyll Blog" 
---

Các bài viết trên Blog được lưu trong thư mục `_posts/`, sau đó phân cấp theo các chủ đề: thư mục `_posts/theory` chứa các bài viết thuộc chủ đề **Toán lý thuyết**; thư mục `_posts/apply` chứa các bài viết thuộc chủ đề **Toán ứng dụng**; thư mục `_posts/sci-tech` là các bài viết thuộc chủ đề **Khoa học & Công nghệ**; cuối cùng thư mục `_posts/others` chứa các bài viết thuộc chủ đề **Chuyện bên lề**.

Tên của bài đăng phải lưu dưới định dạng sau: `NĂM-THÁNG-NGÀY-tiêu-đề.md` (tiếng Việt không dấu).
Trong đó `NĂM` là một số gồm 4 chữ số, `THÁNG` và `NGÀY` cả hai đều là số gồm 2 chữ số; `md` là đuôi mở rộng của file markdown.
Một số ví dụ về đặt tên đúng cách:

```
2018-02-15-demo-1.md
2018-02-16-demo-2.md
```

Trong file bài đăng, phần đầu của file cần cấu hình bằng YAML những mục dữ liệu cơ bản sau:

```YAML
---
layout: single     #  Mặc định bắt buộc 
category: demo   #  Chủ đề bài viết
title: "Demo 1: Cách đăng bài trên Blog"   # Tiêu đề bài viết
excerpt: "Cách đăng 1 bài viết đúng chuẩn định dạng Jekyll Blog"  # Giới thiệu/Trích đoạn bài viết (nên có)
---
```
