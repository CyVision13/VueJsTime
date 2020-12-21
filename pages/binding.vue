<template>
  <div>
      <h1>class and style binding</h1>
      <!-- <div :class="isActive? 'active' : ''" class="binding" @click="toggle">binding : {{isActive.toString()}}</div> -->
      <!-- <div :class="{active:isActive}" class="binding" @click="toggle">binding : {{isActive.toString()}}</div> -->
      <div :class="[{active:isActive},'b']" class="binding" @click="toggle">binding : {{isActive.toString()}}</div>
      <div :style="{color:'red'}">style binding</div>
  </div>
</template>

<script>
export default {
    name:'Binding',
    data(){
        return {
            isActive:false
        }
    },
    methods:{
        toggle(){
            this.isActive = !this.isActive
        }
    }

}
</script>

<style>
.binding {
    width: 200px;
    height: 200px;
    display: flex;
    justify-content: center;
    align-items: center;
    background: red;
}
.active {
    background: burlywood;
}
</style>