<template>
    <div class="card">
        <div class="moldura">
            <img :src="imagem" alt="">
        </div>

        <div class="conteudo">
            <strong>{{titulo}}</strong>
            <p>{{texto}}</p>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        imagem: String,
        titulo: String,
        texto: String
    }
}
</script>

<style>
  .card {
    height: 350px;
    width: 250px;
    box-shadow: 0px 0px 2px 1px rgba(0, 0, 0, 0.363);
    border-radius: 4px;
    padding: 20px;
    margin: 0 10px;
  }

  .card:hover {
    box-shadow: 1px 1px 3px 2px rgba(19, 43, 16, 0.637);
  }

  .moldura {
    height: 150px;
    float: center;
    border-radius: 4px;
    margin-bottom: 8px;
  }

  .moldura img {
    height: 100%;
    width: 100%;
    border-radius: 4px;
  }

  .conteudo p {
    font-size: 14px;
  }


</style>