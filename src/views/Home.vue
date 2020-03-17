<template>
  <div class="home">
    <Datafinder />
  </div>
</template>

<script>
// @ is an alias to /src
import Datafinder from '@/components/Datafinder.vue'


export default {
  name: 'Home',
  components: {
    Datafinder
  }
}
</script>

<style lang="scss">
body {
  background-image: url(../assets/images/port1.png);
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
}

</style>