<template>
    <header>
        <img class="img-fluid" src="https://occ-0-2433-1001.1.nflxso.net/dnm/api/v6/LmEnxtiAuzezXBjYXPuDgfZ4zZQ/AAAABdpYalFU9SD9K6dNwu9SlKsNaQ3AIGWFrN_uDy6R7N3TS5DHIatIETtgeqwC0kM01zJyor2znGql_ixTWzVueA-GllV7Hn03ygETN_Nd7oZA.png?r=81f" alt="yugioh">
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
img{
    width: 10%;
}
header{
    display: flex
}

</style>