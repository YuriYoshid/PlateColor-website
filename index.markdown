---
layout: home
---

<div class="hero">
  <h1 class="hero-title">自炊をもっと楽しく</h1>
  <p class="hero-subtitle">PlateColorで、毎日の食事をカラフルに彩ろう</p>
</div>

<section class="features">
  <h2>PlateColorの特徴</h2>
  <div class="feature-grid">
    <div class="feature-item">
      <h3>食材管理</h3>
      <p>賢く食材を管理して、無駄なく使い切れます</p>
    </div>
    <div class="feature-item">
      <h3>レシピ提案</h3>
      <p>あなたの好みに合わせて、最適なレシピを提案</p>
    </div>
    <div class="feature-item">
      <h3>栄養バランス</h3>
      <p>毎日の食事の栄養バランスを可視化</p>
    </div>
  </div>
</section>

<section class="news">
  <div class="news-container">
    <h2>最新情報</h2>
    {% for post in site.posts limit:3 %}
      <div class="news-item">
        <span class="date">{{ post.date | date: "%Y-%m-%d" }}</span>
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      </div>
    {% endfor %}
  </div>
</section>