---
title: Component dan Props (Part 1)
layout: post
date: 2017-12-06 16:26
category: blog
author: imamassi
description: Perkenalan React
---

Oke, sekarang anda sudah paham sedikit mengenai React dan fungsionalitasnya. Sekarang, kita akan belajar mengenai apa itu Component dan Properties.

<div class="breaker"></div>

<p data-height="265" data-theme-id="0" data-slug-hash="wpvJQR" data-default-tab="result" data-user="imamassi" data-embed-version="2" data-pen-title="Let's Get Started" class="codepen">See the Pen <a href="https://codepen.io/imamassi/pen/wpvJQR/">Let's Get Started</a> by imamassi (<a href="https://codepen.io/imamassi">@imamassi</a>) on <a href="https://codepen.io">CodePen</a>.</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

<figcaption class="caption">Hasil dari belajar Component dan Props</figcaption>

<div class="breaker"></div>

Oke, sebelum terjun, saya ingin agar anda membuat sebuah pen di [CodePen.io](http://codepen.io). Silahkan buka CodePen, dan di pojok kanan atas ada tombol 'Create' , klik, dan klik 'New Pen'.

![Codepen](/assets/images/lets-get-started/2017-12-12_202612.png)

Setelah itu, anda akan melihat tampilan seperti ini:

![a](\assets\images\lets-get-started\2017-12-12_214250.png)

Klik Settings, buka tab Javascript. Lalu, di multiple selection field Javascript Preprocessor, dari None, ubah menjadi Babel. Opsi ini yang akan membuat kita dapat menggunakan JSX di Pen kita.

![a](\assets\images\lets-get-started\2017-12-12_215908.png)

Lalu di Quick-Add, tambahkan React, dan ReactDOM untuk menambahkan kedua script tersebut ke pen kita:

![a](\assets\images\lets-get-started\2017-12-12_214931.png)

Pastikan script React berada diatas script ReactDOM

![a](\assets\images\lets-get-started\2017-12-12_215118.png)

Sekarang, kita bisa menaruh kode dibawah ini ke Pen kita:

Taruh di tab HTML

{% highlight html %}
<div id="root"></div>
{% endhighlight %}

Taruh di tab JSX

{% highlight JSX %}
ReactDOM.render(<p>Halo dunia!</p>, document.getElementById('root'))
{% endhighlight %}

Setelah itu, secara otomatis jendela preview akan menghasilkan tampilan dibawah:

![a](\assets\images\lets-get-started\2017-12-12_220517.png)

Dan selamat! Sekarang, kita telah memberikan elemen dengan ID `root` di HTML kita ke React secara keseluruhan untuk dirender sesuai kebutuhan, _your amazing future react applications start here_ :).