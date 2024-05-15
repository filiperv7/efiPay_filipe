<template>
  <main>
    <div class="presentation">
      <div>
      <a href="https://drive.google.com/file/d/1L-HxzH4KHwZUspZ-QiKIPs86CHep6mfo/view?usp=sharing" target="_blank">
        <img src="../assets/resume.svg" alt="" class="resume">
      </a>
    </div>
   <div class="content-presentation">
    <div class="text-presentation">
      <h1>
        <strong>Filipe Rodrigo</strong>,
        um parceiro no
        <span>desenvolvimento e crescimento</span>
      </h1>
      <h3>Fiz rapidamente esse "clone" do site da Efí Pay em VueJS 3 para falar um pouco de mim e demonstrar parte dos meus conhecimentos em tecnologias front-end. Escolhi o Vue por ser um dos requisitos.</h3>
    </div>

    <a href="https://drive.google.com/file/d/1L-HxzH4KHwZUspZ-QiKIPs86CHep6mfo/view?usp=sharing" target="_blank" class="cta cta-curriculum">
      <img alt="Vue logo" src="@/assets/arrow.svg" />
      <span>Acessar currículo completo</span>
    </a>
   </div>
    </div>
  </main>
</template>

<style scoped>
  main {
    display: flex;
    justify-content: center;
  }

  div.presentation {
    display: flex;
    justify-content: space-between;

    max-width: 1440px;

    padding: 6rem 6rem;

    position: relative;
  }

  main a:has(.resume) {
    position: absolute;
    
    bottom: -.5rem;
  }

  main .resume {
    max-height: 32rem;
  }
  
  main .content-presentation {
    max-width: 37%;

    margin-top: 6rem;
    
    display: flex;
    flex-direction: column;
    gap: 3rem;
  }

  .text-presentation {
    display: flex;
    flex-direction: column;
    gap: 1rem;

    color: #1D1D1D;
  }

  h1 {
    font-size: 2.3rem;
    font-weight: 600;

    line-height: 1.3;
  }
  h1 strong {
    font-weight: 900;
    color: var(--vt-c-text-principal);
  }
  h1>span {
    font-weight: 700;
  }

  h3 {
    font-weight: 400;
    line-height: 1.4;
  }

  a.cta-curriculum {
    gap: .5rem;

    width: 80%;
  }
  
  a span {
    font-weight: 600;
  }
  
  @media (max-width: 1127px) {
    div.presentation {
      padding-bottom: 2rem;
    }

    div.content-presentation {
      margin-top: 3rem;
    }

    .resume {
      max-width: 30rem;
    }

    a.cta-curriculum {
      width: 90%;
    }
  }

  @media (max-width: 1000px) {
    .resume {
      max-width: 24rem;
    }

    div.content-presentation {
      max-width: 42%;
    }
  }

  @media (max-width: 900px) {
    div.presentation {
      flex-direction: column-reverse;
      align-items: center;

      gap: 2rem;

      padding-bottom: 0;
    }

    main .content-presentation {
      max-width: 100%;

      margin-top: 5rem;
      align-items: center;
      
      gap: 2rem;
    }

    h1 {
      font-size: 2rem;
    }

    a.cta-curriculum {
      width: 70%;
    }
    
    .content-presentation h1,
    .content-presentation h3 {
      text-align: center;
    }

    main a:has(.resume) {
      position: relative;
    }
  }

  @media (max-width: 768px) {
    div.presentation {
      padding-left: 2rem;
      padding-right: 2rem;
    }
  }

  @media (max-width: 545px) {
    a.cta-curriculum {
      width: 90%;
    }
  }
  
  @media (max-width: 425px) {
    main .resume {
      max-width: 21rem;
    }  
  }

  @media (max-width: 375px) {
    div.presentation {
      padding-left: 1rem;
      padding-right: 1rem;
    }
  }

  @media (max-width: 352px) {
    a.cta-curriculum {
      font-size: .8rem;
    }
  }

  @media (max-width: 350px) {
    main .resume {
      max-width: 18rem;
    }
  }
</style>
