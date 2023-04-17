<template>
    <div class="col-12 col-sm-6 col-md-4 col-lg-3">
        <div class="card">
            <img class="img-fluid" :src="card.card_images[0].image_url" :alt="card.name">
            <h4>{{ card.name }}</h4>
            <h5>{{ card.archetype }}</h5>
        </div>
    </div>
</template>

<script>
    export default {
        name:'CharacterCard',
        props: ['card']
    }
</script>

<style lang="scss" scoped>
img{
    min-width: 100%;
    max-height: 200px;
    object-fit: contain;
}
.card{
    padding: 50px;
    width: calc(100% / 5);
}

</style>