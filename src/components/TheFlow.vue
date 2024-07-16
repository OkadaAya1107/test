<template>
     <section>
          <div class="container-1">
               <img src="/images/logo.png" alt="">
               <h2>Flow</h2>
               <p>ご契約の流れ</p>
          </div>

          <!-- ボックス -->
          <div class="outside-box">

               <!-- ボックス2 -->
               <div class="inside-box">
                    <img src="/images/Vector1.png" alt="">
                    <p>お問い合わせ</p>
               </div>

               <!-- 矢印 -->
               <div class="arrow">
                    <img src="/images/Polygon.png" alt="">
               </div>

               <!--  ボックス2 -->
               <div class="inside-box">
                    <img src="/images/Vector2.png" alt="">
                    <p>商品説明</p>
               </div>


               <!-- 矢印 -->
               <div class="arrow">
                    <img src="/images/Polygon.png" alt="">
               </div>

               <!--  ボックス3 -->
               <div class="inside-box">
                    <img src="/images/Vector3.png" alt="">
                    <p>お見積もり</p>
               </div>


               <!-- 矢印 -->
               <div class="arrow">
                    <img src="/images/Polygon.png" alt="">
               </div>

               <!--  ボックス4 -->
               <div class="inside-box">
                    <img src="/images/Vector4.png" alt="">
                    <p>お申し込み</p>
               </div>
               <!-- 矢印 -->
               <div class="arrow">
                    <img src="/images/Polygon.png" alt="">
               </div>

               <!--  ボックス5 -->
               <div class="inside-box">
                    <img src="/images/Vector5.png" alt="">
                    <p>導入</p>
               </div>

          </div>

          <p class="description">電話での問い合わせ希望の方は、052-756-3348（平日 10～18時）にご連絡ください。<br>
               商品説明は、販売元であるMILAIイノベーション株式会社の担当者にて実施いたします。</p>
     </section>
</template>

<script setup>

</script>

<style scoped>
section {
     background-color: #FBFBDF;
     height: auto;
     padding: 100px 0 100px 0;
     border-radius: 0 160px 0 0;
}

.container-1 {
     margin: 0 auto;
     text-align: center;
     padding-top: 16px;
}

.container-1 h2 {
     font-size: 36px;
     color: #005A9C;
}

.container-1 p {
     margin-top: -16px;
}

.outside-box {
     justify-content: center;
     padding-top: 60px;
     width: 90%;
     margin: 0 auto;
     display: flex;
     gap: 32px;
}

.inside-box {
     background-color: white;
     width: 10%;
     height: auto;
     text-align: center;
     padding: 16px;
}

.arrow {
     justify-content: center;
     align-items: center;
     display: flex;
}

.description {
     padding-top: 60px;
     text-align: center;
     line-height: 2;
}

/* モバイル時 */
@media (max-width: 767px) {
  .outside-box {
    flex-direction: column;
    align-items: center;
    gap: 16px;
  }

  .inside-box {
    width: 100%;
    max-width: 200px
  }

  .arrow {
    transform: rotate(90deg);
  }

  section {
    border-radius: 0;
    padding: 50px 0
  }

  .container-1 h2 {
    font-size: 28px;
  }

  .description {
    padding: 40px 20px 0;
    font-size: 14px;
  }
}
</style>