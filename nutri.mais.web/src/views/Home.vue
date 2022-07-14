<template>
  <v-main>
    <h1>Tenha uma vida saudável</h1>
    <div class="d-flex">
      <CardNutri 
        v-for="item in lista" 
        :key="item"
        :imagem="item.img" 
        :titulo="item.title" 
        :texto="item.text">
      </CardNutri>
    </div>
  </v-main>
</template>

<script>
import CardNutri from '../components/CardNutri.vue'
export default {
  name: "HomeView",
  components: {
    CardNutri
  },
  data () {
    return { 
      lista: [
        {
          img: 'https://cdn-icons-png.flaticon.com/512/1157/1157252.png', 
          title: 'Não coma açúcar',
          text: 'O consumo do açúcar está ligado ao aumento do risco de ter problemas como diabetes, obesidade, colesterol alto, gastrite etc. Além disso, o açúcar vicia o cérebro e fornece apenas calorias vazias para o organismo,pois ele não contém vitaminas nem minerais, que são nutrientes essenciais para o bom funcionamento do corpo.'
        },
        {
          img: 'https://www.sosergipe.com.br/wp-content/uploads/2022/03/Design-sem-nome-43.png', 
          title: 'Não use óleo de soja',
          text: 'A oxidação do óleo gera substâncias nocivas relacionados ao aumento do risco de doenças cardíacas e câncer. O excesso de óleo – como quando fritamos algo por imersão – ainda provoca excesso de gordura,o que aumenta o risco de formar placas que podem levar ao infarto, uma das maiores causas de mortalidade no Brasil.'
        },
        {
          img: 'https://images.vexels.com/media/users/3/257690/isolated/preview/ff6b1a9a9e0975d46a926072fecd19a0-ingrediente-de-cozimento-do-saco-de-farinha.png', 
          title:'Não consuma farinha de trigo.',
          text: 'A farinha de trigo é rica em carboidratos, e então entra rapidamente na corrente sanguínea. Ou seja,com o consumo do produto ao longo do tempo, o corpo pode criar uma resistência à insulina, causando um quadro de pré-diabetes ou até mesmo diabetes. Além disso, alimentos ricos em carboidratos contribuem para o aumento de complicações inflamatórias.'
        },
        {
          img: 'https://imagensemoldes.com.br/wp-content/uploads/2020/07/%C3%8Dcone-Refrigerante-PNG.png', 
          title: 'Não tome refrigerante',
          text: 'Tomar refrigerante faz mal à saúde, não só porque contém muito açúcar, mas porque também contém componentes que enfraquecem todos os órgãos do corpo. Além disso, o refrigerante não tem qualquer valor nutricional e ainda contém elevadas quantidades de sal, que favorecem a retenção de líquidos, levam ao aumento de peso, barriga estufada e pernas inchadas.'
        }
      ]
    }
  }
}
</script>

<style>

  .d-flex {
    display: flex;
  }
  
</style>