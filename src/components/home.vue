<template>
<h1 v-on:mousemove ="getConsole()"> welcome </h1>
<button v-on:click="getData()"> click me</button>
<button v-on:dblclick="getData('button double   is clicked')">click me </button>
<input type="text" v-model="count">
<h2>{{count}}</h2>

</template> 


<script>
export default {
    name: "homeComponent",
    data(){
            return{
                count:0
            }
        },

    methods:{
        getData()
        {
            this.count= this.count+1;
        },
        getConsole()
        {
            console.warn("function called.....")
        }
    }

}
</script>
<style scoped>
h1{
    color:red;
}

</style>