<template>
  <body>
    <div class="bg-color flex-col">
      <div class="rect-pos-o fluid"><div class="rectangle-o fluid"></div></div>

      <div>
        <h1>แพ็กเกจ</h1>
        <div class="card-container">
          <div class="card-box">
            <b-card
              img-src="../assets/overseas.png"
              img-alt="Image"
              img-top
              class="mx-auto card"
            >
              <b-col style="padding: 1.25rem">
                <h2>Overseas</h2>
                <p>
                  แพ็คเกจสำหรับนักเดินทางต่างประเทศที่รักความคล่องตัวผจญภัยไปไหน
                  ไม่ต้องกังวล
                </p>
              </b-col>
              <b-col style="padding: 1rem">
                <b-button
                  href="#"
                  class="select-btn"
                  style="float: right; margin-top: 2rem"
                  >เลือกแพ็กเกจนี้</b-button
                >
              </b-col>
            </b-card>

            <b-card
              img-src="../assets/family.png"
              img-alt="Image"
              img-top
              class="mx-auto"
            >
              <b-col style="padding: 1.25rem">
                <h2>Family</h2>
                <p>
                  แพ็คเกจสำหรับนักเดินทางต่างประเทศที่รักความคล่องตัวผจญภัยไปไหนไม่ต้องกังวล
                </p>
              </b-col>
              <b-col style="padding: 1rem">
                <b-button
                  href="#"
                  class="select-btn"
                  style="float: right; margin-top: 2rem"
                  >เลือกแพ็กเกจนี้</b-button
                >
              </b-col>
            </b-card>
          </div>
        </div>
      </div>

      <div class="rect-pos-y fluid"><div class="rectangle-y fluid"></div></div>
    </div>
  </body>
</template>

<script>
export default {
  name: "CardSection",
};
</script>

<style scoped>
.bg-color {
  background-color: #ffffff;
}
.flex-col {
  display: flex;
  flex-direction: row;
  align-content: center;
  justify-content: center;
}
h1 {
  margin-top: 6rem;
  margin-bottom: 4rem;
  text-align: center;
}
.card-container {
  display: flex;
  flex-direction: row;
  column-gap: 4rem;
  justify-content: center;
  align-items: center;
  margin-bottom: 7rem;
}
.card-box {
  display: grid;
  column-gap: 4rem;
  row-gap: 2rem;
  justify-content: center;
  grid-template-columns: repeat(1, minmax(0, 1fr));
}
.card {
  overflow: hidden;
  display: flex;
  flex-direction: column;
  max-width: 22.8125rem;
  height: 32.5rem;
  background-color: rgb(252, 252, 252);
  box-shadow: 0px 8px 20px rgba(0, 0, 0, 0.069);
  border-radius: 16px;
  border: none;
}
h2 {
  font-size: 24px;
}
p {
  margin-top: 1rem;
  font-size: 14px;
  color: #333333;
}
.select-btn {
  font-size: 14px;
  cursor: pointer;
  border: none;
  border-radius: 24px;
  padding: 0.8rem 1rem;
  background-color: #c60000;
  color: white;
  margin-top: 2rem;
  width: 10rem;
  align-items: flex-end;
}
.rect-pos-y {
  display: flex;
  justify-content: flex-end;
  align-items: flex-start;
  padding: 2rem;
}
.rectangle-y {
  display: flex;
  position: absolute;
  width: 15vh;
  height: 12vh;
  background: #ffcf00;
}
.rect-pos-o {
  display: flex;
  justify-content: flex-end;
  align-items: flex-end;
  padding: 2rem;
}
.rectangle-o {
  display: flex;
  position: absolute;
  width: 18vh;
  height: 20vh;
  background: #fdf2c3;
}
@media (min-width: 728px) {
  .card-box {
    row-gap: 2rem;
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }
}
</style>
