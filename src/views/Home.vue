<template>
  <div class="container">
    <app-profile></app-profile>
    <div class="wrapper">
      <app-intro></app-intro>
      <app-skills></app-skills>
      <app-timeline></app-timeline>
      <app-portfolio></app-portfolio>
    </div>
  </div>
</template>

<script>
import Profile from '@/components/Profile';
import Intro from '@/components/Introduction';
import Skills from '@/components/Skills';
import Timeline from '@/components/Timeline';
import Portfolio from '@/components/Portfolio';

export default {
  name: "home",
  components: {
    "app-profile": Profile,
    "app-intro": Intro,
    "app-skills": Skills,
    "app-timeline": Timeline,
    "app-portfolio": Portfolio
  }
};
</script>
