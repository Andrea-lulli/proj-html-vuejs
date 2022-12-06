<template>
  <div class="conteiner-bg-blu">
    <!-- sezione 5 latest post -->
    <section>
      <!-- titolo sezione -->
      <div class="titolo">
        <h2>Latest Posts</h2>
        <p>if you are pianning on developing a product loading</p>
      </div>

      <div class="conteiner-card">
        <!--sez card img -->
        <div class="card" v-for="(elem, index) in latest_post" :key="index">
          <div class="conteiner-img">
            <img :src="`/img/${elem.img}`" alt="" />
            <span>{{ elem.data }}</span>
          </div>

          <!-- sez card testo -->
          <div>
            <h5>{{ elem.title }}</h5>
            <p class="titolo-card">{{ elem.description }}</p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "section5Comp",
  props: {
    latest_post: Array,
  },
};
</script>


<style lang="scss" scoped>
.conteiner-bg-blu {
  width: 100%;
  background-color: #f2fff7;
}
section {
  width: 80%;
  margin: 0 auto;
}
.conteiner-card {
  display: flex;
  justify-content: space-between;
}
.card {
  flex-basis: 30%;
}
.titolo {
  text-align: center;
}
p {
  color: #8e989f;
  font-size: 11px;
  margin: 20px 0 70px 0;
  line-height: 20px;
}
.conteiner-img {
  position: relative;
  img {
    width: 100%;
  }
  span {
    position: absolute;
    top: 5px;
    left: 5px;
    font-size: 10px;
    background-color: white;
    padding: 5px;
    color: #8e989f;
    border-radius: 3px;
  }
}
h5 {
  margin: 15px 0;
}
.titolo-card {
  width: 70%;
}
</style>