<template>
  <div>
      <h1>nested child</h1>
  <hr>
  <div>count is : {{count}}</div>
  </div>

</template>

<script>
export default {
    name:'EventChildNested',
    inject:['count']
}
</script>

<style>

</style>