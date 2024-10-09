<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body { 
      font-family: Arial, sans-serif; 
      background: linear-gradient(to right, #AAAAAA, #DDDDDD); /* 預設漸層背景 */
      color: #888;
      margin: 0; /* 移除預設邊距 */
      height: 100vh; /* 設置頁面高度 */
      overflow: hidden; /* 隱藏滾動條 */
      transition: background 0.5s ease; /* 平滑背景轉換 */
    }

    /* 主要容器 */
    .main-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin: 20px;
      height: 100%; /* 讓容器也填滿頁面 */
      justify-content: center;
    }

    /* 音樂播放器容器 */
    .audio-container {
      margin: 10px 0; /* 縮小上下邊距 */
    }

    /* 照片容器 */
    .photo-container {
      display: flex;
      justify-content: center;
      margin: 10px 0; /* 縮小上下邊距 */
    }

    /* 歌名和團名 */
    .song-info {
      font-size: 20px; /* 字體大小 */
      color: #222; /* 字體顏色 */
      margin: 4px 0; /* 調整間距 */
      text-align: center; /* 文字置中 */
      font-weight: bold; /* 設置為粗體 */
    }

    /* 歌詞容器 */
    .lyrics-container {
      margin: 20px auto;
      height: 165px;
      width: 80%;
      overflow-y: scroll;
      text-align: center;
    }

    .lyrics-container::-webkit-scrollbar {
      display: none; /* 隱藏滾動條 */
    }

    .lyrics-container {
      scrollbar-width: none; /* 隱藏 Firefox 的滾動條 */
    }

    .lyrics p {
      margin: 5px 0;
      font-size: 18px;
      line-height: 1.5;
      color: #888;
    }

    .lyrics p.active {
      color: #222;
      font-weight: bold;
    }

    .photo {
      width: 70%;
      border-radius: 10px;
    }
    
    /* 背景上傳按鈕樣式 */
    .upload-container {
      margin-top: 20px;
      text-align: center;
    }
  </style>
  <title>(G)I-DLE_Klaxon</title>
