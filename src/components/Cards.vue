<template>
    <div class="container-fluid mb-4" >
    <div id="title1" class="d-flex justify-content-center mb-5 pb-4 pt-4">
        <h1  style="color: #482C80;">{{ titulo }}</h1>
    </div>
    <div class="d-flex flex-row justify-content-center align-items-center  p-3 mb-5 "  id="segundo">
        <SubCards v-for="card in cards" :titulo="card.tituloCard" :paragrafo="card.paragrafoCard" :urlimage="card.urlImage" />
    </div>
    </div>
</template>

<script>
    import SubCards from './SubCards.vue';
    const cards = [
        {
        tituloCard: 'Aplicativo mobile',
        paragrafoCard: 'Com o aplicativo de força de vendas você pode realizar suas vendas de qualquer lugar e a qualquer momento com o seu celular.',
        urlImage: 'https://drive.google.com/uc?id=10SIEQt1VBKEHfTZv39ym2zglWOm_iEX5',
        },
        {
        tituloCard: 'Gestão na nuvem sempre a mão',
        paragrafoCard: 'Gerencie sua loja utilizando um sistema que controla seu financeiro, vendas, estoque e ainda conta com a parte fiscal sempre atualizada.',
        urlImage: 'https://drive.google.com/uc?id=1OSRTzNuUwbJeD8_iOX3xOdQSzDGkz8PB',
        },{
        tituloCard: 'Feito para atender o seu negócio',
        paragrafoCard: 'O cliente pode optar pela versão mais simples com preço reduzido ou pela versão completa, com todos os recursos.',
        urlImage: 'https://drive.google.com/uc?id=166gwgemtK0gl__dFTrHCbwyIy7INq3Rt',
        },{
        tituloCard: 'Sistema online e offline',
        paragrafoCard: 'Faça as operações do dia a dia da sua loja sem se preocupar com a internet, quando a conexão voltar a sincronização é automática.',
        urlImage: 'https://drive.google.com/uc?id=1HmczQiKZiwJa0NRQes8L_4XIZTtbxhoQ',
        },
    ]
    export default {
        name:'Cards',
        data(){
            return{
                titulo: 'Motivos para Adquirir',
                cards: cards
            }
        },
        methods:{
            
        },
        components:{
            SubCards
        }
    }
</script>