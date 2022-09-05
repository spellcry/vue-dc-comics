<template>
    <header class="main-header">
        <div class="container">
            <div class="logo">
                <img src="../assets/dc-logo.png" alt="">
            </div>
            <nav class="nav">
                <ul class="nav__list">
                    <li class="list__item">Characters</li>
                    <li class="list__item active">Comics</li>
                    <li class="list__item">Movies</li>
                    <li class="list__item">Tv</li>
                    <li class="list__item">Games</li>
                    <li class="list__item">Collectibles</li>
                    <li class="list__item">Videos</li>
                    <li class="list__item">Fans</li>
                    <li class="list__item">News</li>
                    <li class="list__item">Shop</li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
    @import '../style/variables';
    
    .main-header {

        .container {
            display: flex;
            align-items: center;
            .nav {                
                margin-left: auto;
                .nav__list {
                    display: flex;
                    gap: 2rem;
                    .list__item {
                        padding-block: 4rem;
                        text-transform: uppercase;
                        font-weight: bold;
                        font-size: 0.85rem;
                        &.active, &:hover {
                            color: $color-acc;
                            border-bottom: 5px solid $color-acc;
                        }
                    }
                }
            }
        }
    }

</style>