<template>
    <header>
        <h1 class="text-black"> {{ title }}</h1>
    </header>
</template>

<script>
    export default {
        name:'HeaderApp',
        props :{
            title: String
        }
    }
</script>

<style lang="scss" scoped>

</style>