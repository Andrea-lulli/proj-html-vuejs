<template>
  <!-- sezione 1 online marketing -->
  <section class="conteiner">
    <!-- img laterale six  -->
    <div class="card" v-for="(elem, index) in 3" :key="index">
      <div>
        <img src="../assets/img/24.png" alt="" />
      </div>

      <!-- testo online marketing -->
      <div>
        <h3>Online Marketing</h3>
        <p>it is a long estabilished fact that a reader will be distracted</p>
        <div>
          <ul>
            <li>
              <span>&#10003;</span>
              SEO
            </li>
            <li>
              <span>&#10003;</span>
              SEM
            </li>
            <li>
              <span>&#10003;</span>
              Website Strategy
            </li>
            <li>
              <span>&#10003;</span>
              Social management
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "section1Comp",
};
</script>

<style lang="scss" scoped>
.conteiner {
  width: 80%;
  margin: 0 auto;
  display: flex;
}
.card {
  flex-basis: 30%;
  display: flex;
  margin: 30px 0;
}

li {
  list-style: none;
  font-weight: 600;
  font-size: 14px;
  margin: 15px 0;
  span {
    color: #377dff;
    font-weight: 900;
  }
}
p {
  margin: 15px 0;
  line-height: 30px;
  color: #8e989f;
  font-size: 12px;
}

div {
  img {
    width: 80%;
    margin-top: 10px;
  }
}
</style>