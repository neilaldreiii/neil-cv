<template>
  <div class="container">
    <profile></profile>
  </div>
</template>

<script>
import Profile from '@/components/Profile';

export default {
  name: "home",
  components: {
    "profile": Profile
  }
};
</script>
