<template>
  <div>
      deep button 
      <button @click="submit">click from deep component</button>
  </div>
</template>

<script>
export default {
  name:'EventChildNested',
  methods:{
    submit(){
      setTimeout(() => {
        this.$nuxt.$emit('onDelete','delete param')
      }, 313);
    }
  }
}
</script>

<style>

</style>