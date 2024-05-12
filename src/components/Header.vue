<template>
  <div class="header">
    <div class="logo">
      <p>Olá, recrutador(a) da</p>
      <img alt="Vue logo" class="logo-efi" src="@/assets/logo-efi-pay.svg" />
    </div>
    <div class="buttons">
      <a href="https://www.linkedin.com/in/filiperv7/" target="_blank" class="cta">Contatar Filipe</a>
      <a href="https://github.com/filiperv7/efiPay_filipe" target="_blank" class="cta emphasis">Ver repositório</a>
    </div>
  </div>
</template>

<style scoped>
  .header {
    z-index: 10;
    position: absolute;

    width: 100%;
    padding: 2rem 6rem;

    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .logo {
    display: flex;
    flex-direction: column;
  }
  .logo p {
    font-weight: 600;
  }

  .buttons {
    display: flex;
    gap: .8rem;
  }
  .buttons > a.cta {
    min-width: 11.6rem;
  }
  .buttons > a.emphasis {
    background: white;
    color: #0F8DAB;
  }

  @media (max-width: 768px) {
    .header {
      padding: 2rem 2rem;
    }
  }

  @media (max-width: 650px) {
    .buttons > a.cta {
      min-width: 9rem;
      padding: .6rem;
    }
  }

  @media (max-width: 560px) {
    .buttons > a.cta {
      min-width: 6rem;
      font-size: .8rem;
    }
  }

  @media (max-width: 490px) {
    .buttons {
      flex-direction: column;
      gap: .4rem;
    }
    .buttons > a.cta {
      min-width: 9rem;
      font-size: .9rem;
    }
  }

  @media (max-width: 375px) {
    .header {
      padding-left: 1rem;
      padding-right: 1rem;
    }

    .logo p {
      font-size: .7rem;
    }
    .logo-efi {
      max-width: 8rem;
    }

    .buttons > a.cta {
      min-width: 7rem;
      font-size: .7rem;
    }
  }
</style>