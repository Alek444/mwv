<template lang="pug">
  nav(class="menu-nav", v-show="isMenuVisible")
    a(href="#s", class="treinamento-a") Serviços
    a(href="#c", class="software-a") Contato

</template>

<script>
import { mapState } from 'vuex'

export default {
  name: "Menu",
  computed: mapState(['isMenuVisible'])
}
</script>

<style lang="scss">
@import "../../styles/helpers/variables";

nav {
  text-align: center;
  a{
    text-transform: uppercase;    
    text-decoration: none;
    text-align: center;
    opacity: .5;
    transition: opacity .5s ease;
    z-index: 15;
  }/* ESTILO GERAL DOS LINKS*/

  /* MOBILE */
  @media only screen and (max-width: 900px) {
    display: grid;
    grid-template-rows: 30% 12% 12% 12% 12% 12% 12%;
    background-color: $laranja;
    align-items: center;
    height: 100vh;
    transition: display 1s ease;
    z-index: -1;

    a{
      font-size: 25px;
      height: 18vh;
      -webkit-tap-highlight-color: rgba(238, 53, 55, 0);
      color: $branco;
      &.router-link-exact-active {
        opacity: 1;
      }
    }

    .treinamento-a {grid-row: 2;}
    .software-a {grid-row: 3;}
    .mentoria-a {grid-row: 4;}
    .imersao-a {grid-row: 5;}
    .jogos-a {grid-row: 6;}
  }

  /* POSICIONAMENTO E ESTILO GENÉRICO */
  @media only screen and (min-width: 901px) {
    display: flex;
    padding-top: 0px;

    a{
      font-size: 20px;
      transition: opacity 1s ease;
      color: $laranja;
      font-weight: bold;  


      &.router-link-exact-active,
      &:hover,
      &:visited {
        opacity: 1;
      }
    }
    z-index: 900;
  }

  /* DESKTOP */
  @media only screen and (min-width: 900px) {
    align-items: center;
    justify-content: center;
    position: fixed;
    margin: 0px 10vw 0px 50vw;
    z-index: 900;
    a{
      font-size: 18px;
      padding: 0px 20px;
      margin: 25px 0px 10px 0px;
    }
  }

  @media only screen and (min-width: 1800px) {
    align-items: center;
    justify-content: center;
    margin: 0px 10vw 0px 45vw;
    z-index: 1000;

    a{
      font-size: 16px;
      padding: 0px 20px;
      -webkit-tap-highlight-color: rgba(238, 53, 55, 0);
      // padding: 20px 0px 10px;
    }
  }/* DESKTOP */
  
}
</style>
