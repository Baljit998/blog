<template>
<div>
    <h3 v-bind="$attrs">Peter</h3>
    <h3>Baljit</h3>
    <h3>Bruce</h3>

</div>
</template>

<script>
export default {
    name: "UserNew",
    props:{
        id:String,
        data:String

    }
}
 
</script>
