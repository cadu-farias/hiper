<template>
    <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="true">
        <div class="carousel-inner">
            <div class="carousel-item active">
            <picture>
                    <source class="d-block w-100" media="(max-width: 860px)" srcset="https://drive.google.com/uc?id=1JCJK_b8uWJFn5QcYv5EFGCSxXkpzT-9U">
                    <source media="(max-width: 600px)" srcset="https://drive.google.com/uc?id=1lgkBWOMxWGYRT6jnJxkgvZ_O6GyUd4XQ">
                    <img src="../assets/img/Banner_2-1.jpg" class="d-block w-100" alt="irina">
            </picture>
            <a href="https://hiper.com.br/experimente-gratis?HCode=J&J03345" Target="_blank" class="btn btn-warning py-3 position-absolute btnp" style="left:21%; bottom: 20%;"><strong>{{textobotao}}</strong></a>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name:'Carousel',
        data(){
            return{
                titulo: 'O Sistema ideal para micro, pequenas e médias empresas.',
                paragrafo: 'Tenha controle total das suas vendas e estoque, cadastre clientes e produtos, faça a gestão financeira e emita documentos fiscais com o Hiper.',
                textobotao: 'Solicitar orçamento',
                urlimage: 'https://www.athuz.com.br/wp-content/uploads/2019/06/hiper_produtos.png'
            }
        },
        methods:{
            
        }
    }
</script>