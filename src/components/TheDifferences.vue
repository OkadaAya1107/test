<template>
  <section>

    <div class="box">
      <img class="logo" src="/images/logo.png" alt="">
      <h2 class="subtitle">Differences</h2>
      <p>従来の教材との違い</p>
    </div>

    <div class="container-box">
      <div class="container-1">
        <div class="title">
          <h2>無学年方式を採用</h2>
        </div>
        <p class="text">
          従来の教材は対象学年ごとの作りとなっており、該当の問題を解いて覚えるものが主流でした。みらいスタディの教材は無学年方式を採用しているため、学年に関わらず学力・習熟度に応じたスタート位置から学習いただけます。
        </p>
      </div>

      <div class="container-2">
        <img src="/images/Rectangle-1.png">
      </div>
    </div>

  </section>
</template>
  

<style scoped>
.box {
  padding-left: 80px;
  padding-top: 40px;
  background-image: url('/images/image-24.png');
  background-size: contain;
  background-position: left bottom;
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
}

.container-1 {
  width: 40%;
  margin: 0 auto;
}

.container-2 {
  width: 40%;
  margin: 0 auto;
}


.container-box {
  display: flex;
  margin: 0 auto;
  background: url('/images/image-25.png');
  background-size: 400px;
  background-position: left 0px bottom -150px;
  background-repeat: no-repeat;
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
  }

  .container-1,
  .container-2 {
    width: 90%;
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
  }

  .container-1,
  .container-2 {
    width: 90%;
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


