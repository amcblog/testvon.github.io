---
layout: single
#classes: wide
category: demo
permalink: /categories/demo/demo-9
tags:
  - Demo 
  - formatting
  - notice
title: "Demo 9: Một số loại bố cục văn bản"
excerpt: "Cách bố trí bài viết cũng là một yếu tố quan trọng." 
---
---
Bài viết có thể hiện tính năng trình bày 1 số loại bố cục cho văn bản giúp tăng khả năng truyền tải của bài viết.

**Thông báo:** Đây là 1 văn bản [thông báo](#) về một thông tin nào đó. Mong rằng thông báo này của chúng tôi sẽ giúp ích cho bạn đọc.
{: .notice}

**Một thông báo khác:** Đây là 1 văn bản [thông báo khác](#) về một thông tin nào đó. Mong rằng thông báo này của chúng tôi sẽ giúp ích cho bạn đọc.
{: .notice--primary}

**Thông tin thêm:** Đây là phần [thông tin thêm](#) tới bạn đọc về một chủ đề nào đó. Mong rằng phần thông tin thêm này của chúng tôi sẽ giúp ích cho bạn đọc.
{: .notice--info}

**Chú ý:** Đây là 1 văn bản [chú ý](#) bạn đọc về một thông tin nào đó. Mong rằng lời nhắc nhở này của chúng tôi sẽ giúp ích cho bạn đọc.
{: .notice--warning}

**Mẹo:** Đây là 1 văn bản cung cấp một [mẹo](#) nào đó cho bạn đọc về một chủ đề nào đó. Mong rằng mẹo chúng tôi cung cấp sẽ giúp ích cho bạn đọc.
{: .notice--success}

Bạn cũng có thể gộp nhiều đoạn văn bản vào trong một thông báo bằng cách sử dụng Liquid để capture nội dung và sau đó filter với markdownify:

```html
{% raw %}{% capture notice-2 %}
### Chú ý:

* Cảm ơn bạn đã chú ý đến chú ý này.
* Mong rằng chú ý này đã khiến bạn chú ý đến các chú ý khác.
{% endcapture %}{% endraw %}

<div class="notice">{% raw %}{{ notice-2 | markdownify }}{% endraw %}</div>
```
{% capture notice-2 %}
#### Chú ý:

* Cảm ơn bạn đã chú ý đến chú ý này.
* Mong rằng chú ý này đã khiến bạn chú ý đến các chú ý khác.
{% endcapture %}

<div class="notice">
  {{ notice-2 | markdownify }}
</div>
