<template>
  <div class="conclusion-container">
    <div class="conclusion">
    <h2><span>Concluindo</span>...</h2>

    <div>
      <p>
      Atualmente trabalho na SdInnovation como Desenvolvedor Back-end Pleno, presencialmente. Usando o framework back-end NestJS.
    </p>
    <p>
      O fato de eu já ter conhecimento profundo também do back-end, me traz muitas vantagens no front-end, principalmente quanto à interação dentro do time.
    </p>
    </div>
    <p>
      Estou à procura de uma oportunidade no front-end; tenho bastante experiência e conhecimento de design, UX/UI e estou à disposição para <strong>testes técnicos</strong> para comprovar minha senioridade. 
    </p>
    <p>
      Já atuei com React, Next.js, Angular, HTML, CSS, JavaScript, TypeScript, APIs Rest, C#, Node, Express, NestJS, Mocha, Jest, MySQL, PostgreSQL, MongoDB, GraphQL.
    </p>
  </div>
  </div>
</template>

<style scoped>
  div.conclusion-container {
    display: flex;
    justify-content: center;
  }

  .conclusion {
    display: flex;
    flex-direction: column;
    justify-content: center;

    gap: .5rem;
    
    padding: 3rem 6rem;

    max-width: 1440px;
  }

  h2 {
    font-size: 2rem;
    font-weight: 700;
  }
  h2 span {
    font-weight: 700;
    color: var(--vt-c-text-principal);
  }

  .conclusion p {
    font-size: 1rem;
    font-weight: 600;
  }

  p strong {
    font-weight: 700;
  }

  @media (max-width: 1024px) {
    .conclusion {
      max-width: 100%;
    }
  }

  @media (max-width: 768px) {
    .conclusion {
      padding-left: 2rem;
      padding-right: 2rem;
    }
  }

  @media (max-width: 375px) {
    .conclusion {
      padding-left: 1rem;
      padding-right: 1rem;
    }

    .conclusion p {
      font-size: .9rem;
    }
  }
</style>