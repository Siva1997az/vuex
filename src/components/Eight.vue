<template>
    <div>
        <h1>{{randomname}}</h1>
    </div>
  </template>
  
  <script>
  
  
  export default {
    name: 'App',
    components: {},
      data() {
        return {
            randomname:''
        }
      
    },
    
    mounted() {
        
        this.$store.commit('setName','Bittu')
        this.randomname=this.$store.getters.getName
    },
    created() {

    }
  }
  </script>
  
  <style>
  
  </style>
  