<template>
    <main>
        <section class="container">
                 <ul>
                    <CharacterCard v-for="(card,index) in store.cardList" :key="card.id" :card="card"/>
                </ul>
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
    padding: 85px;
}
ul{
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    justify-items: center;
    justify-content: center;
    text-align: center;
}
.container{
    background-color: white;
    margin: 0 auto;
}
</style>