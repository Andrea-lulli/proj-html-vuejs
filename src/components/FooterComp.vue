<template>
  <div class="conteiner-bg-blu">
    <footer class="conteiner-sito">
      <div class="conteiner-card">
        <!-- footer laterale sx -->
        <div class="card-sx">
          <div>
            <img src="../assets/img/35.png" alt="" />
          </div>
          <div>
            <p>
              It is a long estabilished fact that a reder will be distracted by
              the readable content.
            </p>
            <p>Copyright @ 2018 <span>Sofbox</span></p>
          </div>
        </div>

        <!-- footer laterale dx -->
        <div class="card-dx">
          <ul v-for="(elem, index) in footer" :key="index">
            <li class="titolo">{{ elem.name }}</li>
            <li
              class="lista-footer"
              v-for="(element, index) in elem.options_menu"
              :key="index"
            >
              {{ element.name }}
            </li>
          </ul>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: "FooterComp",
  props: {
    footer: Array,
  },
};
</script>

<style lang="scss" scoped>
.conteiner-bg-blu {
  width: 100%;
  background-color: #f2fff7;
  border-top: #efe9e9 1px solid ;
  padding-top: 50px;
}
.conteiner-card {
  display: flex;
}

.card-sx {
  flex-basis: 20%;
}

.card-dx {
  flex-basis: 73%;
  display: flex;
  justify-content: space-around;
}

p {
  margin-bottom: 40px;
  line-height: 20px;
  color: #8e989f;
  font-size: 10px;
}

span {
  color: #377dff;
  font-weight: 700;
  font-size: 12px;
}

img {
  width: 50%;
}

li {
  color: black;
  list-style: none;
}

.titolo {
  font-size: 13px;
  font-weight: 700;
  margin-bottom: 20px;
}

.lista-footer {
  font-size: 11px;
  color: #8e989f;
  margin-bottom: 15px;
}
</style>