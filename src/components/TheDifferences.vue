<template>
  <section class="content">
    <div class="text">
      <h1 class="title-1">Differences</h1>
      <p class="subtitle-1">従来の教材との違い</p>

      <div class="images-2">
        <h2 class="title-2">無学年方式を採用</h2>
        <p class="subtitle-2">従来の教材は対象学年ごとの作りとなっており、該当の問題を解いて覚えるものが主流でした。みらいスタディの教材は無学年方式を採用しているため、学年に関わらず学力・習熟度に応じたスタート位置から学習いただけます。</p>
      </div>
    </div>
    <div class="image-container">
      <img src="/images/image-26.png" class="images-1">
    </div>
  </section>
  </template>
  

<style scoped>
.content {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  padding: 40px 80px;
}

.text {
  line-height: 2;
  word-wrap: break-word;
  overflow-wrap: break-word;
}

.title-1 {
  font-size: 30px;
  color: #005A9C;
  margin-bottom: 20px;
}

.subtitle-1 {
  font-size: 18px;
  margin-bottom: 40px;
}

.title-2 {
  margin-bottom: 10px;
}

.subtitle-2 {
  font-family: YuGothic;
  font-size: 16px;
}

.image-container {
  flex-shrink: 0;
  width: 576px; 
  height: 500px;
}

.images-1 {
  width: 100%;
  height: auto;
  border-radius: 16px;
  background-repeat: no-repeat;
}

.images-2 {
  background-image: url('images/image-25.png');
  width: 480px;
  height: 600px;
  object-fit: cover; 
  background-repeat: no-repeat;
}
</style>


