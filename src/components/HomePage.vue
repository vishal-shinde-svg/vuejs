<template>
// <!--<h1> Welcome </h1>
// <input tyep="text" placeholder="Enter email" v-model="email">
// <input type="text" placeholder="Enter password" v-model="password ">
// <br>
// <br>
// <button v-on:click="getData()"> Get value</button>-->
<h1> get checkbox and Radio button vlaue </h1>

<h3> technology</h3>
<lable for="java"> java </lable>
<input type="checkbox" vlaue="java" v-model="technology"  id="java"  >

<lable for="vue"> vue </lable>
<input type="checkbox" vlaue="vue " v-model="technology" id="vue" >

<lable for="node"> node </lable>
<input type="checkbox" vlaue="node " v-model="technology"  id="node" >

<h4> selected thechnology{{technology}} </h4>
</template>

<script>
export default {
    name: 'HomePage',
    data() {
        return {
            technology:[] 
        }
    },
}
//     methods: {
//         getData() {
//             console.warn("values : ",this.email , this.password);
//         }
//     }
// }





</script>
