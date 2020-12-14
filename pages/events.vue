<template>
  <div>
       <events-child @onSuccess="onSuccess"></events-child>
  </div>
</template>

<script>
export default {
name: 'Events',
    methods:{
        onSuccess(param){
            console.log('success',param);
        }
    }
}
</script>

<style>

</style>