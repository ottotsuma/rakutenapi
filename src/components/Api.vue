<template>
  <div id="api">
      {{data}}
  </div>
</template>

<script>
import axios from 'axios'

export default {
  name: 'Api',
  components: {
    api
  },
  data() {
    return {
      data: {}
    }
  },
  beforeMount(){
    this.getName();
  },
  methods: {
    async getName(){
      const res = await axios.get('https://api.agify.io/?name=michael');
    console.log(res)
    this.data = res
    }
  }
}
</script>

<style>
#api {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
