<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p> This site is dedicated to reaching out to small businesses that would like to build a legit web 
        presence no matter your technical level. We want to bring the Mom & Pop business to the web. Our 
        objective is to offer you a site that pleases you with services available to help with site management. 
        We want to bring the new wave of companies to the web. Why? Because we want to bring small business 
        into the 21st with a helping hand. So please contact us for a consultation.
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
