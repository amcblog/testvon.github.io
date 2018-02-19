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

These are gallery tests for image wrapped in `<figure>` elements.

To place a gallery add the necessary YAML Front Matter:

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

And then drop-in the gallery include --- gallery `caption` is optional.

```liquid
{% raw %}{% include gallery caption="This is a sample gallery with **Markdown support**." %}{% endraw %}
```

{% include gallery caption="This is a sample gallery with **Markdown support**." %}

This is some text after the gallery just to make sure that everything aligns properly.

Here comes another gallery, this time set the `id` to match 2nd gallery hash in YAML Front Matter.

```yaml
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
```

And place it like so: 

```liquid
{% raw %}{% include gallery id="gallery2" caption="This is a second gallery example with images hosted externally." %}{% endraw %}
```

{% include gallery id="gallery2" caption="This is a second gallery example with images hosted externally." %}

And for giggles one more gallery just to make sure this works. To fill page content container add `class="full"`.

{% include gallery id="gallery3" class="full" caption="This is a third gallery example with two images and fills the entire content container." %}
