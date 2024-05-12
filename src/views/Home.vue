<script setup lang="ts">
import Conclusion from '../components/Conclusion.vue';
import Presentation from '../components/Presentation.vue';
import Projects from '../components/Projects.vue';
</script>

<template>
  <div class="home">
    <Presentation />

    <Projects />

    <Conclusion />

    <footer>
      <p>Carta de apresentação do <span>Filipe Rodrigo</span> para <span>Efí Pay</span>, vaga de Desenvolvedor front-end Pleno</p>

      <p>Mini clone da página inicial de <a href="https://dev.efipay.com.br/" target="_blank">documentação técnica</a> da Efí Pay</p>
    </footer>
  </div>
</template>

<style scoped>
  footer {
    display: flex;
    align-items: center;
    justify-content: space-between;
    
    padding: 1rem 6rem;

    border-top: 2px solid #cecece;

    font-style: italic;
  }
  footer p span {
    font-weight: 500;
  }

  @media (max-width: 1264px) {
    footer {
      flex-direction: column;
      align-items: start;
    }
  }

  @media (max-width: 768px) {
    footer {
      padding-left: 2rem;
      padding-right: 2rem;
    }
  }

  @media (max-width: 375px) {
    footer {
      padding-left: 1rem;
      padding-right: 1rem;
    }
  }
</style>