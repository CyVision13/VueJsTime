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
        defaultInitialValue:{
            type:Number,
            required:true
        },
        initialCounter:{
            type:Number,
            // required:true,
            default(){
                return this.defaultInitialValue
            }
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