<template>
    <div>
        <h1>{{xyz}}</h1>
        
    </div>
  </template>
  
  <script>
  
  
  export default {
    name: 'App',
    data() {
     return {
      xyz:''
     }
    },
    components: {
      
    },
    mounted() {
    // alert(this.$store.getters.getName);
    this.$store.commit('setName','tarak')
    this.xyz=this.$store.getters.getName
    // console.log(this.xyz)
    
  }
  }
  </script>
  
  <style>
  
  </style>
  