<template>
<h2>{{user}}</h2>
<h1>{{user.name}}</h1>
<button v-on:click="getData()"> click me</button>

</template>

<script>
export default {
    name: "homePage2",
    props:{
        name:String,
        user:Object,
        getData:Function
     },
}

</script>
