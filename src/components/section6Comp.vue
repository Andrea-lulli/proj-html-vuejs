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
        <div class="mappa">
          <img src="../assets/img/StaticMapService.GetMapIma.png" alt="" />
          <div class="conteiner-ind">
            <div>
              <p class="street">Storey Ave</p>
              <p>San Francisco. California 94129</p>
              <p class="opzioni-mappa">Visualizza mappa piu grande</p>
            </div>
            <div>
              <img src="../assets/img/freccia mappa.png" alt="" />
            </div>
          </div>

          <!-- posizione su mappa -->
          <div class="ind-posizione">
            <img src="../assets/img/posizione-mappa.png" alt="" />
          </div>
          <!-- dati mappa -->
          <div class="dati-mappa">
            <span>Data maggio 2020 </span>
            <span>Termini e condizioni d'uso</span>
            <span>Segnala un arrore sulla mappa</span>
          </div>

          <!-- zoom mappa -->
          <div class="zoom">
            <div>
              <button>+</button>
            </div>
            <div>
              <button>-</button>
            </div>
          </div>

          <!-- immagine satellite su mappa -->
          <div class="img-satellite">
            <img src="../assets/img/satellite.png" alt="" />
          </div>
        </div>
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
        <!-- conteiner form -->
        <div>
          <div>
            <h5>Get in Touch</h5>
          </div>

          <!-- form -->
          <form>
            <!-- conteiner imnput name e mail -->
            <div class="input_name">
              <input class="name" type="text" placeholder="Your Name" />
              <input class="name email" type="email" placeholder="Your Email" />
            </div>

            <!-- conteiner imnput subject-->
            <div class="input_subject">
              <input class="name" type="text" placeholder="Your Subject" />
            </div>

            <!-- conteiner imnput subject-->
            <div class="input_subject">
              <textarea class="message" name="message" rows="20" cols="65">
               Your Message</textarea
              >
            </div>
            <!-- button di invio dati -->
            <div>
              <button class="button-blue">Send Message</button>
            </div>
          </form>
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
  border: 1px solid #efe9e9;
  margin-right: 8px;
  padding: 5px;
}
.icone-fb {
  padding: 5px 9px;
}
.input_name {
  display: flex;
  justify-content: space-between;
  input {
    flex-basis: 48%;
    padding: 10px;
    border: 1px solid #efe9e9;
    font-size: 12px;
  }
}
.input_subject {
  display: flex;

  input {
    border: 1px solid #efe9e9;
    font-size: 12px;
    margin: 15px 0;
    padding: 10px;
    flex-basis: 100%;
  }
}

.message {
  border: 1px solid #efe9e9;
  font-size: 12px;
  margin: 15px 0;
  padding: 10px;
  color: #8e989f;
}

.button-blue {
  background-color: #377dff;
  border: 0;
  padding: 10px 20px;
  border-radius: 3px;
  color: white;
  margin: 15px 0 100px 0;
}
.conteiner-ind {
  display: flex;
  position: absolute;
  top: 5px;
  left: 5px;
  background-color: white;
  padding: 7px;
  div {
    p {
      line-height: 4px;
      margin-right: 20px;
    }
  }
}
.street {
  color: black;
  font-weight: 700;
}

.opzioni-mappa {
  color: #377dff;
  margin-top: 30px;
  font-weight: 700;
}

.ind-posizione {
  position: absolute;
  top: 40%;
  left: 50%;
}

.dati-mappa {
  position: absolute;
  display: flex;

  bottom: 0;
  right: 0;
  span {
    font-size: 8px;
    padding: 2px;
    margin: 0 1px;
    background-color: white;
    color: black;
    font-weight: 800;
  }
}
.mappa {
  position: relative;
}

.zoom {
  position: absolute;
  bottom: 10%;
  right: 2%;
  background-color: white;
  button {
    background-color: white;
    border: 0;
    font-size: 30px;
    font-weight: 700;
    color: #8e989f;
    text-align: center;
    padding: 5px 10px;
    width: 100%;
  }
}

.img-satellite {
  position: absolute;
  left: 5%;
  bottom: 5%;

  img {
    width: 80%;
    border: 3px solid white;
    border-radius: 7px;
  }
}
</style>