<template>
  <div>
      <provide-child-nested></provide-child-nested>
  </div>
</template>

<script>
import provideChildNested from './provideChildNested.vue'
export default {
  components: { provideChildNested },
    name:'provideChild'
}
</script>

<style>

</style>