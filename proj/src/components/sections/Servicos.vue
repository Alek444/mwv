<template lang="pug">
  div.servicos
    h1 Serviços
    h3 Oferecemos manutenção e assistência para problemas com:

    section#seguimentos

      div 
        img(src="../../assets/geladeira.jpg")
        p Refrigerador

      div 
        img(src="../../assets/maquina.jpg")
        p Máquina de lavar roupa

      div 
        img(src="../../assets/forno.jpg")
        p Fornos (elétricos, a gás e microondas)

      div 
        img(src="../../assets/fogao.jpg")
        p Fogão

    section#vantagens
      div 
        <svg id="home" height="512pt" viewBox="0 -1 512 512" width="512pt" xmlns="http://www.w3.org/2000/svg">
          <path d="m204.5 458.605469v51.855469l-12.539062-10.128907c-1.9375-1.566406-48.035157-38.992187-94.78125-92.660156-64.484376-74.035156-97.179688-140.492187-97.179688-197.519531v-5.652344c0-112.761719 91.738281-204.5 204.5-204.5s204.5 91.738281 204.5 204.5v5.652344c0 4.789062-.253906 9.652344-.714844 14.574218l-39.992187-36.484374c-8.191407-83.15625-78.519531-148.339844-163.792969-148.339844-90.757812 0-164.597656 73.839844-164.597656 164.597656v5.652344c0 96.367187 124.164062 213.027344 164.597656 248.453125zm122.699219-28.660157h59.851562v-59.851562h-59.851562zm-122.699219-310.238281c46.753906 0 84.792969 38.039063 84.792969 84.792969s-38.039063 84.792969-84.792969 84.792969-84.792969-38.039063-84.792969-84.792969 38.039063-84.792969 84.792969-84.792969zm0 39.902344c-24.753906 0-44.890625 20.136719-44.890625 44.890625 0 24.75 20.136719 44.890625 44.890625 44.890625 24.75 0 44.890625-20.140625 44.890625-44.890625 0-24.753906-20.140625-44.890625-44.890625-44.890625zm280.609375 243.222656-11.21875-10.234375v64.058594c0 29.828125-24.269531 54.09375-54.097656 54.09375h-126.332031c-29.828126 0-54.097657-24.265625-54.097657-54.09375v-64.058594l-11.21875 10.234375-26.890625-29.476562 155.371094-141.746094 155.375 141.746094zm-51.121094-46.636719-77.363281-70.574218-77.359375 70.574218v100.457032c0 7.828125 6.367187 14.195312 14.195313 14.195312h126.332031c7.828125 0 14.195312-6.367187 14.195312-14.195312zm0 0"/>
        </svg>
        h3 Atendimento #[br] 100% à domicilio!

      div 
        <svg id="calendar" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 512 512" style="enable-background:new 0 0 512 512;" xml:space="preserve"> 
          <g> <g> <g> <circle cx="386" cy="210" r="20"/> <path d="M432,40h-26V20c0-11.046-8.954-20-20-20c-11.046,0-20,8.954-20,20v20h-91V20c0-11.046-8.954-20-20-20 c-11.046,0-20,8.954-20,20v20h-90V20c0-11.046-8.954-20-20-20s-20,8.954-20,20v20H80C35.888,40,0,75.888,0,120v312 c0,44.112,35.888,80,80,80h153c11.046,0,20-8.954,20-20c0-11.046-8.954-20-20-20H80c-22.056,0-40-17.944-40-40V120 c0-22.056,17.944-40,40-40h25v20c0,11.046,8.954,20,20,20s20-8.954,20-20V80h90v20c0,11.046,8.954,20,20,20s20-8.954,20-20V80h91 v20c0,11.046,8.954,20,20,20c11.046,0,20-8.954,20-20V80h26c22.056,0,40,17.944,40,40v114c0,11.046,8.954,20,20,20 c11.046,0,20-8.954,20-20V120C512,75.888,476.112,40,432,40z"/> <path d="M391,270c-66.72,0-121,54.28-121,121s54.28,121,121,121s121-54.28,121-121S457.72,270,391,270z M391,472 c-44.663,0-81-36.336-81-81s36.337-81,81-81c44.663,0,81,36.336,81,81S435.663,472,391,472z"/> <path d="M420,371h-9v-21c0-11.046-8.954-20-20-20c-11.046,0-20,8.954-20,20v41c0,11.046,8.954,20,20,20h29 c11.046,0,20-8.954,20-20C440,379.954,431.046,371,420,371z"/> <circle cx="299" cy="210" r="20"/> <circle cx="212" cy="297" r="20"/> <circle cx="125" cy="210" r="20"/> <circle cx="125" cy="297" r="20"/> <circle cx="125" cy="384" r="20"/> <circle cx="212" cy="384" r="20"/> <circle cx="212" cy="210" r="20"/> </g> </g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> <g> </g> 
        </svg>
        h3 Funcionamos #[br] em feriados!


</template>

<script>
export default {
  name: "Servicos"
};
</script>

<style lang="scss">
@import "../../styles/helpers/variables";

.servicos {
  text-align: center;
  background-color: $laranja;
  padding: 50px;

  h1 { 
    font-size: 40px;
    font-weight: lighter;
   }

  h3 { 
    font-weight: bold;
    font-size: 20px;
  }

  h1, h3 {
    color: white;
    margin-bottom: 20px;
  }

  #seguimentos {
    display: flex;
    justify-content: center;
    border-radius: 10px;

    div {
      display: flex;
      flex-direction: column;
      justify-content: center;
      
      
      img {
        background-color: $branco;
        padding: 20px;
        width: 200px;
        height: 200px;
        margin-bottom: 20px;
        border-radius: 50%;
      }

      p { 
        color: $branco;
        font-size: 20px;
        text-align: center;
        font-weight: bold;
        text-transform: uppercase;
        max-width: 200px;
      }
    }
  }

  #vantagens {
    background-color: $branco;
    box-shadow: 0px 0px 20px 5px #00000020;
    display: flex;
    justify-content: center;
    border-radius: 10px;

    margin: 0px auto;

    div {
      margin: 0px 50px;

      h3 {
        color: #777;
      }
      #home,
      #calendar {
        height: 50px;
        width: 50px;
        fill: $laranja;
      }
    }
  }
}

// MOBILE
@media only screen and (max-width: 900px) {
  .servicos {
    margin: 15vh auto 0px auto;

    #seguimentos {
      flex-direction: column;
      padding: 40px 0px;
      width: 80vw;
      margin: 0px auto;

      div {
        margin: 0px auto;
        p { margin-bottom: 20px;}

      }
    }

    #vantagens {
      flex-direction: column;
      padding: 40px 0px;
      width: 60vw;

      #calendar {
        margin-top: 40px;
      }
    }
  }
}

// Telas
@media only screen and (min-width: 901px) {
  .servicos {
    margin: 5vh auto 0px auto;

    #seguimentos {
      flex-direction: row; 
      padding: 40px;
      width: 80vw;
      margin: 0px auto 50px auto;


      div {
        margin: 0px 40px;

      }
    }

    #vantagens {
      flex-direction: row; 
      padding: 40px;
      width: 40vw;
    }
  }
}
</style>