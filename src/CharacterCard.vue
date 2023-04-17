<template>
    <div class="col-12 col-sm-6 col-md-4 col-lg-3">
        <img :src="card.card_images[0].image_url" :alt="card.name">
        <h4>{{ card.name }}</h4>
        <h5>{{ card.archetype }}</h5>

    </div>
</template>

<script>
    export default {
        name:'CharacterCard',
        props: ['card']
    }
</script>

<style lang="scss" scoped>

</style>