<template>
  
  <section class="section">
    
      <div class="layout">
         <h2>Thoughts</h2>
        <p>開発者の想い</p>
      </div>

        <div class="container">
          <div class="title">
          <h2>自分で考えて、自分で解決する<br>
            力を身に着けていってほしい
          </h2>
        </div>

          <p class="text">
            今までの算数・数学は問題と解法の1体1の対応やパターンを暗記するものが主流でした。これではどこが重要なのか、自分で考え選択することが難しくなっています。
            <br>
            <br>
            学力の根幹である自分で考えて、自分で解決する力（思考力・解決力）を身に着けてほしい。覚えることはできるだけ少なくして、論理的思考で解決していくということを学び、それを使いこなせるように身につけていくために。
            <br>
            <br>
            そんな思いから開発された教材です。
          </p>
        </div>
  </section>
</template>

<script setup>
import { ref } from 'vue';


</script>

<style scoped>
.layout {
  padding-left: 80px;
  padding-top: 40px;
  background-image: url('/images/image-24.png');
  background-size: contain;
  background-position: left;
  background-repeat: no-repeat;
}

.layout h2 {
  font-size: 32px;
}

.layout p {
   margin-top: -16px;
}

section {
  background: linear-gradient(100deg, #005A9C 10%, #fff 100%), url('/images/image-22.png');
  height: 100vh;
  color: white;
  background-size: cover, 600px;
  background-position: center, right bottom;
  background-repeat: no-repeat, no-repeat;
  background-blend-mode: multiply;
}

.container {
  width: 40%;
  margin: 0 auto;
}

.title {
  padding: 40px 0 40px 0;
  font-size: 24px;
}

.text {
  line-height: 2;
}


/* タブレット */
@media (min-width: 768px) and (max-width: 991px) {
  .container {
    width: 90%;
  }

  .layout {
    padding-left: 32px;
  }
}

/* モバイル */
@media (min-width: 576px) and (max-width: 767px) {
  .container {
    width: 90%;
  }

  .layout {
    padding-left: 32px;
  }
}

/* モバイルミニ */
@media (max-width: 575px) {
  .container {
    width: 90%;
  }

  .layout {
    padding-left: 32px;
  }
}
</style>