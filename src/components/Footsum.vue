<template>
  <div class="hello">
    <h3>{{ msg }}</h3>
    </div>
</template>

<script>
export default {
  name: 'Footsum',
  props: {
    msg: String
  }
}
</script>

<style lang="scss">
h3 {
    color: #dcdcdd80;
}
</style>