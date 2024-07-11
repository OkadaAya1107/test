<template>
  <section>
    <div class="box">
      <img class="logo" src="/images/image-24.png" alt="">
      <h2 class="subtitle">Features</h2>
      <p>教材の特徴</p>
    </div>

    <div class="container-box">
      <div class="container-1">
        <div class="title-container">
          <!-- サークル・ポイント -->
          <div class="circle">
            <span>point</span>
            <span class="number">01.</span>
          </div>

          <!-- ひらめきマーク -->
          <div class="right">
            <img src="/images/image-31.png" alt="">
          </div>

          <!-- タイトル -->
          <div class="title">
            <h2>144つのSTEP</h2>
          </div>
        </div>

        <!-- 説明 -->
        <p class="text">
          年少さん～高校生まで、継続して学べる豊富なプログラムを準備。［BRONZE～DIAMONDまで各36STEP、合計144STEP］習熟度に応じて自分のペースで進めることが可能で週1回～約50分程度で1STEPクリア。
        </p>
      </div>

      <div class="container-2">
        <img src="/images/Group-8.png" alt="">
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
.box {
  padding-left: 80px;
  padding-top: 40px;
  background-image: url('/images/image-24.png');
  background-size: contain;
  background-position: left;
  background-repeat: no-repeat;
}

.logo {
  margin-bottom: -16px;
}

.box h2 {
  font-size: 32px;
}

.box p {
  margin-top: -16px;
}

section {
  padding: 100px 0 100px 0;
  max-width: 100%;
  background-color: #f5f5f54d;
}

.container-1 {
  width: 40%;
  margin: 0 auto;
}

.container-2 {
  margin: 0 auto;
  margin-top: 40px;
}

.container-2 img {
  width: 800px;
  height: 202px;
  top: 285px;
  left: 720px;
}

.container-box {
  display: flex;
  margin: 0 auto;
}

.title-container {
  display: flex;
  align-items: center;
  gap: 16px;
}

.title {
  color: #005A9C;
}

.circle {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 50px;
  height: 50px;
  text-align: center;
  background-color: #005A9C;
  color: white;
  padding: 8px;
  border-radius: 50%;
  border: 2px dotted white;
}

.number {
  font-size: 24px;
}

.right img {
  width: 44px;
  height: 51px;
  top: 271px;
  left: 230px;
}

.title {
  padding: 40px 0 40px 0;
  font-size: 24px;
}

.subtitle {
  color: #005A9C;
}

.text {
  line-height: 2;
  word-wrap: break-word;
  overflow-wrap: break-word;
}

/* タブレット */
@media (min-width: 768px) and (max-width: 991px) {
  .container-1 {
    width: 90%;
  }

  .box {
    padding-left: 32px;
  }
}

/* モバイル */
@media (min-width: 576px) and (max-width: 767px) {
  .container-box {
    flex-direction: column;
    align-items: center;
  }

  .container-1,
  .container-2 {
    width: 100%;
    padding: 0 16px;
    box-sizing: border-box;
  }

  .container-2 img {
    max-width: 100%;
    height: auto;
  }

  .box {
    padding-left: 32px;
  }

  .text {
    width: 100%;
  }
}

/* モバイルミニ */
@media (max-width: 575px) {
  .container-box {
    flex-direction: column;
    align-items: center;
  }

  .container-1,
  .container-2 {
    width: 100%;
    padding: 0 16px;
    box-sizing: border-box;
  }

  .container-2 img {
    max-width: 100%;
    height: auto;
  }

  .box {
    padding-left: 32px;
  }

  .text {
    width: 100%;
  }
}
</style>
