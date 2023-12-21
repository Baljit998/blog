<template>
    <h2>Teacher Name is: {{ name }}</h2>
    </template>
    <script>
    export default{
        name:'TeacherNew',
        props: {
        name: String
    }
    }
    </script>