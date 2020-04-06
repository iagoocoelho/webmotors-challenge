<template>
  <div id="app">
    <!-- <HelloWorld/> -->
    <header>
      <img src="./assets/logo-webmotors.png" alt />
    </header>
    <div class="searchContainer">
      <div class="searchTypeLine">
        <a href="#" class="searchType">
          <img src="./assets/car_icon_gray.svg" alt="carIcon" />
          <h2>
            <span>comprar</span>
            <strong>CARROS</strong>
          </h2>
        </a>
        <a href="#" class="searchType">
          <img src="./assets/bike_icon_gray.svg" alt="motocycleIcon" class="icon" />
          <h2>
            <span>comprar</span>
            <strong>MOTOS</strong>
          </h2>
        </a>
      </div>
      <div class="buttonSellCar">
        <a href="#">Vender meu carrro</a>
      </div>

      <div class="form">
        <form>
          <div class="checkboxNewUsed">
            <input type="checkbox" name id="novo" />
            <label for="novo">Novos</label>
            <input type="checkbox" name id="usado" />
            <label for="usado">Usados</label>
          </div>

          <div class="inputContainer">
            <div class="localization">
              <span>Onde:</span>
              <input type="text" name id value="São Paulo" />
            </div>

            <div class>
              <span>Raio</span>
              <select>
                <option>25 km</option>
                <option>50 km</option>
                <option>75 km</option>
                <option>100 km</option>
              </select>
            </div>

            <div class>
              <span>Marca</span>
              <select>
                <option>A</option>
                <option>B</option>
                <option>C</option>
              </select>
            </div>

            <div class>
              <span>Modelo</span>
              <select>
                <option>A</option>
                <option>B</option>
                <option>C</option>
              </select>
            </div>
          </div>

          <div class="inputContainer">
            <div class="inputContainerSize2">
              <span>Ano Desejado</span>
              <select>
                <option>A</option>
                <option>B</option>
                <option>C</option>
              </select>
            </div>

            <div class="inputContainerSize2">
              <span>Faixa de Preço</span>
              <select>
                <option>A</option>
                <option>B</option>
                <option>C</option>
              </select>
            </div>

            <div class="inputContainerSize3">
              <span>Versão:</span>
              <select>
                <option>A</option>
                <option>B</option>
                <option>C</option>
              </select>
            </div>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: "App",
  components: {
    // HelloWorld
  }
};
</script>

<style lang="scss">
#app {
  margin: 0;
  padding: 0;

  a {
    text-decoration: none;
    color: #8b8b97;
  }

  header {
    max-width: 993px;
    margin: 0 auto;
  }

  div.searchContainer {
    max-width: 993px;
    margin: 0 auto;
    height: 312px;

    div.searchTypeLine {
      display: inline;

      a.searchType {
        display: inline-flex;
        text-transform: uppercase;
        padding: 0 20px 8px 20px;
        border-bottom: 1px solid #d8d8d8;
        line-height: 1.4em;

        &:hover {
          color: red;
          border-bottom: 2px solid red;
          h2 span {
            color: #8b8b97;
          }
        }

        img {
          width: 27px;
          height: 22px;
          margin-right: 14px;
          align-self: flex-end;

          &:hover {
            color: red;
          }
        }

        h2 {
          display: flex;
          flex-direction: column;
          margin: 0;
        }
      }
    }

    .buttonSellCar {
      float: right;
      display: flex;
      border-color: #f89e00;
      color: #f89e00;
      border: 2px solid;
      width: 200px;
      height: 40px;
      align-items: center;
      justify-content: center;

      a {
        color: #f89e00;
      }
    }

    div.form {
      width: 100%;
      background-color: #fff;
    }
  }
}
</style>