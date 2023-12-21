<template>
<div class="user">
    <h2>{{ data.name }}</h2>
    <h2>{{ data.email }}</h2>
    <button v-on:click="getData(data.name)">Alert name</button>
</div>

</template>
<script>
export  default{
    name:'userNew',
    props:{
        data:Object,
        getData:Function
    },
}
</script>
<style>
.user{
    background-color: aquamarine;
    padding: 10px;
    border-bottom: 1px solid;
    margin-top: 20px;

}
</style>