<template>
    <div class="container-fluid p-5">
        <div class="container">
            <div class="purple-strip1"></div>
              <div class="d-flex w-100 flex-row justify-content-center align-items-center mb-4 mt-4" id="primeiro">
                <div class="d-flex w-100 h-100 justify-content-center flex-column align-items-center mb-4 mt-4 ps-4 pe-4" :class="{'order-2': isMobile, 'justify-content-center': !isMobile}">
                        <h1 class="p-4" style="color: #482C80;">{{titulo}}</h1>
                        <p class="p-2">{{ paragrafo }}</p>
                        <a href="https://hiper.com.br/experimente-gratis?HCode=J&J03345" Target="_blank" class="btn btn-success py-2"><strong style="font-size: 1.5rem;">{{ textobotao }}</strong></a>
                </div>
                <div class="d-flex h-100  w-100 justify-content-center align-items-center mt-4 mb-4" :class="{'order-1': isMobile, 'justify-content-center': !isMobile}">
                        <div class="background-image-container"></div>
                        <img :src="urlimage" alt="" class="d-block w-100">
                </div>
              </div>
        </div>
    </div>
</template>

<script>
    export default {
        name:'ComponenteEsquerdo',
        data(){
            return{
              isMobile: false,
            }

        },
  mounted() {
    this.isMobile = window.innerWidth <= 980;
    window.addEventListener('resize', this.handleResize);
  },
  beforeDestroy() {
    window.removeEventListener('resize', this.handleResize);
  },
  methods: {
    handleResize() {
      this.isMobile = window.innerWidth <= 980;
    }},
      props:{
            titulo: String,
            paragrafo: String,
            textobotao: String,
            urlimage: String
      }
    }
</script>