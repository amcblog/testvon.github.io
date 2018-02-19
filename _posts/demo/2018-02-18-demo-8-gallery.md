---
layout: single
title: "Demo 8: Gallery"
excerpt: "Đăng bộ sưu tậm ảnh của bạn." 
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
  - url: https://unsplash.com/photos/6eCBRY8x3WM
    image_path: https://images.unsplash.com/photo-1496776574435-bf184935f729?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=d2735b09c03133aac6006a57388d7aa8&auto=format&fit=crop&w=750&q=80
    alt: "Leafs and light."
  - url: https://unsplash.com/photos/iHcKoB32NRI
    image_path: https://images.unsplash.com/photo-1501720073446-cb5ad67b48c4?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=b08d3cd9a19296b1d07597c70beb6ba4&auto=format&fit=crop&w=750&q=80
    alt: "Coconut and sky."
  - url: https://unsplash.com/photos/t8ts5bNQyWo
    image_path: https://images.unsplash.com/photo-1494008127121-feed7bf4f03c?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=67363b1526d00da2c7f76133918a3a3a&auto=format&fit=crop&w=750&q=80
    alt: "Cherry blossom"
gallery3:
  - image_path: /images/demo-8/gallery-3.jpeg
    alt: "Ảnh 1"
  - image_path: /images/demo-8/gallery-6.jpeg
    alt: "Ảnh 2"
---
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
{% include gallery caption="Caption có hỗ trợ **Markdown**." %}

Đây là một đoạn văn bản sau khi đăng xong bộ sưu tập để kiểm tra căn lề.

Đây là bộ sưu tập thứ hai, với định dạng ảnh đính kèm link ngoài:

```yaml
gallery2:
  - url: https://unsplash.com/photos/6eCBRY8x3WM
    image_path: https://images.unsplash.com/photo-1496776574435-bf184935f729?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=d2735b09c03133aac6006a57388d7aa8&auto=format&fit=crop&w=750&q=80
    alt: "Leafs and light."
  - url: https://unsplash.com/photos/iHcKoB32NRI
    image_path: https://images.unsplash.com/photo-1501720073446-cb5ad67b48c4?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=b08d3cd9a19296b1d07597c70beb6ba4&auto=format&fit=crop&w=750&q=80
    alt: "Coconut and sky."
  - url: https://unsplash.com/photos/t8ts5bNQyWo
    image_path: https://images.unsplash.com/photo-1494008127121-feed7bf4f03c?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=67363b1526d00da2c7f76133918a3a3a&auto=format&fit=crop&w=750&q=80
    alt: "Cherry blossom"
```

Sau khi cấu hình xong phần mã YAML, ta đăng bộ sưu tập, sử dụng thêm `id` để tham chiếu: 

```liquid
{% raw %}{% include gallery id="gallery2" caption="Bộ sưu tập với ảnh đính kèm link ngoài." %}{% endraw %}
```

{% include gallery id="gallery2" caption="Bộ sưu tập với ảnh đính kèm link ngoài." %}

Bộ sưu tập cuối (không pop-up) với ảnh phủ toàn bộ phần nội dung bằng cách thêm `class="full"`:

{% include gallery id="gallery3" class="full" caption="" %}
