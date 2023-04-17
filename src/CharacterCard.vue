<template>
    <div class="col-12 col-sm-6 col-md-4 col-lg-3">
        <div class="card">
            <img class="img-fluid card-img" :src="card.card_images[0].image_url" :alt="card.name">
            <div class="text-card">
                <h4>{{ card.name }}</h4>
                <h5 class="arche">{{ card.archetype }}</h5>
            </div>
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

.card{
    padding: 20px;
    width: calc(100% / 5);
    text-align: center;
    justify-content: center;
    justify-items: center;
}
.card-img{
    min-width: 100%;
    max-height: 200px;
    object-fit: contain;
}
.text-card{
    width: 140px;
    height: 140px;
    background-color: goldenrod;
    color: white;
}
.arche{
    color: black;
    float: inline-end;
}
</style>