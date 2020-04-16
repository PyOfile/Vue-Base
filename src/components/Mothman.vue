<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p> 
    
    </p>
  </div>
</template>

<script>
export default {
  name: 'Mothman',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h1 {
  font-size: 65px;
  padding: 1em 1em 1em 4em;
  color: #1670a0; 

}
p {
  padding: 2em 1em 2em 2em;
  font-weight: bold;
    color: #dcdcdd;
}
</style>
