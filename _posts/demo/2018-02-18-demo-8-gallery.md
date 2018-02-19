---
layout: single
title: "Demo 8: Gallery"
excerpt: "" 
permalink: /categories/demo/demo-8
categories: demo
tags:
  - gallery
  - demo
gallery:
  - url: /images/demo-8/gallery-1.jpeg
    image_path: /images/demo-8/gallery-1.jpeg
    alt: "Ảnh 1"
    title: "Ảnh 1"
  - url: /images/demo-8/gallery-2.jpeg
    image_path: /images/demo-8/gallery-2.jpeg
    alt: "Ảnh 2"
    title: "Ảnh 2"
  - url: /images/demo-8/gallery-3.jpeg
    image_path: /images/demo-8/gallery-3.jpeg
    alt: "Ảnh 3"
    title: "Ảnh 3"
  - url: /images/demo-8/gallery-4.jpeg
    image_path: /images/demo-8/gallery-4.jpeg
    alt: "Ảnh 4"
    title: "Ảnh 4"
  - url: /images/demo-8/gallery-5.jpeg
    image_path: /images/demo-8/gallery-5.jpeg
    alt: "Ảnh 5"
    title: "Ảnh 5"
  - url: /images/demo-8/gallery-6.jpeg
    image_path: /images/demo-8/gallery-6.jpeg
    alt: "Ảnh 6"
    title: "Ảnh 6"
gallery2:
   - url: https://flic.kr/p/8a6Ven
     image_path: https://farm2.staticflickr.com/1272/4697500467_8294dac099_q.jpg
     alt: "Black and grays with a hint of green"
   - url: https://flic.kr/p/8a738X
     image_path: https://farm5.staticflickr.com/4029/4697523701_249e93ba23_q.jpg
     alt: "Made for open text placement"
   - url: https://flic.kr/p/8a6VXP
     image_path: https://farm5.staticflickr.com/4046/4697502929_72c612c636_q.jpg
     alt: "Fog in the trees"
gallery3:
  - image_path: /images/demo-8/gallery-3.jpeg
    alt: "Ảnh 1"
  - image_path: /images/demo-8/gallery-6.jpeg
    alt: "Ảnh 2"
---
Bài viết thử nghiệm tính năng đăng bộ sưu tập ảnh (gallery) trong phần tử `<figure>`.

Để đăng bộ sưu tập định dạng pop-up, ta thêm đoạn mã sau vào đoạn mã YAML cấu hình ở phần đầu bài viết:

```yaml
gallery:
  - url:         # URL của ảnh
    image_path:  # đường dẫn ảnh
    alt: ""      # Text thay thế nếu không load được ảnh
    title: ""    # Phụ đề ảnh 
```
Trên đây ta đã thêm vào 1 ảnh cho bộ sưu tập, vì bộ sưu tập bao gồm nhiều ảnh nên có thể thêm các ảnh khác vào theo cách tương tự. Dưới đây là 1 ví dụ:

```yaml
gallery:
  - url: /images/demo-8/gallery-1.jpeg
    image_path: /images/demo-8/gallery-1.jpeg
    alt: "Ảnh 1"
    title: "Ảnh 1"
  - url: /images/demo-8/gallery-2.jpeg
    image_path: /images/demo-8/gallery-2.jpeg
    alt: "Ảnh 2"
    title: "Ảnh 2"
  - url: /images/demo-8/gallery-3.jpeg
    image_path: /images/demo-8/gallery-3.jpeg
    alt: "Ảnh 3"
    title: "Ảnh 3"
```

Bạn cũng có thể thêm `caption` cho bộ sưu tập:

```liquid
{% raw %}{% include gallery caption="Caption có hỗ trợ **Markdown**." %}{% endraw %}
```

{% include gallery caption="Caption có hỗ trợ **Markdown**."" %}

