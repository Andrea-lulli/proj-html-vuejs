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
      <div class="conteiner-card conteiner-sito">
        <div class="card">
          <!-- img card -->
          <div>
            <img :src="`/img/${testimonials[ind_dim].photo}`" alt="" />
          </div>

          <!-- testo card -->
          <div>
            <span>{{ testimonials[ind_dim].name }}</span>
            <span>{{ testimonials[ind_dim].firstname }}</span>
            <span class="role"> - {{ testimonials[ind_dim].role }}</span>
            <p>{{ testimonials[ind_dim].description }}</p>
          </div>
        </div>

        <div class="card">
          <!-- img card -->
          <div>
            <img :src="`/img/${testimonials[ind_dim1].photo}`" alt="" />
          </div>

          <!-- testo card -->
          <div>
            <span>{{ testimonials[ind_dim1].name }}</span>
            <span>{{ testimonials[ind_dim1].firstname }}</span>
            <span class="role"> - {{ testimonials[ind_dim1].role }}</span>
            <p>{{ testimonials[ind_dim1].description }}</p>
          </div>
        </div>
      </div>
      <!-- pulsanti cambio card -->
      <div class="cambio-card">
        <span class="cl-blu" @click="cambiocard()">&#183;</span>
        <span @click="cambiocard1()">&#183;</span>
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
  data() {
    return {
      ind_dim: "0",
      ind_dim1: "1",
    };
  },
  methods: {
    //funzione per cambio card dinamico
    cambiocard() {
      (this.ind_dim = 0), (this.ind_dim1 = 1);
    },
    cambiocard1() {
      (this.ind_dim = 2), (this.ind_dim1 = 3);
    },
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
}
.card {
  flex-basis: 37%;
  padding: 15px;
  box-shadow: 0px 8px 22px 5px#eff1fe;
  background-repeat: no-repeat;
  background-position: center;
  background-color: white;
  background-image: url("../assets/img/img-virgolette.png");
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
.cambio-card {
  span {
    font-size: 80px;
    margin: 0 5px;
    cursor: pointer;
  }
}
.cl-blu {
  color: #377dff;
}
</style>