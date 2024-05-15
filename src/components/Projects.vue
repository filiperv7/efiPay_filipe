<script setup lang="ts">
import { faDev } from '@fortawesome/free-brands-svg-icons';
import { faCode, faKeyboard, faLaptop, faMicrochip, faTerminal, type IconDefinition } from '@fortawesome/free-solid-svg-icons';
import Card from '../components/Card.vue';


interface CardContent {
  title: string;
  description: string;
  icon: IconDefinition;
}

const cardsContent: CardContent[] = [
  {
    title: "+3 anos de Front-end",
    description: "JS, TS, principais frameworks front-end e consumo de APIs Rest",
    icon: faCode
  },
  {
    title: "+2 anos de Back-end",
    description: "C# com .NET e Node com TypeScript, Express, NestJS; Integração com DB",
    icon: faTerminal
  },
  {
    title: "Projetos freelancer",
    description: "Como o site da Epiffania Joias em React com CMS em GraphQL",
    icon: faDev
  },
  {
    title: "2 anos na Capgemini",
    description: "Cuidando de demandas back-end e contribuindo com domínio de negócio",
    icon: faLaptop
  },
  {
    title: "TDD, SOLID e DBB",
    description: "Prezo pela qualidade do código limpo e semântico com eficiência",
    icon: faKeyboard
  },
  {
    title: "Experiências variadas",
    description: "Já trabalhei em outros setores da tecnologia, inclusive com hardware",
    icon: faMicrochip
  },
]
</script>

<template>
  <div class="projects-container">
  <div class="projects">
    <div class="content">
      <h2><span>Carreira,</span> meu desempenho profissional</h2>

      <div class="cards">
        <Card v-for="card in cardsContent" v-bind:key="card.title" :title="card.title" :description="card.description" :icon="card.icon" />
      </div>
    </div>

    <a href="https://filiperv7.vercel.app/" target="_blank"><img src="@/assets/portfolio.svg" alt="" class="portfolio"></a>
   </div>
  </div>
</template>

<style scoped>
  div.projects-container {
    background-color: #ffffff;

    display: flex;
    justify-content: center;
  }

  div.projects {
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    position: relative;

    width: 100%;
    max-width: 1440px;
    
    padding: 3rem 6rem;
  }
  div.projects .content {
    display: flex;
    flex-direction: column;
    
    gap: 2rem;
  }

  h2 {
    font-size: 2rem;
    font-weight: 700;
  }
  h2 span {
    font-weight: 700;
    color: var(--vt-c-text-principal);
  }

  div.cards {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;

    gap: 2rem;
  }

  div.projects > a {
    position: absolute;
    right: 0;
  }

  img.portfolio {
    height: 22rem;
    width: 30rem;
    
    object-fit: cover;
    object-position: 0;
  }
  
  @media (min-width: 1460px) {
    img.portfolio {
      position: static;
      object-fit: fill;
      
      height: 25rem;
      width: 34rem;
    }

  }

  @media (max-width: 1300px) {
    div.cards {
      grid-template-columns: 1fr 1fr;
    }
  }
  
  @media (max-width: 1180px) {
    div.cards {
      grid-template-columns: 1fr;
    }
  }

  @media (max-width: 1024px) {
    div.cards {
      grid-template-columns: 1fr 1fr 1fr;
    }

    div.projects > a {
      display: none;
    }
  }

  @media (max-width: 872px) {
    div.cards {
      grid-template-columns: 1fr 1fr;
    }
  }
  
  @media (max-width: 768px) {
    div.projects {
      padding-left: 2rem;
      padding-right: 2rem;
    }
  }

  @media (max-width: 722px) {
    div.cards {
      grid-template-columns: 1fr;
    }
  }

  @media (max-width: 446px) {
    h2 {
      font-size: 1.8rem;
    }
  }

  @media (max-width: 375px) {
    div.projects {
      padding-left: 1rem;
      padding-right: 1rem;
    }

    h2 {
      font-size: 1.6rem;
    }
  }
</style>