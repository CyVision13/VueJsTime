<template>
  <div>
      <h1>life cycle methods</h1>
      <button @click="counter++">Counter = {{counter}}</button>
      <nuxt-link to="/">Home</nuxt-link>
  </div>
</template>

<script>
export default {
    name:'life',
    data(){
        return {
            counter:13
        }
    },
    beforeCreate(){
        console.log('beforeCreate');
    },
    created(){
        console.log('Created');
    },
    beforeMount(){
        console.log('beforeMount');
    },
    mounted(){
        console.log('mounted');
    },
    beforeUpdate(){
        console.log('beforeUpdate');
    },
    updated(){
        console.log('updated');
    },
    beforeDestroy(){
        console.log('beforeDestroy');
    },
    destroyed(){
        console.log('destroyed');
    }
}
</script>

<style>

</style>