<template>
    <div class="cards">
        <div class="current-series">
            Current Series
        </div>
        <ul class="cards__list">
            <li v-for="(card, index) in cards" :key="index" class="list__item">
                <Card :imageSrc="card.thumb" :title="card.series"/>
            </li>
        </ul>
    </div>
</template>

<script>
    import Card from './CardComponent.vue';
    import cards from '../data';

    export default {
        data() {
            return {
                cards,
            }
        },
        components: {
            Card
        }
    }
</script>

<style lang="scss" scoped>
    @import '../style/variables';
    @import '../style/mixins';

    .cards {
        position: relative;
        @include paddingBlock;
        .current-series {
            position: absolute;
            top: 0;
            padding: 0.5rem 1rem;
            transform: translateY(-50%);
            background-color: $color-acc;
            text-transform: uppercase;
            font-weight: bold;
        }
        .cards__list {
            display: flex;
            flex-wrap: wrap;
            gap: 3rem 1.5rem;
            padding-inline: 1rem;
            .list__item {
                flex-basis: calc(calc(100% - 1.5rem * 5) / 6);
            }
        }
    }
</style>