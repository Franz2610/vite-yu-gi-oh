<template>
    <main>
        <section class="container">
            <div class="row">
                <CharacterCard v-for="(card,index) in store.cardList" :key="card.id" :card="card"/>
            </div>
        </section>
    </main>
</template>

<script>
import { store } from './store';
import CharacterCard from './CharacterCard.vue';
    export default {
        name:'MainCard',
        components: {
            CharacterCard
        },
        data() {
            return {
                store
            }
        }
        
    }
</script>

<style lang="scss" scoped>
main{
    background-color: goldenrod;
}

</style>