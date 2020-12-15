<template>
    <div>
        <provide-child></provide-child>
        <button @click="count++">plus</button>
        root : {{count}}
    </div>
</template>

<script>
export default {
    name:'provide',
    data(){
        return {
            count:0
        }
    },
    provide(){
        return {
            count: this.count
        }
    }
}
</script>

<style>

</style>