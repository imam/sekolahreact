---
title: Oke, Apa Itu React? (Part 2)
layout: post
date: 2017-12-04 22:57
category: blog
author: imamassi
description: Perkenalan React
---

<p data-height="265" data-theme-id="0" data-slug-hash="OOqaJa" data-default-tab="result" data-user="imamassi" data-embed-version="2" data-pen-title="OOqaJa" class="codepen">See the Pen <a href="https://codepen.io/imamassi/pen/OOqaJa/">OOqaJa</a> by imamassi (<a href="https://codepen.io/imamassi">@imamassi</a>) on <a href="https://codepen.io">CodePen</a>.</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

Oke, diatas ini adalah contoh lain dari *keajaiban* React.

Diatas jika kita membuka tab Babel, kita melihat sebuah elemen `<Youtube />`, ini jelas bukan elemen HTML, melainkan elemen yang dibuat dengan menggunakan React. Kita menyebutnya sebagai sebuah komponen. (Komponen ini bukan komponen resmi React, ini adalah komponen yang didapat dari [https://github.com/compedit/react-youtube](https://github.com/compedit/react-youtube) dan saya koding agar dapat diproses di CodePen diatas).

{% highlight js %}

const youtubeopts = {
  width: '320',
  height: '',
  controls: 0
}

ReactDOM.render(
  <Youtube videoId="3P6DWAwwViU" opts={youtubeopts}/>,
  document.getElementById('root')
)

{% endhighlight %}

Jika kita lihat, React membuat kita lebih mudah dalam memasukkan video tersebut. Dibandingkan saya memasukkan kode embed yang panjang, saya tinggal menambahkan komponen yang telah dibuat oleh orang, memasukkan properti (sebutan atribut dalam komponen React) berupa `videoId` dan opts yang berisi opsi dalam Youtube playernya (Diatas saya membuat widthnya 320 pixel dan tanpa kontrol).