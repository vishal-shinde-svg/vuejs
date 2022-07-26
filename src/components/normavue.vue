<template>
<!-- <HelloWorld msg="Welcome to Your Vue.js App" />
<homePage2  :user="user" :getData="getData"/> -->
<ul>
  <li v-for="item in user" :key="item.name">
  <reusableComponent :data="item"  :getData="getData"/>
  <!-- {{item.name}}
  {{item}} -->
  </li>
</ul>


</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'


// import homePage2 from './components/homePage2.vue'


 
import reusableComponent from './components/reusableComponent.vue'
export default {
    name: 'App',
    components: {
    // HelloWorld,
    // homePage2
    reusableComponent,
    
// },
// data(){
//   return{
//     user:[{name:"vishal", email:"shinde05@gmail.com"}]
//   }
// },
// methods:{
//   getData()
//   {
//     alert("Hello")
  },
  methods:{
        getData(name){
            alert(name)
        }
    },
  data()
  {
    return{
      user:[{name:"vishal" , email:"shindev@gmail.com"},
            {name:"akshay", email:"vishal@gmail.com"},
            {name:"hi",emai:"shinde@gmail.com"}
      ]
    }
  }
 }



</script>