</head>
<body>
  <div class="main-container">
    <!-- 添加圖片 -->
    <div class="photo-container">
      <img src="https://lineimg.omusic.com.tw/img/album/7489404.jpg?v=20240708194140" alt="Song Image" class="photo">
    </div>
    
    <!-- 歌名和團名 -->
    <div class="song-info">Klaxon - (G)I-DLE</div>
    
    <!-- 第一首歌 -->
    <div class="audio-container">
      <audio id="audio1" controls>
        <source src="klaxon.mp3" type="audio/mp3">
      </audio>
    </div>

    <!-- 歌詞顯示區域 -->
    <div class="lyrics-container" id="lyrics-container1">
      <div class="lyrics" id="lyrics1">
        <p data-time="3.5">What time is it now?</p>
        <p data-time="7">Time to summer</p>
        <p data-time="9">mm... One two</p>
        <p data-time="10.5">좀 미친 소리 같지만 난 네게 반했어</p>
        <p data-time="15">(Uh-uh-ooh-whoa ~ ~ ~)</p>
        <p data-time="18">자꾸 눈으로 욕 하지마 더 네게 빠졌어</p>
        <p data-time="23">(Uh-uh-ooh-whoa ~ ~ ~ Yeah)</p>
        <p data-time="26.9">영화보다 멋진 드라마틱 romantic show</p>
        <p data-time="30.5">나 처음 본 순간 완전 영원한 반쪽인걸</p>
        <p data-time="34.5">또못본척 못들은척 넘어가려 하지 어림없어</p>
        <p data-time="38.5">차 떠나가라 소리칠 거야</p>
        <p data-time="41.5">I love you ~ baby ~ ~</p>
        <p data-time="45">야 나 좀 봐줘 lady ~ ~</p>
        <p data-time="49">더 hit the klaxon</p>
        <p data-time="50.5">Hon-hon-hon-hon-hon-honk</p>
        <p data-time="53">또 hit the klaxon</p>
        <p data-time="54.6">Hon-hon-hon-hon-hon-honk</p>
        <p data-time="57">Hey hop in sweetie boy</p>
        <p data-time="59">Ooh ~ ooh-ah ~ ooh ~ ~</p>
        <p data-time="64.5">Honk honk hit the klaxon</p>
        <p data-time="67">Ooh ~ ooh-ah ~ ooh ~ ~</p>
        <p data-time="72.8">Honk honk hit the klaxon</p>
        <p data-time="76.4">Yeah 오픈카 타고 드라이브는 어때</p>
        <p data-time="78.9">Wannabe by Spice Girls ~ 틀고 okay</p>
        <p data-time="80.8">야 딱 봐도 그 여자는 불건전해</p>
        <p data-time="82.7">그만 힐끔대고 벨트나 매 옆에</p>
        <p data-time="84.7">Pretty hot stuff hot stuff beautiful</p>
        <p data-time="86.7">But don't worry I don't want a boy toy</p>
        <p data-time="89">잠깐 갓길에 멈춰</p>
        <p data-time="90.5">깜빡이도 안 켜고 덮쳐</p>
        <p data-time="93">힙합보다 멋진 발라드틱 romantic show</p>
        <p data-time="96.5">너 처음 본 순간 완전 딱 천생연분인걸</p>
        <p data-time="100.8">또못본척 못들은척 넘어가려 하지 어림없어</p>
        <p data-time="104.6">차 떠나가라 소리칠 거야</p>
        <p data-time="107.3">I love you ~ baby ~ ~</p>
        <p data-time="110.9">야 나 좀 봐줘 lady ~ ~</p>
        <p data-time="115">더 hit the klaxon</p>
        <p data-time="116.8">Hon-hon-hon-hon-hon-honk</p>
        <p data-time="119">또 hit the klaxon</p>
        <p data-time="120.8">Hon-hon-hon-hon-hon-honk</p>
        <p data-time="123">Hey hop in sweetie boy</p>
        <p data-time="124.8">Hey I love you</p>
        <p data-time="126.5">I want to do interview</p>
        <p data-time="128.5">Ah yeah 난 너의</p>
        <p data-time="130.5">완벽한 the true lover</p>
        <p data-time="132.7">Hey I love you</p>
        <p data-time="134.7">I want to do interview</p>
        <p data-time="136.7">Ah yeah 난 너의</p>
        <p data-time="138.7">완벽한(the true lover)</p>
        <p data-time="139.3">I love you ~ baby ~ ~</p>
        <p data-time="143.5">야 나 좀 봐줘 lady ~ ~</p>
        <p data-time="147.5">Hit the klaxon</p>
        <p data-time="148.8">Hon-hon-hon-hon-hon-honk</p>
        <p data-time="151.2">또 hit the klaxon</p>
        <p data-time="152.8">Hon-hon-hon-hon-hon-honk</p>
        <p data-time="155.3">Hey hop in sweetie boy</p>
        <p data-time="156.9">Ooh ~ ooh-ah ~ ooh ~ ~</p>
        <p data-time="162.9">Honk honk hit the klaxon</p>
        <p data-time="165">Ooh ~ ooh-ah ~ ooh ~ ~</p>
        <p data-time="171">Honk honk hit the klaxon</p>
      </div>
    </div>

    <!-- 背景圖片上傳 -->
    <div class="upload-container">
      <label for="bgUpload">可以自訂背景呦</label>
      <input type="file" id="bgUpload" accept="image/*">
    </div>
  </div>

  <script>
    // 背景上傳處理邏輯
    const bgUpload = document.getElementById('bgUpload');
    bgUpload.addEventListener('change', function (event) {
      const file = event.target.files[0];
      if (file) {
        const reader = new FileReader();
        reader.onload = function (e) {
          document.body.style.backgroundImage = `url(${e.target.result})`;
          document.body.style.backgroundSize = 'cover';  // 背景圖片覆蓋整個頁面
          document.body.style.backgroundPosition = 'center';  // 圖片置中
          document.body.style.backgroundRepeat = 'no-repeat';  // 圖片不重複
        };
        reader.readAsDataURL(file); // 讀取上傳的圖片
      }
    });

    // 歌詞同步功能
    function syncLyrics(audio, lyricsElement, containerElement) {
      const lyrics = lyricsElement.getElementsByTagName('p');
      
      audio.addEventListener('timeupdate', () => {
        for (let i = 0; i < lyrics.length; i++) {
          const time = parseFloat(lyrics[i].getAttribute('data-time'));
          const nextTime = lyrics[i + 1] ? parseFloat(lyrics[i + 1].getAttribute('data-time')) : Infinity;

          if (audio.currentTime >= time && audio.currentTime < nextTime) {
            lyrics[i].classList.add('active'); // 當前歌詞變為活躍
            lyrics[i].scrollIntoView({ behavior: 'smooth', block: 'center' }); // 自動滾動並將當前歌詞居中
          } else {
            lyrics[i].classList.remove('active');
          }
        }
      });
    }

    // 對每首歌進行歌詞同步
    const audio1 = document.getElementById('audio1');
    const lyrics1 = document.getElementById('lyrics1');
    const container1 = document.getElementById('lyrics-container1');
    syncLyrics(audio1, lyrics1, container1);
  </script>

</body>
</html>
