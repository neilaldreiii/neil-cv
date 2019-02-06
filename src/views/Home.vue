<template>
  <div class="container">
    <app-profile></app-profile>
    <div class="wrapper">
      <app-intro></app-intro>
      <app-skills></app-skills>
    </div>
  </div>
</template>

<script>
import Profile from '@/components/Profile';
import Intro from '@/components/Introduction';
import Skills from '@/components/Skills';

export default {
  name: "home",
  components: {
    "app-profile": Profile,
    "app-intro": Intro,
    "app-skills": Skills
  }
};
</script>
