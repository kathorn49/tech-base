<template>
  <body>
    <div class="bg-color">
      <div class="main">
        <div class="mascot">
          <img src="../assets/ant-2.png" class="img-fluid" />
        </div>
        <div class="feature-container">
          <div class="feature-group">
            <div class="feature-box">
              <img src="../assets/price.png" />
              <div class="feature-content">
                <h5>ราคาเบาๆ</h5>
                <p>ความคุ้มครองครอบคลุม<br />ในราคาที่เหมาะสม</p>
              </div>
            </div>
            <div class="feature-box">
              <img src="../assets/callcenter.png" />
              <div class="feature-content">
                <h5>จัดเต็มทุกเส้นทาง</h5>
                <p>มีบริการช่วยเหลือฉุกเฉิน<br />พร้อมติดต่อได้ 24 ชั่วโมง</p>
              </div>
            </div>
          </div>
          <div class="feature-group">
            <div class="feature-box">
              <img src="../assets/hospital.png" />
              <div class="feature-content">
                <h5>ป่วยไม่กลัว</h5>
                <p>ความคุ้มครองครอบคลุม<br />ในราคาที่เหมาะสม</p>
              </div>
            </div>
            <div class="feature-box">
              <img src="../assets/insurance.png" />
              <div class="feature-content">
                <h5>มั่นใจ Jaadhai</h5>
                <p>รับประกันภัยโดย<br />บริษัท เอ็ม เอส ไอ จี ประกันภัย</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </body>
</template>

<script>
export default {
  name: "FeatureComponent",
};
</script>

<style scoped>
.bg-color {
  background-color: #fffae6;
}
.main {
  padding: 4rem 6rem 4rem 6rem;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-content: space-between;
}
.mascot {
  display: flex;
  padding-left: 18vh;
  padding-right: 2vh;
  padding-bottom: 3rem;
  justify-content: center;
  align-items: flex-end;
}
.feature-container {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap-reverse;
  column-gap: 5.625rem;
  padding: 3rem 0 3rem 0;
}
.feature-group {
  display: flex;
  flex-direction: column;
  row-gap: 5rem;
}
img {
  width: 7rem;
  height: auto;
}
.feature-box {
  display: flex;
  flex-direction: row;
  column-gap: 2rem;
  align-items: center;
}
.feature-content {
  margin-top: 3rem;
  display: flex;
  flex-direction: column;
}
h5 {
  font-size: 20px;
}
p {
  font-size: 14px;
  color: #777777;
}
@media (max-width: 1168px) {
  .mascot {
    padding-left: 0;
    padding-right: 6vh;
  }
  .feature-container {
    row-gap: 5rem;
  }
}
</style>
