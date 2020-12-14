<template>
  <div>
      
      <p>event child</p>
      <button @click="submit">Submit</button>
  </div>
</template>

<script>
export default {
    name:'EventsChild',
    methods:{
        submit(){
            setTimeout( () => {
                this.$emit('onSuccess','my custom param')
            }, 1000);
        
        }
    }
}
</script>

<style>

</style>