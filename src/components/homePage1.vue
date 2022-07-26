<template>
<h1> array & array obect</h1>
<ul>
    <li v-for="item in technology" :key="item">
        {{item}}
    </li>>
</ul>

<ul>
    <li v-for="item in user" :key="item.email"> name is :{{item.name}} email is :
    </li>
</ul>
</template>

<script>
export default {
    name: "homePage1",
    data() {
        return {
            technology: ['java', 'php', 'javascript', 'node'],
            user: [{
                    name: "vishal",
                    email: 'vishalshinde09@gmail.com'
                },

                {
                    name: "akshay",
                    email: "ak9@gmail.com"
                }
            ]
        }
    },

}
</script>
