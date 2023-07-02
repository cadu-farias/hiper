<template>
  <header>
    <NavBar />
  </header>
    <Carousel />
    <div class="background-div1 pb-5">
      <a href="https://wa.me/5586998006276?text=Olá%20quero%20testar%20o%20aplicativo%20Hiper%20gestão%20grátis!" class="whatsapp-button" target="_blank" rel="noopener noreferrer">
        <span class="whatsapp-icon"></span>
        Teste grátis
      </a>
      <ComponenteSimples />
      <Cards />
    </div>
    <div v-for="post in postagens">
      <ComponenteDireito :titulo="post.titulo" v-if="post.lado == 1" :paragrafo="post.paragrafo" :textobotao="post.textobotao" :urlimage="post.urlImage" />
      <ComponenteEsquerdo :titulo="post.titulo" v-else :paragrafo="post.paragrafo" :textobotao="post.textobotao" :urlimage="post.urlImage" />
    </div>
    <!-- <RouterView /> -->
    <footer id="sticky-footer" class="flex-shrink-0 py-4 bg-dark text-white-50">
    <div class="container text-center">
      <small>Copyright &copy; Cadu Farias</small>
    </div>
  </footer>
</template>

<script>
import NavBar from './components/NavBar.vue'
import ComponenteSimples from './components/ComponenteSimples.vue'
import Carousel from './components/Carousel.vue'
import Cards from './components/Cards.vue'
import ComponenteDireito from './components/ComponenteDireito.vue'
import ComponenteEsquerdo from './components/ComponenteEsquerdo.vue'

const postagens = [
        {
        titulo: 'Realize vendas',
        paragrafo: 'Descomplique as rotinas administrativas da sua loja, controle o estoque e relize vendas com o Hiper. Tudo o que o seu negócio precisa para continuar crescendo.',
        urlImage: 'https://drive.google.com/uc?id=1NpaFXFLtPr1_KmnMpL3YcODgLAVLxXqK',
        textobotao: 'Experimente Grátis',
        lado:1
        },
        {
        titulo: 'Controle de Estoque',
        paragrafo: 'Uma boa gestão de estoque é essencial para o sucesso da sua loja. Com o Hiper, você utiliza o mesmo sistema que faz a gestão da sua loja para gerir o seu estoque, garantindo informações detalhadas, atualizadas e armazenadas com segurança.',
        urlImage: 'https://www.prontosolucoes.com/img/hiper/hiper-gestao-estoque.jpg',
        textobotao: 'Experimente Grátis',
        lado:2
        },{
        titulo: 'Gestão financeira',
        paragrafo: 'Com o módulo financeiro do Hiper, você tem controle total das receitas da sua loja. Controle seu fluxo de caixa, gere relatórios de resultado e acompanhe as contas a pagar e receber.',
        urlImage: 'https://impactoautomacao.com.br/hiper_novo/img/gestao-financeira.png',
        textobotao: 'Experimente Grátis',
        lado:1
        },{
        titulo: 'Emissão Fiscal NFC-e',
        paragrafo: 'Seja qual for a sua demanda fiscal o Hiper te atende, ele é homologado para emissão de documentos fiscais NFe, NFC-e e ECF. Nele é possível importar via XML as notas fiscais de compras de forma simples e rápida. Também é possível gerar o Sintegra e o SPED fiscal, conforme a necessidade do seu negócio.',
        urlImage: 'https://impactoautomacao.com.br/hiper_novo/img/nota-fiscal.png',
        textobotao: 'Experimente Grátis',
        lado:2
        },
    ]

export default {
  data(){
    return{
      postagens: postagens
    }
  },components:{
    NavBar,
    ComponenteSimples,
    Carousel,
    Cards,
    ComponenteDireito,
    ComponenteEsquerdo
  }
}
</script>

<style>

</style>
