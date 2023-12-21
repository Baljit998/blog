<template>
<h2>Student Name is : {{ name }}</h2>
</template>

<script>
export default {
    name: 'StudentNew',
    props: {
        name: String
    }
}
</script>
