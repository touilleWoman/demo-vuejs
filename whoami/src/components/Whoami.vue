<template>
  <div>
    <button v-on:click="apiGet"> who am I ? </button>
    <User :info="info"/>
  </div>
</template>

<script>
import User from "./User.vue"
import axios from "axios"

export default {
    name: "Whoami",
    components : {
      User
    },
    data () {
      return {
          info: null
      }
    },
    methods :{
        apiGet(){
            axios
              .get('https://stage.numizon.com/userapi/user/', {
                  auth: {
                    username: 'jie123',
                    password: '5Qg-c6X-mcB-oQZ'
              }})
              .then(response => (this.info = response.data))
        }
    }
}
</script>

<style scoped>

</style>