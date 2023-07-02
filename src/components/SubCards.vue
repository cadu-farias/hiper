<template> 
    <div class="card ms-2 me-2" style="width: 18rem; height: 500px;">
      <img :src="urlimage" class="card-img-top" alt="...">
      <div class="card-body ">
        <h3 style="color: #482C80; text-align: center;">{{ titulo }}</h3>
        <p class="card-text" style="text-align: center;">{{ paragrafo }}</p>
      </div>
    </div>
</template>

<script>
    export default {
        name:'SubCards',
        data(){
            return{
            }
        },
        methods:{
            
        },
        props:{
            titulo: String,
            paragrafo: String,
            urlimage: String,
        }
    }
</script>