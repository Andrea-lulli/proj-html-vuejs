<template>
  <!-- sezione 2 - get tips tricks -->
  <section class="conteiner">
    <!-- card sx -->
    <div class="card-sx">
      <!-- titolo sezione  -->
      <div>
        <h1>Get tips tricks on how to skyrocket your sales</h1>
        <p>
          Faff about only a quid blower i don't want no agro bleeding chimney
          pot burke tosser cras nice one boot fanny!
        </p>
      </div>

      <!-- conteiner card con img  -->
      <div>
        <!-- card reporting -->
        <div class="card">
          <div class="img-card">
            <img src="../assets/img/510.png" alt="" />
          </div>
          <div class="descrizione">
            <h5 class="report">Reporting analysis</h5>
            <p>
              it is a long estabilished fact that a reader will be distracted by
              the readable content of a page when lookong at its layout.
            </p>
          </div>
        </div>

        <!-- card technical con img  -->
        <div class="card">
          <div class="img-card">
            <img src="../assets/img/511.png" alt="" />
          </div>
          <div class="descrizione">
            <h5>Technical SEO Audit</h5>
            <p>
              it is a long estabilished fact that a reader will be distracted by
              the readable content of a page when lookong at its layout.
            </p>
          </div>
        </div>
      </div>
      <div></div>
    </div>

    <!-- sezione destra con img  -->
    <div class="card-dx">
      <img src="../assets/img/509.jpeg" alt="" />
    </div>
  </section>
</template>

<script>
export default {
  name: "section2Comp",
};
</script>

<style lang="scss" scoped>
.conteiner {
  width: 80%;
  margin: 0 auto;
  display: flex;
  justify-content: space-around;
}

.card {
  display: flex;
}

.card-sx {
  flex-basis: 46%;
  margin-top: 80px;
}

.card-dx {
  flex-basis: 46%;
  margin-top: 80px;
}

div {
  img {
    width: 85%;
  }
}

p {
  margin-bottom: 40px;
  line-height: 20px;
  color: #8e989f;
  font-size: 12px;
}
h1 {
  line-height: 40px;
}
.descrizione {
  margin: 0px 15px;
}

.report {
  color: #377dff;
}
h5 {
  margin-bottom: 10px;
}

.img-card {
  img {
    width: 100%;
    margin: 20px 0;
  }
}
</style>