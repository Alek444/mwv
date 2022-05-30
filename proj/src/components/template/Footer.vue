<template lang="pug">
  footer#c
    section#social
      h1 Entre em contato

      div
        instagram-embed(class-name="insta" :max-width=100 :url="'https://www.instagram.comp/p/B83sKxMFgOp/'" )

        a.fb-button(href="https://www.facebook.com/mwrefrigeracao.wilson.5" target="_blank") 
          <svg id="fb" x="0px" y="0px" viewBox="0 0 112.196 112.196" style="enable-background:new 0 0 112.196 112.196;" xml:space="preserve"> <g> <circle id="bola" cx="56.098" cy="56.098" r="56.098"/> <path style="fill:#FFFFFF;" d="M70.201,58.294h-10.01v36.672H45.025V58.294h-7.213V45.406h7.213v-8.34 c0-5.964,2.833-15.303,15.301-15.303L71.56,21.81v12.51h-8.151c-1.337,0-3.217,0.668-3.217,3.513v7.585h11.334L70.201,58.294z"/> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> </svg>
          p @mwrefrigeracao

        a.zap-button(href="https://api.whatsapp.com/send?phone=5588999349169&text=Ol%C3%A1%20%F0%9F%91%8B%2C%20vi%20o%20seu%20site%2C%20gostaria%20de%20saber%20mais%20sobre%20seus%20servi%C3%A7os!%20%F0%9F%91%8D%F0%9F%9B%A0%E2%9A%99" target="_blank") 
          <svg id="zap" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 512 512" style="enable-background:new 0 0 512 512;" xml:space="preserve"> <g> <g> <path d="M256.064,0h-0.128C114.784,0,0,114.816,0,256c0,56,18.048,107.904,48.736,150.048l-31.904,95.104l98.4-31.456 C155.712,496.512,204,512,256.064,512C397.216,512,512,397.152,512,256S397.216,0,256.064,0z M405.024,361.504 c-6.176,17.44-30.688,31.904-50.24,36.128c-13.376,2.848-30.848,5.12-89.664-19.264C189.888,347.2,141.44,270.752,137.664,265.792 c-3.616-4.96-30.4-40.48-30.4-77.216s18.656-54.624,26.176-62.304c6.176-6.304,16.384-9.184,26.176-9.184 c3.168,0,6.016,0.16,8.576,0.288c7.52,0.32,11.296,0.768,16.256,12.64c6.176,14.88,21.216,51.616,23.008,55.392 c1.824,3.776,3.648,8.896,1.088,13.856c-2.4,5.12-4.512,7.392-8.288,11.744c-3.776,4.352-7.36,7.68-11.136,12.352 c-3.456,4.064-7.36,8.416-3.008,15.936c4.352,7.36,19.392,31.904,41.536,51.616c28.576,25.44,51.744,33.568,60.032,37.024 c6.176,2.56,13.536,1.952,18.048-2.848c5.728-6.176,12.8-16.416,20-26.496c5.12-7.232,11.584-8.128,18.368-5.568 c6.912,2.4,43.488,20.48,51.008,24.224c7.52,3.776,12.48,5.568,14.304,8.736C411.2,329.152,411.2,344.032,405.024,361.504z"/> </g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> </svg>
          p Agendar visita!

    section#maps
      h1 Nosso endereço
      div(@click.stop.prevent="copy")
        p Av jose gifone da Silveira 3035, loja 2 #[br] Acaraú - CE #[br] CEP - 62580.000
        input#endereco(type="text" style='display: hidden;' value="Av jose gifone da Silveira 3035, loja 2. Acaraú - CE. CEP - 62580.000") 

      iframe(src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2369.3427205229796!2d-40.118482119282305!3d-2.8901018868078063!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x7ea02e420980819%3A0x1ff111fa55f81de8!2sAv.%20Jos%C3%A9%20Giffoni%20da%20Silveira%2C%203035%20-%20Perseguidas%2C%20Acara%C3%BA%20-%20CE%2C%2062580-000!5e0!3m2!1spt-BR!2sbr!4v1581777753226!5m2!1spt-BR!2sbr" frameborder="0" style="border:0;" allowfullscreen="")
      
    section#copy
      .copy
        h3#copy-year #[strong 2019] @ MW Refrigeração

      .dev
        h3 #[strong Desenvolvido por] #[a(href="https://meindexe.com/") meindexe.com]
      
      h6 Some icons made by #[a(href="https://www.flaticon.com/authors/flat-icons" title="Flat Icons") Flat Icons] from #[a(href="https://www.flaticon.com/" title="Flaticon") www.flaticon.com ] is licensed by #[a(href="http://creativecommons.org/licenses/by/3.0/" title="Creative Commons BY 3.0" target="_blank") CC 3.0 BY]

</template>

<script>
import InstagramEmbed from "vue-instagram-embed";

export default {
  name: "Footer",
  components: { InstagramEmbed },
  methods: {
    copy() {
      /* Get the text field */
      var copyText = document.getElementById("endereco");

      /* Select the text field */
      copyText.select();
      copyText.setSelectionRange(0, 99999); /*For mobile devices*/

      /* Copy the text inside the text field */
      document.execCommand("copy");

      /* Alert the copied text */
      this.$toasted.info('Endereço Copiado!', { 
        theme: "bubble", 
        position: "bottom-center", 
        duration : 5000
      })
    }
  }
};
</script>

<style lang="scss">
@import "../../styles/helpers/variables";

footer {
  display: flex;
  justify-content: center;
  flex-direction: column;

  #social {
    display: flex;
    text-align: center;
    justify-content: center;
    flex-direction: column;

     h1 { 
      font-size: 40px; 
      padding: 80px 0px 20px 0px;
      font-weight: lighter;
      text-align: center;
      color: $roxo;
    }

    div {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      .zap-button {
        display: flex;
        flex-direction: row;
        background-color: $laranja  ;
        color: $branco;
        border: 1px solid $branco;
        border-radius: 10px;

        transition: all .5s ease;

        padding: 20px;
        font-size: 20px;
        margin: 0px 20px 50px 20px;

        #zap {
          margin-right: 20px;
          width: 30px;
          fill: $branco;
          transition: all .2s ease;
        }

        &:hover {
          background-color: $branco;
          color: $laranja;
          border-color: $laranja;

          #zap {
            fill: $laranja;
          }
        }

      }

      .fb-button {
        display: flex;
        flex-direction: row;
        padding-bottom: 40px;


        #fb {
          width: 40px;
          margin-right: 10px;
          #bola {
            fill: #3B5998;
            transition: all .5s ease;

          }
        }

        p {
          font-size: 25px;
          color: rgb(59, 89, 152);
          transition: all .5s ease;

        }

        &:hover {
          #fb #bola { fill: $laranja; }
          p { color: $laranja; }
        }
      }

      .insta {
        padding: 40px 0px;
      }

    }
  }

  #maps {
    background-color: $roxo;
    color: $branco;

    padding-top: 50px;

    h1 { 
      font-size: 40px; 
      font-weight: lighter;
      text-align: center;
    }

    div {
      cursor: pointer;
      text-align: center;
      font-size: 20px;
      padding: 40px;

      input { display: none;}
    }

    iframe {
      width: 100vw;
      height: 40vh;
    }
  }

  #copy {
    display: flex;
    flex-direction: column;
    justify-content: center;
    color: $branco;
    text-align: center;
    background-color: $roxo;
    color: $branco;

    padding: 50px;

    .copy,
    .dev,
    h6 {
      font-size: 16px;
    }

    .copy {
      color: $branco;
      #copy-year strong {
        opacity: 0.5;
      }
      margin-bottom: 10px;
    }

    .dev {
      font-size: 12px;
      margin-bottom: 30px;

      h3 strong {
        opacity: 0.5;
      }
      h3 a {
        color: $branco;
      }
    }

    h6 {
      font-size: 12px;
      opacity: 0.5;
      a {
        color: $branco;
      }
    }
  }
}

// MOBILE
@media only screen and (max-width: 900px) {

}

// Telas
@media only screen and (min-width: 901px) {

}

</style>
