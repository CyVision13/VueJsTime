<template>
    <div>
        <h1>Methods</h1>
        <div>
            getcomputedCount : {{getcomputedCount}}
        </div>
        <div>
            getCountMethod : {{getCountMethod()}}
        </div>
        <div @click="updateCounter">
            updateCounter : {{count}}
            <div @click.stop="updateCounter2"> <!-- erja nadadan be @click parrent -->
                updateCounter2 : {{count2}}
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:"methods",
    data(){
        return{
            count:0,
            count2:0
        }
    },
    computed:{
        getcomputedCount(){
            console.log('getComputed');
            return this.count * 2
            
        }
    },
    methods:{
        getCountMethod(){
            console.log('getMethod');
              return this.count * 2
              
        },
        updateCounter(){
            this.count++
        },
        updateCounter2(){
            this.count2++
        }
    }
}
</script>

<style>

</style>