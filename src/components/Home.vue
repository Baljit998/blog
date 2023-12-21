<template>
<h1>Non-Props Data</h1>
<UserNew data="some data" xyz="user-cmp" />


</template>

<script>
import UserNew from './User.vue'
export default {
    name: 'HomeComp',
    components:{
        UserNew
    }
 

}
</script>

<style scoped>
h1 {
    color: red
}
</style>
