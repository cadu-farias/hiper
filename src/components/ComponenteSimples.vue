<template>
    <div class="container-fluid  pb-5 d-flex">
        <div class="d-flex w-100 flex-row justify-content-center align-items-center" id="primeiro" >
            <div class="d-flex w-50 justify-content-center align-items-center">
                <img :src="urlimage" alt="" class="d-block w-100">
            </div>
            <div class="d-flex w-50 justify-content-center flex-column align-items-center ps-4 pe-4">
                <h1 style="color: #482C80;" class="pb-4">{{ titulo }}</h1>
                <p class="m-2 pb-4">{{ paragrafo }}</p>
                <a  href="https://hiper.com.br/experimente-gratis?HCode=J&J03345" Target="_blank" class="btn btn-info p-3 mb-4"><strong style="font-weight: 800;">Experimente Grátis</strong></a>
                
            </div>
        </div> 
    </div>
</template>

<script>
    export default {
        name:'ComponenteSimples',
        data(){
            return{
                titulo: 'O Sistema ideal para micro, pequenas e médias empresas.',
                paragrafo: 'Tenha controle total das suas vendas e estoque, cadastre clientes e produtos, faça a gestão financeira e emita documentos fiscais com o Hiper.',
                textobotao: 'Experimente Grátis',
                urlimage: 'https://impactoautomacao.com.br/hiper_novo/img/img-sistema-ideal.png'
            }
        },
        methods:{
            
        }
    }
</script>