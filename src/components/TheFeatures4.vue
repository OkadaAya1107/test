<template>
  <section>
    <div class="container-box">
      <div class="container-2">
        <img src="/images/Group-11.png" alt="">
      </div>
      <div class="container-1">
        <div class="title-container">
          <div class="circle">
            <span>point</span>
            <span class="number">04.</span>
          </div>
          <div class="right">
            <img src="/images/image-31.png" alt="">
          </div>
          <div class="title">
            <h2>英語版みらいスタディ</h2>
          </div>
        </div>
        <p class="text">
          It is a long established fact that a reader will be distracted by the readable content of a page when looking
          at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as
          opposed to using 'Content here, content here',
        </p>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
img {
  display: flex;
  margin: auto;
}

section {
  padding: 100px 0 100px 0;
  height: auto;
  max-width: 100%;
}

.container-box {
  display: flex;
  margin: 0 auto;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}

.container-1 {
  width: 40%;
  padding-left: 40px;
}

.container-2 {
  width: 40%;
}

.container-2 img {
  max-width: 100%;
  height: auto;
}

.title-container {
  display: flex;
  align-items: center;
  gap: 16px;
}

.right img {
  width: 44px;
  height: 51px;
  top: 197px;
  left: 852px;
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

.title {
  padding: 40px 0;
  font-size: 24px;
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
    flex-direction: column-reverse;
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
    flex-direction: column-reverse;
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