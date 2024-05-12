<script setup lang="ts">
import { type IconDefinition } from '@fortawesome/free-solid-svg-icons';
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';

  defineProps<{
  title: string
  description: string
  icon: IconDefinition
}>()
</script>

<template>
  <div class="card">
    <FontAwesomeIcon :icon="icon" class="icon" />

    <div class="text">
      <h3 class="title-card">{{ title }}</h3>
      <p class="text-card">{{ description }}</p>
    </div>
  </div>
</template>

<style scoped>
  .card {
    display: flex;
    align-items: start;

    gap: 1rem;

    max-height: 10rem;
  }
  .card .icon {
    width: 2.8rem;
    height: 2.8rem;

    color: #c7d1e0;

    margin-top: .4rem;
  }
  .card .text {
    max-width: 9.3rem;
  }

  .title-card {
    font-size: 1.5rem;
    font-weight: 700;
    color: var(--vt-c-text-principal);
  }

  .text-card {
    font-weight: 600;
  }
  
  @media (max-width: 1300px) {
    .card .text {
      max-width: 13rem;
    }
  }

  @media (max-width: 1180px) {
    .card .text {
      max-width: 22rem;
    }
  }

  @media (max-width: 1024px) {
    .card .text {
      max-width: 11rem;
    }
  }

  @media (max-width: 872px) {
    .card .text {
      max-width: 16rem;
    }
  }

  @media (max-width: 722px) {
    .card .text {
      max-width: 30rem;
    }
  }

  @media (max-width: 446px) {
    h3.title-card {
      font-size: 1.3rem;
    }
  }
</style>