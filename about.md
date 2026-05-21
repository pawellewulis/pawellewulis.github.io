---
layout: page
title: About
permalink: /about/
---

<style>
.about-box {
  display: flex;
  align-items: flex-start;
  gap: 28px;
  margin-top: 1.5em;
  padding: 24px;
  background: #f5f5f5;
  border-radius: 8px;
}

.about-photo {
  width: 200px;
  flex-shrink: 0;
}

.about-photo img {
  width: 100%;
  height: auto;
  display: block;
}

.about-text {
  flex: 1;
  min-width: 0;
}

@media screen and (max-width: 700px) {
  .about-box {
    gap: 16px;
    padding: 18px;
  }

  .about-photo {
    width: 105px;
  }

  .about-text {
    font-size: 1rem;
    line-height: 1.55;
  }
}
</style>

<div class="about-box">

  <div class="about-photo">
    <img src="/assets/img/profile/couch2.png" alt="">
  </div>

  <div class="about-text">
    <p>
      A while ago, I got a PhD in mathematics. I was hunting for prime numbers in funny patterns.
    </p>

    <p>
      I started this blog to cover some topics that don’t fully belong to academia or to my professional work. Enjoy!
    </p>

    <p>
      <strong>Contact:</strong><br>
      pavellevblog@gmail.com
    </p>
  </div>

</div>