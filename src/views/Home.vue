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
      <div class="footer">
        <p>Carta de apresentação do <a href="https://filiperv7.vercel.app/" target="_blank">Filipe Rodrigo</a> para <span>Efí Pay</span>, vaga de Desenvolvedor front-end Pleno</p>

<p>Mini clone da página inicial de <a href="https://dev.efipay.com.br/" target="_blank">documentação técnica</a> da Efí Pay</p>
      </div>
    </footer>
  </div>
</template>

<style scoped>
  footer {
    display: flex;
    justify-content: center;
  }
  
  .footer {
    display: flex;
    align-items: center;
    justify-content: space-between;

    max-width: 1440px;
    width: 100%;
    
    padding: 1rem 6rem;

    border-top: 2px solid #cecece;
  }
  .footer p span,
  .footer p a {
    font-weight: 600;
    color: #f37021;
  }

  @media (max-width: 1264px) {
    .footer {
      flex-direction: column;
      align-items: start;
    }
  }

  @media (max-width: 768px) {
    .footer {
      padding-left: 2rem;
      padding-right: 2rem;
    }
  }

  @media (max-width: 375px) {
    .footer {
      padding-left: 1rem;
      padding-right: 1rem;
    }
  }
</style>