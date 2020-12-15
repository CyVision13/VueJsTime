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
        },
        busHandler(param){
            console.log(' on delete called', param);
        }
    },
    mounted(){
        this.$nuxt.$on('onDelete',this.busHandler)
    },
    beforeDestroy(){
        this.$nuxt.$off('onDelete',this.busHandler)
    }
}
</script>

<style>

</style>