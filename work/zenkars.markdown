---
layout: post
title: Client Project - zenkars | Codebrahma
permalink: /work/zenkars/
---

## Zenkars

[zenkars.com](http://zenkars.com)

<div class="jcarousel-wrapper">
  <div class="jcarousel">
    <ul>
      <li><img src="/images/work/zenkars/homepage.png" width="700" height="400" alt=""></li>
      <li><img src="/images/work/zenkars/list.png" width="700" height="400" alt=""></li>
      <li><img src="/images/work/zenkars/profile.png" width="700" height="400" alt=""></li>
      <li><img src="/images/work/zenkars/desc.png" width="700" height="400" alt=""></li>
      <li><img src="/images/work/zenkars/4steps.png" width="700" height="400" alt=""></li>
      <li><img src="/images/work/zenkars/payment.png" width="700" height="400" alt=""></li>
    </ul>
  </div>

  <a href="#" class="jcarousel-control-prev" data-jcarouselcontrol="true" title="">‹</a>
  <a href="#" class="jcarousel-control-next" data-jcarouselcontrol="true" title="">›</a>
  <p class="jcarousel-pagination"> </p>
</div>


### Technology
Rails, Masonry, Rspec,  Faye, Bootstrap.

### Effort

10 months,  2 engineers

### About

Zenkars is the place to buy used cars.

It integrates with ARI, which is the inventory of the used cars in the US.

ARI has a legacy API. They use FTP, and send files for every change in the
inventory. This was pretty tricky.

So we TDD'd a very simple ARI wrapper to deal with this and open sourced it.
You can find it [here](https://github.com/Codebrahma/Ari-Fetch)
