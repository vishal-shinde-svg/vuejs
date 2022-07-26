<template>
<h1>reusableComponent</h1>
<!-- <h1>{{data}}</h1> -->
<div class="user">
<h2>{{data.name}}</h2>
<h3>{{data.email}}</h3>
<button v-on:click="getData(data.name)">Alert value</button>
</div>

</template>

<script>
export default{
    name:"reusableComponent",
    props:{
        data:Object,
        getData:Function
    },
    
}
</script>
<style>
.user{
    background-color: bisque;
    padding :10px;
    border-bottom:1px solid ;
    margin-bottom: 20px;
}
</style>