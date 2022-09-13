<template>
  <body>
    <div class="bg-image">
      <div id="top-section">
        <div class="form-container">
          <b-form>
            <h1>จัดเต็มทุกการเดินทาง</h1>
            <div class="row">
              <div class="row-input">
                <div class="short-box">
                  <b-form-input type="text" placeholder="ต้นทาง" class="mb-2" />
                </div>
                <img src="../assets/arrow.png" width="15px" height="15px" />
                <div class="short-box">
                  <b-form-input
                    type="text"
                    placeholder="ปลายทาง"
                    class="mb-2"
                  />
                </div>
              </div>
            </div>
            <div class="row">
              <div class="row-input">
                <div class="short-box">
                  <b-form-input
                    type="text"
                    placeholder="วันที่ไป"
                    class="mb-2"
                    onfocus="(this.type = 'date')"
                  />
                </div>
                <div class="push"></div>
                <div class="short-box">
                  <b-form-input
                    type="text"
                    placeholder="วันที่กลับ"
                    class="mb-2"
                    onfocus="(this.type = 'date')"
                  />
                </div>
              </div>
            </div>
            <div class="row">
              <div class="long-box">
                <b-form-input type="text" placeholder="ประเภทการเดินทาง" />
              </div>
            </div>
            <div class="row">
              <div class="long-box">
                <b-form-input type="text" placeholder="จำนวนผู้เดินทาง" />
              </div>
            </div>
            <div class="row">
              <b-button class="check-btn">เช็คราคา</b-button>
            </div>
            <div class="row">
              <div class="row-input" style="column-gap: 2rem">
                <a href="#"><p>ขั้นตอนการซื้อ</p></a>
                <a href="#"><p>ข้อมูลผลิตภัณฑ์</p></a>
              </div>
            </div>
          </b-form>
        </div>
        <div>
          <img src="../assets/pic-1.png" id="vector" class="img-fluid" />
        </div>
      </div>
    </div>
  </body>
</template>

<script>
export default {
  name: "FormComponent",
};
</script>

<style scoped>
.bg-image {
  background: url("../assets/bg-3.png") no-repeat center center;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  min-height: 103vh;
}
#top-section {
  display: flex;
  flex-direction: row;
  column-gap: 4rem;
  justify-content: center;
  align-items: center;
  padding: 2rem;
  padding-bottom: 4rem;
}
.form-container {
  padding-bottom: 2rem;
}
form {
  display: flex;
  flex-direction: column;
  max-width: 37.25rem;
  max-height: 36.625rem;
  padding: 1.75rem;
  padding-left: 5.75rem;
  align-content: center;
  margin-left: 2rem;
  background: url("../assets/form-bg.svg");
}
.row {
  display: flex;
  margin-top: 0.75rem;
  align-items: center;
  justify-content: center;
}
.row-input {
  display: flex;
  flex-direction: row;
  grid-column-gap: 2rem;
  column-gap: 1rem;
  align-items: center;
  justify-content: center;
}
input {
  padding: 16px 15px 10px;
  margin-top: 0.75rem;
}
.check-btn {
  font-size: 14px;
  cursor: pointer;
  border: none;
  border-radius: 24px;
  padding: 0.8rem 1rem;
  background-color: #c60000;
  color: white;
  margin-top: 2rem;
  width: 30rem;
}
input[type="text"] {
  width: 32rem;
  border-radius: 15px;
  border: 1px solid #eeeeee;
  font-size: 13px;
  color: #777777;
}
input[type="date"] {
  width: 32rem;
  border-radius: 15px;
  border: 1px solid #eeeeee;
  font-size: 13px;
  color: #777777;
}
h1 {
  font-family: "Prompt", sans-serif;
  font-weight: normal;
  text-align: center;
  margin-top: 1.2rem;
  font-size: 30px;
}
img {
  margin-top: 1.2rem;
}
.push {
  margin-left: auto;
}
.short-box {
  display: flex;
  width: 13.25rem;
}
.long-box {
  display: flex;
  width: 32rem;
  margin-bottom: 0.5rem;
}
p {
  color: #00916e;
  text-decoration: underline;
}
#vector {
  max-height: 100vh;
  margin-top: 4rem;
}
</style>
