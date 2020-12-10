<template>
  <div>
      <p>Counter is {{counter}}</p>
      <p>initial counter {{initialCounter}}</p>
      <button @click="counter++">plus</button>
  </div>
</template>

<script>
export default {
    // props:['initialCounter'],
    props:{
        initialCounter:{
            type:Number,
            required:true,
            
        }
    },
    data(){
        return {
            counter: this.initialCounter
        }
    }
}
</script>

<style>

</style>