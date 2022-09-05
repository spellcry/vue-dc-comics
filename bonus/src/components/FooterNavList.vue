<template>
    <div class="list-wrapper">
        <h4 class="title">Dc Comics</h4>
        <ul class="nav__list">
            <li class="list__item">Characters</li>
            <li class="list__item">Comics</li>
            <li class="list__item">Movies</li>
            <li class="list__item">Tv</li>
            <li class="list__item">Games</li>
            <li class="list__item">Videos</li>
            <li class="list__item">News</li>
        </ul>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
    @import '../style/variables';

    .list-wrapper {
        .title {
            margin-bottom: 0.3rem;
            font-size: 1.2rem;
            color: $color-white;
        }
        .nav__list {
            display: flex;
            flex-direction: column;
            gap: 0.3rem;
            .list__item {
                font-size: 0.8rem;
                color: #888;
            }
        }
    }
</style>