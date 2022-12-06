<template>
  <section>
    <!-- titolo testimonials -->
    <div class="testimonials title">
      <h2>Our Testimonials</h2>
      <p>
        if you are planning on developing a product landing app or website, take
        a look at this beautiful-crafted
      </p>
    </div>
    <div class="conteiner-bg-blu">
      <!-- conteiner card -->
      <div class="conteiner-card">
        <div class="card" v-for="(elem, index) in testimonials" :key="index">
          <!-- img card -->
          <div>
            <img :src="`/img/${elem.photo}`" alt="" />
          </div>

          <!-- testo card -->
          <div>
            <span>{{ elem.name }}</span>
            <span>{{ elem.firstname }}</span>
            <span class="role"> - {{ elem.role }}</span>
            <p>{{ elem.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "section4Comp",
  props: {
    testimonials: Array,
  },
};
</script>


<style lang="scss" scoped>
.testimonials {
  width: 100%;
  background-color: #f2fff7;
  background-image: url("../assets/img/15.png");
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  padding-bottom: 100px;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  h2 {
    width: 100%;
  }
}

.conteiner-bg-blu {
  width: 100%;
  background-color: #f2fff7;
  padding-bottom: 100px;
}
.conteiner-card {
  display: flex;
  justify-content: space-around;
  width: 80%;
  margin: 0 auto;
}
.card {
  flex-basis: 37%;
  padding: 15px;
  box-shadow: 0px 8px 22px 5px#eff1fe;
  background-color: #ffffff;
}

div {
  text-align: center;
  padding: 10px 0 20px 0;
  img {
    width: 15%;
    border-radius: 50%;
    border: 3px solid white;
  }
}
p {
  color: #8e989f;
  font-size: 10px;
  margin: 20px 0 2px 0;
  line-height: 20px;
  text-align: start;
}
span {
  font-size: 13px;
  font-weight: 700;
}
.role {
  color: #8e989f;
  font-size: 9px;
}
</style>