---
layout: article
title: Photo Gallery Demo
tags: [jekyll, gallery, lightgallery, justifiedgallery]

head-csss:
  - assets/lib/justifiedgallery/css/justifiedGallery.min.css
  - assets/lib/lightgallery/css/lightgallery.min.css
body-footer-scripts:
  - assets/lib/justifiedgallery/js/jquery.justifiedGallery.min.js
  - assets/lib/lightgallery/js/lightgallery-all.min.js
galleries:
  - id: dynamic-demo
    type: dynamic
    images:
      - thumbnail_url: assets/images/posts/photo-gallery-demo/dynamic-sample1-th.jpg
        url: assets/images/posts/photo-gallery-demo/dynamic-sample1.jpg
        html_content: Description 1
      - thumbnail_url: assets/images/posts/photo-gallery-demo/dynamic-sample2-th.jpg
        url: assets/images/posts/photo-gallery-demo/dynamic-sample2.jpg
  - id: thumbnail-demo
    type: thumbnails
    images:
      - thumbnail_url: assets/images/posts/photo-gallery-demo/thumbnail-sample1-th.jpg
        url: assets/images/posts/photo-gallery-demo/thumbnail-sample1.jpg
        html_content: Description 1
      - thumbnail_url: assets/images/posts/photo-gallery-demo/thumbnail-sample10-th.jpg
        url: assets/images/posts/photo-gallery-demo/thumbnail-sample10.jpg
        html_content: Description 2
      - thumbnail_url: assets/images/posts/photo-gallery-demo/thumbnail-sample11-th.jpg
        url: assets/images/posts/photo-gallery-demo/thumbnail-sample11.jpg
---

Demonstration for how this theme can include pictures in to a blog post or page.<!--more-->
This photo gallery utilizes [lightGallery](https://www.lightgalleryjs.com){:target="_blank"} for viewing photos and [Justified Gallery](http://miromannino.github.io/Justified-Gallery){:target="_blank"} for rendering thumbnails.

#### lightGallery - Dynamic Mode

[lightGallery dynamic mode demo](https://www.lightgalleryjs.com/demos/dynamic-mode){:target="_blank"}

<a class="pf-button-primary" href="#" id="dynamic-demo">Launch Gallery</a>

#### lightGallery - Thumbnails

[lightGallery thumbnails demo](https://www.lightgalleryjs.com/demos/thumbnails){:target="_blank"}

{% assign _gallery = page.galleries[1] %}
{% include snippets/components/gallery/thumbnails.html gallery=_gallery %}