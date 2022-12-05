<template>
  <!-- sezione 6 - contact -->
  <section class="conteiner">
    <!-- titolo contact -->
    <div class="titolo">
      <h2>Contact with our team</h2>
      <p>if you are planning on developing a product landing</p>
    </div>

    <!-- conteiner mappa -->
    <div class="conteiner-contact">
      <div class="sez-sx">
        <img src="../assets/img/StaticMapService.GetMapIma.png" alt="" />
      </div>

      <!-- conrteiner lato dx -->
      <div class="sez-dx">
        <!-- logo -->
        <div class="logo">
          <img src="../assets/img/35.png" alt="" />
        </div>

        <!-- posizione  -->
        <div class="posizione">
          <h5>9840 Shore St. Fond Du Loc. WI 54935</h5>
          <p>0 1223 456 789</p>
          <p>mail@sofbox.com</p>
        </div>

        <!-- conteiner icone  -->
        <div class="conteiner-icone">
          <font-awesome-icon
            icon="fa-brands fa-facebook-f"
            class="icone icone-fb"
          />
          <font-awesome-icon icon="fa-brands fa-twitter" class="icone" />
          <font-awesome-icon icon="fa-brands fa-github" class="icone" />
          <font-awesome-icon icon="fa-brands fa-instagram" class="icone" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "section6Comp",
};
</script>

<style lang="scss" scoped>
.conteiner {
  margin: 0 auto;
  width: 80%;
}
.titolo {
  text-align: center;
  margin: 50px 0;
  p {
    margin: 20px 0;
  }
}

p {
  color: #8e989f;
  font-size: 11px;
  margin: 15px 0;
}
h5 {
  margin: 20px 0;
}
.conteiner-contact {
  display: flex;
  justify-content: space-between;
}
.sez-sx,
.sez-dx {
  flex-basis: 48%;
  img {
    width: 100%;
  }
}

.sez-dx {
  flex-basis: 48%;
  img {
    width: 20%;
  }
}
.icone {
  color: #377dff;
  border: 1px solid #eee5e5;
  margin-left: 8px;
  padding: 5px;
}
.icone-fb {
  padding: 5px 9px;
}
</style>