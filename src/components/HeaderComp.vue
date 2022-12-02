<template>
  <header>
    <!-- logo -->
    <div>
      <img src="../assets/img/logo-2.png" alt="" />
    </div>
    <!-- nav conteiner -->
    <nav>
      <span v-for="(elem, index) in nav" :key="index"> {{ elem.name }}</span>
    </nav>

    <!-- nav destro con icone -->
    <div class="nav-dx">
      <!-- icone carca -->
      <div>
        <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
      </div>

      <!-- icona carrello -->
      <div>
        <font-awesome-icon icon="fa-solid fa-cart-shopping" />
      </div>

      <!-- bottone get started -->
      <div class="">
        <button class="button-blue">GetStarted</button>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderComp",
  props: {
    nav: Array,
  },
};
</script>


<style scoped lang="scss">
header {
  width: 80%;
  margin: 0 auto;
  padding: 20px 0;
  display: flex;
}
div {
  flex-basis: 20%;
  align-items: center;
  img {
    width: 50px;
  }
}

nav {
  display: flex;
  align-items: center;
  justify-content: end;
  flex-basis: 50%;
  font-weight: 600;
  font-size: 14px;
  text-align: center;

  span {
    align-items: center;
    margin: 0 10px;
    padding: 4% 0;
    color: #495057;
    justify-content: space-between;
  }
}

nav {
  span:hover {
    color: #377dff;
    border-bottom: 2px solid #377dff;
  }
}
.nav-dx {
  flex-basis: 30%;
  display: flex;
  align-items: center;
  justify-content: end;
}

.button-blue {
  background-color: #377dff;
  border: 0;
  padding: 10px 20px;
  border-radius: 3px;
  color: white;
}
</style>
