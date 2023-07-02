<template>
    <div class="container-fluid p-5 background-div">
        <div class="container">
            <div class="purple-strip"></div>
            <div class="d-flex w-100 flex-row justify-content-center align-items-center mb-4 mt-4" id="primeiro">
                    <div class="d-flex w-100 justify-content-center align-items-center mt-4">
                            <div class="background-image-container"></div>
                            <img :src="urlimage" alt="" class="d-block w-100">
                    </div>
                    <div class="d-flex w-100 justify-content-center flex-column align-items-center mb-4 mt-4 ps-4 pe-4">
                            <h1 class="" style="color: #482C80;">{{titulo}}</h1>
                            <p class="p-2">{{ paragrafo }}</p>
                            <a href="https://hiper.com.br/experimente-gratis?HCode=J&J03345" Target="_blank" class="btn btn-success py-2"><strong style="font-size: 1.5rem;">{{ textobotao }}</strong></a>
                        </div>
                    <!-- Conteúdo da segunda div -->
                </div>
            </div>
        </div>
</template>

<script>
    export default {
        name:'ComponenteDireito',
        data(){
            return{
            }
        },
        methods:{
            
        },
        props:{
            titulo: String,
            paragrafo: String,
            textobotao: String,
            urlimage: String
        }
    }
</script>