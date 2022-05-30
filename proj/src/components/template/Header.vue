<template lang="pug">
  header
    //- include ../../assets/fundo-header.svg
    a(class="toggle bt-menu-div" @click="toggleMenu" v-if="!hideToggle")
      div(v-show="!isCloseIcon")
        include ../../assets/close-menu.svg
      div(v-show="isCloseIcon")
        include ../../assets/botao-menu.svg


    div(class='logo-div' )
      <svg id="logo" viewBox="0 0 395.875 73.639"><g id="Grupo_217" data-name="Grupo 217" transform="translate(-0.125)"><path id="Caminho_1" data-name="Caminho 1" d="M550.133,434.6v33.382s0,.034,0,.1c0,6.974-1.984,17.724-17.827,18.007" transform="translate(-443.637 -413.951)" fill="none" stroke="#61559a" stroke-linecap="round" stroke-width="3"></path><path id="Caminho_2" data-name="Caminho 2" d="M222.727,427.857H209.148s-13.862-.283-13.862-13.862V369.862S195,356,209.148,356h61.106s13.579.283,13.579,13.862v31.4s-.566,8.77-9.053,8.77-8.77-8.77-8.77-8.77V382.027s-.283-8.77-8.77-8.77-9.053,8.77-9.053,8.77v19.237s.566,8.77-8.487,8.77-9.053-8.77-9.053-8.77l-.283-19.237s-.283-8.77-8.77-8.77-9.053,8.77-9.053,8.77v34.8S212.26,427.857,222.727,427.857Z" transform="translate(-195.16 -356)" fill="#ff7d17"></path><g id="Refrigeração" transform="translate(139 9.362)"><text id="Refrigeração-2" data-name="Refrigeração" transform="translate(0 44)" fill="#707070" font-size="41" font-family="DancerProBook, Dancer Pro"><tspan x="0" y="0">Refrigeração</tspan></text></g></g></svg>

</template>

<script>
import { mapState } from 'vuex'

export default {
  name: "Header",
  props: {
    hideToggle: Boolean,
  },
  computed: mapState(['isCloseIcon']),
  methods: {
    toggleMenu() {
      this.$store.commit("toggleMenu")
    }
  }
};
</script>

<style lang="scss">
@import "../../styles/helpers/variables";

header {
  width: 100vw;
  position: fixed;
  display: grid;
  top: -2px;
  background-color: $branco;

  

  @media only screen and (max-width: 900px) {
    font-size: 14px;
    height: 15vh;
    z-index: 20;

    grid-template-columns: 30% 60% 20%;
    grid-template-rows: 15vh;

    #logo {
      width: 200px;
    }

    .logo-div {
      grid-column: 2;
      grid-row: 1;
      margin: auto 30vw auto auto;
      border-radius: 0px 0px 10px 10px;
    }
    .bt-menu-div {
      grid-column: 1;
      grid-row: 1;
      margin: auto auto auto auto;
    }
    #curva-svg {
      grid-column: 1 / 3;
      grid-row: 1;
      g {
        // width: 100vw;
      }
    }
  } // mobile

  @media only screen and (min-width: 901px) {
    font-size: 12px;
    grid-template-columns: 30% 10% 60%;
    z-index: 900;
    box-shadow: 0px 0px 20px rgba(0,0,0, 0.2);
    
    .logo-div {
      grid-column: 2;
      justify-self: center;
      padding: 20px 0px 10px 0px;
      border-radius: 0px 0px 20px 20px;
      svg {
        height: 40px;
        justify-self: center;
      }
    }
    .bt-menu-div {
      display: none;
    }
    #curva-svg {
      display: none;
    }
  } // desktop

  @media only screen and (min-width: 1800px) {
    grid-template-columns: 30% 10% 60%;
  }

}
</style>
