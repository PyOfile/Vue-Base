<template>
<b-container class="pullum">
<b-row align-v="center">
<b-col>
<div>
  <b-card class="gullum" style="max-width: 80rem;">
  <template v-slot:header>
      
    <b-form @submit="onSubmit" @reset="onReset" v-if="show" >
      <b-form-group
        id="input-group-1"
        label="Email address:"
        label-for="input-1"
      >
        <b-form-input class="fullum"
          id="input-1"
          v-model="form.email"
          type="email"
          required
          placeholder="Please Share Your Email Here!"
        ></b-form-input>
      </b-form-group>

      <b-form-group id="input-group-2" label="Your Name:" label-for="input-2">
        <b-form-input class="fullum"
          id="input-2"
          v-model="form.name"
          required
          placeholder="Please Write Your Name Here!"
        ></b-form-input>
      </b-form-group>
      <ul>
      <li><b-button type="submit" variant="dark">Submit</b-button></li>
      <li><b-button type="reset" variant="light">Reset</b-button></li>
      </ul>
   </b-form>
  </template>
  </b-card>
</div>
</b-col>
</b-row>
</b-container>
</template>

<script>
  export default {
    data() {
      return {
        form: {
          email: '',
          name: '',
          
        },
        show: true
      }
    },
    methods: {
      onSubmit(evt) {
        evt.preventDefault()
        alert(JSON.stringify(this.form))
      },
      onReset(evt) {
        evt.preventDefault()
        // Reset our form values
        this.form.email = ''
        this.form.name = ''
        // Trick to reset/clear native browser form validation state
        this.show = false
        this.$nextTick(() => {
          this.show = true
        })
      }
    }
  }
</script>

<style scoped lang="scss">
.pullum {
  
  text-decoration-color: #000000;
}

.gullum {
  border-radius: 6px;
  width: auto;
  padding: 50px 20px 20px 20px;
  background-color: #1a1b1c80;
  box-shadow: inset 0 0 10px #dcdcdd;
}

.fullum {
  background-color: #dcdcdd95;
}

ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 16px;
}

</style>