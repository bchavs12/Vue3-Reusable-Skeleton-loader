<script setup>
import { Suspense } from 'vue';
import UserCard from './components/UserCard.vue';
import UserCardSkeletonVue from './components/UserCardSkeleton.vue';


</script>

<template>
  <main>
    <Suspense>
      <UserCard />
      <template #fallback>
        <UserCardSkeletonVue />
      </template>
    </Suspense>
  </main>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Mouse+Memoirs&display=swap");

*,
::before,
::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

main {
  max-width: 620px;
  margin: 0 auto;
  padding-top: 32px;
  display: flex;
  flex-direction: column;
  gap: 16px;
}
</style>
