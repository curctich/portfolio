<template>
  <div>
    <MV />
    <Profile />
    <Career />
  </div>
</template>

<script>
import MV from '~/components/MV.vue';
import Profile from '~/components/Profile.vue';
import Career from '~/components/Career.vue';

export default {
  components: {
    MV,
    Profile,
    Career,
  }
}
</script>

<style lang="scss" scoped>
</style>
