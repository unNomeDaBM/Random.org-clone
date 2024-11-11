<template>
    <a href="">
        <slot></slot>
    </a>
</template>

<script>
    export default{
        props:["linkName"]
    }
</script>

<style scoped>
    *{
        padding: 0;
        border: 0;
        margin: 0;
    }
    a{
        font-family: sans-serif;
        font-size: 0.59em;
        font-weight: 800;
    }
</style>