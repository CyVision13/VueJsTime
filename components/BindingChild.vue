<template>
  <div>
      <div>binding child</div>
      <div>attrs is : {{$attrs}}</div>
      <div v-bind="$attrs">binded </div>
  </div>
</template>

<script>
export default {
    // inheritAttrs:false,
    props:['b']
}
</script>

<style>

</style>