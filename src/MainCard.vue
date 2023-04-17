<template>
    <main>
        <section class="container">
            <div class="row">
                <div class="cards">
                    <ul>
                         <CharacterCard v-for="(card,index) in store.cardList" :key="card.id" :card="card"/>
                    </ul>
                </div>
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
ul{
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    text-align: center;
    justify-content: center;
}


</style>