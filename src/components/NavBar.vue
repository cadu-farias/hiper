<template>
    <header>
        <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
            <div class="container-fluid">
                <a class="navbar-brand" href="#">J & J Soluções</a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                    <router-link class="nav-link active" aria-current="page" to="/">Inicio</router-link>
                    </li>
                    <li class="nav-item">
                        <router-link class="nav-link" to="about">Sobre</router-link>
                    </li>
                </ul>
                </div>  
                </div>
            </nav>
    </header>
</template>
  
<script>
    export default {
        name:'NavBar',
        data(){
            return{
                menu: 'nav-list'
            }
        },
        methods:{
            abrirNavBar(){
                this.menu == 'nav-list' ? this.menu = 'nav-list active' : this.menu = 'nav-list'
            }
        }
    }
</script>
