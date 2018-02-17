---
layout: single
#classes: wide
header:
  image: /images/demo-5.jpeg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
category: demo
permalink: /categories/demo/demo-5
tags:
  - Demo 
  - header
  - ảnh bìa
title: "Demo 5: Thêm ảnh bìa cho bài viết"
excerpt: "Ảnh bìa làm bài viết của bạn thêm sinh động và giúp truyền tải ý tưởng của bạn tốt hơn." 
---
---

Bài viết này có sử dụng ảnh bìa.

Để thêm ảnh bìa cho bài viết của mình, bạn thêm đối tượng `header` vào đoạn mã YAML trên đầu bài viết. Đối tượng `header` đó cần có thuộc tính con bắt buộc là `image` chứa đường dẫn tới file ảnh mà bạn muốn làm ảnh bìa.

```yaml
header:
  image:   # đường dẫn ảnh
```

Ví dụ bài viết này được thêm ảnh bằng đoạn mã YAML sau:

```yaml
header:
  image: /assets/images/unsplash-image-1.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
```

Bạn nên chọn ảnh bìa thể hiện được chủ đề của bài viết, điều này giúp bài viết của bạn có khả năng truyền tải tốt hơn.
