---
title: Oke, Apa Itu React? (Part 3)
layout: post
date: 2017-12-05 13:30
category: blog
author: imamassi
description: Perkenalan React
---

<p data-height="265" data-theme-id="0" data-slug-hash="EbMzBy" data-default-tab="result" data-user="imamassi" data-embed-version="2" data-pen-title="Apa Itu React? (Part 2 - Pen 2)" class="codepen">See the Pen <a href="https://codepen.io/imamassi/pen/EbMzBy/">Apa Itu React? (Part 2 - Pen 2)</a> by imamassi (<a href="https://codepen.io/imamassi">@imamassi</a>) on <a href="https://codepen.io">CodePen</a>.</p>
<script async src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

{% highlight jsx %}

class Youtubeku extends React.Component{
...
render(){
    return <div>
      <Youtube videoId={this.state.videoId} onReady={this._onReady} opts={this.state.opts}/><br/>
      <button onClick={this.play}>Play Video</button>
      <button onClick={this.pause}>Pause Video</button>
    </div>
  }
...
}
{% endhighlight %}

Dan terakhir, adalah kode panjang diatas. Saya membuat sebuah komponen `Youtubeku`  , yang berisi `komponen Youtube` dan dua button `Play video` dan `Pause video` . Silahkan jika anda ingin membaca isi tab Babel, namun anda tidak perlu memahami secara keseluruhan semuanya untuk sekarang :).

{% highlight jsx %}
ReactDOM.render(
  <div>
    <Youtubeku videoId="3P6DWAwwViU"/>
    <Youtubeku videoId="JKCBeDeVxkg"/>
  </div>,
  document.getElementById('root')
)
{% endhighlight %}

Dengan saya membuat sebuah komponen baru, saya dapat melakukan apapun yang saya inginkan ke komponen tersebut, dan saya dapat merender 2 komponen yang sama, hanya `videoId` yang berbeda.

<div class="breaker"></div>

Jelas, masih banyak contoh yang bisa saya berikan untuk menjelaskan mengenai apa itu React, tapi saya rasa seharusnya anda cukup paham dibalik layar React itu maksudnya dibuat untuk apa.

> React, secara singkat, adalah sebuah library untuk mengelola tampilan DOM. Seluruh kinerja dalam menampilkan elemen, diberikan ke React, dan kita membiarkan React yang bekerja dalam memikirkan apa yang harus tampil, bagaimana, dan kapan.