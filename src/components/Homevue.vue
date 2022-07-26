<template>
<h1>Welcome {{"hello" . length}}</h1>
<h2> hello {{email}} </h2>
<h1> hi {{mobile=9970710108}} </h1>
<h1> new number {{mobile==true}} </h1>

<h1> name {{getName("vishal")}} </h1>

<h1> name {{getData()}} </h1>  
<h1> name {{getData().name}} </h1>
<h1> email {{email}} </h1>
</template>

<script>
export default {
    name: "Homevue",
    data() {
        return {
            email: 'vishalshinde@gamil.com',
            mobile: 9970215151

        }
    },

    methods: {
        getName(name) {
            return name;
        },
        getData() {
            return {
                name: "shinde vishal",
                email: this.email,

            }
        }
    }

}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>
