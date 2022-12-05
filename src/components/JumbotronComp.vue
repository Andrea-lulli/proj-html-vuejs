<template>
  <div class="jumbotron">

    <!-- testo laterale six -->
    <div>
      <div>
        <h1>The biggest platform for yoour growth.</h1>
        <p>
          There are many varations of passages of lorem ipsum available, but the
          majority have suffered alteration in some form
        </p>
      </div>
      <div>
        <button class="button-blue">Read More</button>
      </div>
    </div>

    <!-- img laterale dx -->
    <div>
      <img src="../assets/img/508.jpeg" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "JumbotronComp",
};
</script>

<style lang="scss" scoped>

.jumbotron {
  width: 90%;
  margin: 0 auto;
  display: flex;
  div {
    flex-basis: 50%;
    h1 {
      margin-top: 70px;
      margin-bottom: 20px;
      line-height: 50px;
      font-weight: 500;
      font-size: 40px;
    }
    p {
      margin-bottom: 30px;
      line-height: 30px;
      color: #8e989f;
    }
  }
}
.button-blue {
  background-color: #377dff;
  border: 0;
  padding: 10px 20px;
  border-radius: 3px;
  color: white;
}
.button-blue:hover{
  background-color: black;
}

</style>