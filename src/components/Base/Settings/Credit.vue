<template>
  <div class="credit">
    <perfect-scrollbar>
      <h1>クレジット</h1>
      <div class="section">
        <h2>制作</h2>
        <p>いっぺー</p>
      </div>
      <div class="section">
        <h2>使用素材</h2>
        <div class="item">
          <h3>画像</h3>
          <h4>Canva</h4>
          <ul class="list">
            <li><a target="_blank" rel="nofollow noopener" href="https://www.canva.com/photos/MADGv5rcu7M-woman-walking-in-the-street-during-night-time/">"夜の間に通りを歩いている女性"</a> | Aleksandar Pasaric 様</li>
            <li><a target="_blank" rel="nofollow noopener" href="https://www.canva.com/photos/MAEEWnGpeF8-man-looking-out-of-window/">"Man looking out of window"</a> | ozgurdonmaz 様</li>
            <li><a target="_blank" rel="nofollow noopener" href="https://www.canva.com/photos/MADesfDpSrk-phases-of-the-moon-moon-lunar-cycle-/">"月の満ち欠け。月の月の周期。"</a> | Allexxandar 様</li>
            <li><a target="_blank" rel="nofollow noopener" href="https://www.canva.com/photos/MADaAx-NWHE-milky-way-/">"天の川！"</a> | Sahil Malhotra 様</li>
            <li><a target="_blank" rel="nofollow noopener" href="https://www.canva.com/photos/MAC5MsKKatU-cat-on-the-moon-background/">"Cat on the moon background"</a> | ks2009q 様</li>
          </ul>
          <h4>Unsplash</h4>
          <ul class="list">
            <li><a target="_blank" rel="nofollow noopener" href="https://unsplash.com/photos/_b4ppn1Ssgw?utm_source=unsplash&utm_medium=referral&utm_content=creditShareLink">"Downtown Park, Bellevue, United States"</a> | Elisha Terada 様</li>
            <li><a target="_blank" rel="nofollow noopener" href="https://unsplash.com/photos/F-pSZO_jeE8?utm_source=unsplash&utm_medium=referral&utm_content=creditShareLink">"429 Cornelius Rd, Cerulean, KY 42215, USA, United States"</a> | Jongsun Lee 様</li>
            <li><a target="_blank" rel="nofollow noopener" href="https://unsplash.com/photos/NwDSEPXr9og?utm_source=unsplash&utm_medium=referral&utm_content=creditShareLink">"Downtown Bellevue at Night, Bellevue, United States"</a> | Dylan Mullins 様</li>
          </ul>
          <h4>写真AC</h4>
          <ul class="list">
            <li><a target="_blank" rel="nofollow noopener" href="https://www.photo-ac.com/main/detail/1828030?title=%E3%83%90%E3%83%BC%E3%82%AB%E3%82%A6%E3%83%B3%E3%82%BF%E3%83%BC&searchId=2565206629">"バーカウンター"</a> | 河童 様</li>
          </ul>
        </div>
        <div class="item">
          <h3>フォント</h3>
          <ul class="list">
            <li><a href="https://moji-waku.com/pigmo01/" target="_blank" rel="nofollow noopener">"ピグモ 01"</a> | もじワク研究 様</li>
            <li><a href="http://togoshi-font.osdn.jp/" target="_blank" rel="nofollow noopener">"戸越ゴシック"</a> | mshio 様</li>
          </ul>
        </div>
        <div class="item">
          <h3>BGM</h3>
          <ul class="list">
            <li><a href="https://soundcloud.com/xvahmbk5syft/p0owqmeiguu1" target="_blank" rel="nofollow noopener">"めうちきりんのメトロポリス"</a> | いっぺー</li>
          </ul>
        </div>
        <div class="item">
          <h3>SE</h3>
          <h4>Freesound</h4>
          <ul class="list">
            <li><a href="https://freesound.org/people/Zott820/sounds/209580/" target="_blank" rel="nofollow noopener">"Entrance Bell"</a> | Zott820 様</li>
            <li><a href="https://freesound.org/people/davidbain/sounds/136778/" target="_blank" rel="nofollow noopener">"Page Turn"</a> | davidbain 様</li>
            <li><a href="https://freesound.org/people/exterminat/sounds/164806/" target="_blank" rel="nofollow noopener">"Page turns and book close/open"</a> | exterminat 様</li>
          </ul>
        </div>
      </div>
      <div class="section">
        <h2>使用技術</h2>
        <div class="item">
          <h3>プログラミング言語</h3>
          <ul class="list">
            <li><a href="https://www.rust-lang.org/ja" target="_blank" rel="nofollow noopener">Rust</a></li>
            <li><a href="https://developer.mozilla.org/ja/docs/Web/JavaScript" target="_blank" rel="nofollow noopener">JavaScript</a></li>
          </ul>
        </div>
        <div class="item">
          <h3>フレームワーク</h3>
          <ul class="list">
            <li><a href="https://tauri.studio/" target="_blank" rel="nofollow noopener">tauri</a></li>
            <li><a href="https://vuejs.org/" target="_blank" rel="nofollow noopener">Vue.js</a></li>
          </ul>
        </div>
      </div>
    </perfect-scrollbar>
  </div>
</template>

<script>
export default {
  name: 'credit',
}
</script>

<style>
.credit .ps {
  height: 60vh;
}

.section {
  margin-bottom: 5rem;
}

  .section a {
    border-bottom: 1px dashed #fbfaf5;
  }

  .section h2 {
    display: inline-block;
    border-bottom: 2px solid #fbfaf5;
  }

  .section .item {
    margin-bottom: 5rem;
  }

    .item h3 {
      font-size: 2.4rem;
      margin-bottom: 1.2rem;
    }

    .item h3::before {
      content: '- ';
    }
    .item h3::after {
      content: ' -';
    }

    .item h4 {
      font-size: 2rem;
      margin: 1rem 0;
    }
  
  .list {
    font-size: 2rem;
  }

    .list li {
      margin-bottom: 1rem;
    }

      .list li > a {
        font-size: 2rem;
      }
</style>