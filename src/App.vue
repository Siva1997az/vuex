<template>
  <div>
    <four-tag></four-tag>
    <eight-tag></eight-tag>
  </div>
</template>

<script>
import Four from './components/Four.vue'
import Eight from './components/Eight.vue'
export default {
  name: 'App',
  data() {
    return {
      
    }
  },
  components: {
    'four-tag':Four,
    'eight-tag':Eight
  },
  mounted() {
    // alert(this.$store.getters.getName);
    // this.xyz=this.$store.getters.getName
    // console.log(this.xyz)
    this.$store.dispatch('actCode').then((data)=>{
      console.log(data)
    }).catch((data)=>{
      console.log(data)
    })
  
  }
}
</script>

<style>

</style>
