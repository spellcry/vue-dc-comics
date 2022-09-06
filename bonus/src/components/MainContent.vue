<template>
    <main class="main-content">
        <Hero/>
        <div class="container">
            <Cards/>
            <button class="load-more">
                Load more
            </button>
        </div>
    </main>
</template>

<script>
import Hero from './HeroComponent.vue';
import Cards from './CardsComponent.vue';

export default {
    components: {
        Hero,
        Cards
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/variables';
    
    .main-content {
        background-color: $color-dark;
        color: $color-white;
        .container {
            text-align: center;
            .load-more {
                padding: 0.8rem 4rem;
                margin-bottom: 1rem;
                border: none;
                background-color: $color-acc;
                color: $color-white;
                font-weight: bold;
                font-size: 0.85rem;
            }
        }
    }

</style>