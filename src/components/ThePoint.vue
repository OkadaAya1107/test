<template>
  <section>
    <div class="title">
      <img src="/images/image-9.png" class="left-image">
      <div class="title-content">
        <div class="company">
          <p>法人</p>
        </div>
        <div class="container-1">
          <h2>導入実績 <span class="number">50</span> 社以上</h2>
        </div>
      </div>
      <img src="/images/image-10.png"  class="right-image">
    </div>

    <div class="logo">
      <ul>
        <li v-for="image in images" :key="id">
          <img :src="image.src">
        </li>
      </ul>
    </div>

    <table class="info-table">
      <tr>
        <td class="label">契約法人数：</td>
        <td class="value">50社以上（2023年10月時点）</td>
      </tr>
      <tr>
        <td class="label">導入エリア：</td>
        <td class="value">
          北海道、宮城、東京、群馬、千葉、愛知<br>
          大阪、兵庫、岡山、広島、福岡
        </td>
      </tr>
      <tr>
        <td class="label">導入施設　：</td>
        <td class="value">
          学習塾、プログラミングスクール<br>
          学童保育施設（幼稚園・保育園等）
        </td>
      </tr>
    </table>

    <!-- メッセージ -->
    <div>
      <img class="message" src="/images/Group-12.png" alt="">
    </div>

    <!-- 導入のポイント -->
    <div>
      <img class="logo" src="/images/logo.png" alt="">
    </div>
    <div class="container-2">
      <img src="/images/image-31.png" alt="">
      <h2>導入のポイント</h2>
    </div>

    <!-- 3つのポイント -->
    <div class="point-container">

      <div class="point">
        <img src="/images/image-18.png" alt="">
        <div class="text-overlay">
          <h3>初期費用</h3>
          <h2>ゼロ</h2>
        </div>
        <p>
          It is a long established fact that a reader will be distracted by the readable content of a page when
          looking
          at its layout.
        </p>
      </div>

      <div class="point">
        <img src="/images/image-18.png" alt="">
        <div class="text-overlay">
          <h3>専門講師</h3>
          <h2>不要</h2>
        </div>
        <p>
          It is a long established fact that a reader will be distracted by the readable content of a page when
          looking
          at its layout.
        </p>
      </div>

      <div class="point">
        <img src="/images/image-18.png" alt="">
        <div class="text-overlay">
          <h3>サポート</h3>
          <h2>安心</h2>
        </div>
        <p>
          It is a long established fact that a reader will be distracted by the readable content of a page when
          looking
          at its layout.
        </p>
      </div>

    </div>

  </section>
</template>

<script setup>
import { ref } from "vue";

const images = ref([
  {
    id: 'a',
    src: 'images/image-13.png'
  },
  {
    id: 'b',
    src: 'images/image-11.png'
  },
  {
    id: 'c',
    src: 'images/image-12.png'
  },
  {
    id: 'd',
    src: 'images/image-14.png'
  },
]);

</script>

<style scoped>
section {
  height: 100vh;
}

.title {
  display: flex;
  margin: 0 auto;
  justify-content: center;
  margin-top: 60px;
}


.title-content {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0 20px;
}

.company {
  background-color: #005A9C;
  padding: 0px 24px;
  color: white;
  border-radius: 2px;
  font-size: 11px;
  margin-bottom: -24px;
  margin-right: auto;
  margin-left: 14px;
}

.container-1 h2 {
  margin: 0;
  text-align: center;
}

.container-2 {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 20px;
}

.container-2 h2 {
  color: #005A9C;
}

.container-2 img {
  width: 44px;
  height: 51px;
  top: 915px;
  left: 527px;
}

.number {
  font-size: 60px;
  color: #005A9C;
}

.left-image,
.right-image {
  max-height: 80px;
  width: auto;
}

.logo {
  max-width: 100%;
  display: flex;
  margin: 0 auto;
  margin-top: 40px;
  justify-content: center;
  overflow-x: auto;
  /* 横スクロールを許可 */
}

.logo ul {
  display: flex;
  list-style: none;
  padding: 0;
  margin: 0;
}

.logo li {
  margin: 0 10px;
}

.logo img {
  max-width: 100%;
  height: auto;
}

.info-table {
  width: 40%;
  border-collapse: collapse;
  margin: auto
}

.info-table .label::before {
  content: '';
  position: absolute;
  bottom: -1px;
  left: 0;
  width: 20%;
  /* one-third of the width */
  height: 2px;
  background-color: #005A9C;
  /* color */
}

.info-table .label::after {
  content: '';
  position: absolute;
  bottom: -1px;
  right: 0;
  width: 80%;
  /* two-thirds of the width */
  height: 2px;
  background-color: #ccc;
  /* default color */
}

.info-table tr {
  border-bottom: 1px solid #ccc;
  position: relative;
}

.info-table td {
  padding: 10px 5px;
  vertical-align: center;
}

.info-table .label {
  width: 120px;
  color: #005A9C;
  font-weight: bold;
}

.info-table .value {
  line-height: 1.8;
}

.message {
  width: 50%;
  display: flex;
  margin: 0 auto;
  margin-top: 40px;
}

.point-container {
  display: flex;
  justify-content: space-around;
  align-items: flex-start;
  width: 90%;
  margin-top: 72px;
  margin: auto;

}

.point {
  position: relative;
  text-align: center;
  max-width: 300px;
  margin: 0 auto;
  margin-top: 40px;
}

.point img {
  max-width: 100%;
}

.text-overlay {
  position: absolute;
  margin-top: -40px;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  width: 100%;
  box-sizing: border-box;
}

.text-overlay h3 {
  margin: 8px 0;
  color: #005A9C;
}

.text-overlay h2 {
  margin: 0;
  font-size: 24px;
  color: #005A9C;
}

.text-overlay p {
  font-size: 14px;
  line-height: 1.6;
}


/* タブレット */
@media (min-width: 768px) and (max-width: 991px) {
  .info-table {
    width: 90%;
    border-collapse: collapse;
    margin: auto
  }

  .message {
    width: 90%;
  }
}

/* モバイル */
@media (min-width: 576px) and (max-width: 767px) {
  .info-table {
    width: 90%;
    border-collapse: collapse;
    margin: auto
  }

  .message {
    width: 90%;
  }

  .point-container {
    flex-direction: column;
    align-items: center;
  }
}

/* モバイルミニ */
@media (max-width: 575px) {
  .info-table {
    width: 90%;
    border-collapse: collapse;
    margin: auto
  }

  .message {
    width: 90%;
  }

  .point-container {
    flex-direction: column;
    align-items: center;
  }
}
</style>