<template>
<div class="conteiner">
  <div class="sfondo">
    <img src="../assets/img/14.png" alt="">
  </div>
<section class="conteiner-sito">
    <!-- conteiner titolo -->
    <div class="conteiner-title">
      <div class="title">
        <h1>Popular features that your business needs</h1>
        <p>
          Faff abaut a quid i don't want no agro bleeding chimney pot burke
          tosser cras nice one boot fanny!
        </p>
      </div>

      <!-- conteiner button -->
      <div class="cont-button">
        <button class="button-blue">Explore More Feature</button>
      </div>
    </div>
    <!-- conteiner card dinamiche -->
    <div class="conteiner-card">
      <!-- singole card -->
      <div class="card" v-for="(elem, index) in key_features" :key="index">
        <div>
          <h5>{{ elem.name }}</h5>
        </div>
        <div class="conteiner-img">
          <img class="icone" :src="`/img/${elem.img}`" alt="" />
        </div>
      </div>
    </div>
  </section>
</div>
  
</template>

<script>
export default {
  name: "section3Comp",
  props: {
    key_features: Array,
  },
};
</script>

<style lang="scss" scoped>
.conteiner{
  width: 100%;
  position: relative;
}
.sfondo{
    position: absolute;
    top:0;
    left: 0;
    z-index: -1;
    img{
      width: 54%;
    }
    
  }
.conteiner-card {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  margin-bottom: 130px;
}
.card {
  flex-basis: 23%;
  margin-bottom: 40px;
  padding: 15px 10px;
  box-shadow: 5px 5px 32px 7px #e2dcdc;
  border-radius: 5px;
}
.icone {
  width: 30%;
  margin: 10px 0;
}
h5 {
  margin-left: 10px;
  margin-top: 10px;
}

.button-blue {
  background-color: #377dff;
  border: 0;
  padding: 15px 20px;
  border-radius: 3px;
  color: white;
}

.conteiner-title {
  margin: 60px 0;
  display: flex;
  justify-content: space-between;
}

.title {
  flex-basis: 73%;
  p {
    margin-top: 30px;
    line-height: 20px;
    color: #8e989f;
    font-size: 14px;
    width: 60%;
  }
}
.cont-button {
  flex-basis: 23%;
}
.card:hover{
  background-color: #6cdac1;
  color: white;
  filter: brightness(110%);
  .icone{
    filter: invert(0.4);
}
}  
  
</style>