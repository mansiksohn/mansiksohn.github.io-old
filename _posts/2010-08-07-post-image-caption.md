---
title: "Post: Image (Caption)"
categories: projects
tags:
  - image
  - Post Formats
featured_image: '/img/tools/Die Spring.jpg'
---

{% capture fig_img %}
![Foo]({{ '/assets/images/unsplash-gallery-image-3.jpg' | relative_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Photo from Unsplash.</figcaption>
</figure>
