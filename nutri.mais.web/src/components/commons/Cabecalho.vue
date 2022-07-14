<template>
    <header class="cabecalho">
        <div class="logo">
            <img src="../../assets/logo.png" alt="">
            <strong class="nomelogo" >Nutri Mais</strong>
        </div>
        <div class="espacador"></div>
        <div class="botao">
            <button>login</button>
            <button>Cadastre-se</button>
        </div>
    </header>
</template>

<script>
export default {
    name: 'CabecalhoView',
    components: {
    }
}
</script>

<style>
    .cabecalho {
        height: 60px;
        background-color: rgba(255, 251, 241, 0.767);
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        box-shadow: 0px 1px 4px 0px black;
        display: flex;
    }

    .botao {
        float: right;
        height: 100%;
        display: flex;
    }

    .botao button {
        border: none;
        font-size: 18px;
        font-family: none;
        background-color: transparent;
        cursor: pointer;
        margin: 0 10px;
    }

    .botao button:hover {
        font-weight: 600;
    }
 
    .logo {
        height: 100%;
        display: flex;
    }

    .espacador {
        margin-inline-start: auto;
    }

    .nomelogo {
        font-size: 24px;
        margin: auto;
        margin-left: 15px;
    }


</style>
