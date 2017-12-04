---
title: Introduction
layout: post
date: 2017-12-02 17:42
category: blog
author: imamassi
description: Perkenalan React
---

Halo kawan-kawan,

Ingin belajar ReactJs?

---------

## Oke, apa itu React?

Sebelum saya menjelaskan hal tersebut, akan lebih baik mungkin saya memperlihatkan sedikit mengenai React :) (Mungkin akan membutuhkan waktu beberapa saat sebelum anda melihat CodePen dibawah)

<p data-height="265" data-theme-id="0" data-slug-hash="aVMBWv" data-default-tab="result" data-user="imamassi" data-embed-version="2" data-pen-title="Hello World in React" class="codepen">See the Pen <a href="https://codepen.io/imamassi/pen/aVMBWv/">Hello World in React</a> by imamassi (<a href="https://codepen.io/imamassi">@imamassi</a>) on <a href="https://codepen.io">CodePen</a>.</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

CodePen diatas sudah ditambahkan react.js (dari https://unpkg.com/react/umd/react.development.js) dan react-dom.js (dari https://unpkg.com/react-dom/umd/react-dom.development.js). ReactDOM ( `ReactDOM.render()` ) didapat dari react-dom.js .

Jika anda melihat tab HTML di CodePen diatas, maka kita akan melihat bahwa kita tidak akan melihat tulisan 'Hello, world!', 'Hello, world!' dirender dari kode Javascript (Tab Babel berisi JSX, Javascript, berbeda sedikit, akan dibahas sebentar lagi) kita.


{% highlight js %}

ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);

{% endhighlight %}

Diatas, secara sekilas kita dapat mengartikan bahwa `ReactDOM` mencari di dokumen HTML sebuah elemen dengan id `root`, lalu, ia mengubah elemen tersebut dengan elemen `h1` yang memiliki konten 'Hello, world!'.

> Dari sini, kita dapat melihat salah satu fitur React, kita dapat melempar sebuah elemen HTML ke React, dan React kelak akan memprosesnya lebih lanjut