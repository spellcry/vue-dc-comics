<template>
    <aside class="main-sidebar">
        <div class="container">
            <ul class="aside__list">
                <li class="list__item">
                    <a href="#">
                        <img src="../assets/buy-comics-digital-comics.png" alt="">
                        Digital Comics
                    </a>
                </li>
                <li class="list__item">
                    <a href="#">
                        <img src="../assets/buy-comics-merchandise.png" alt="">
                        Dc Merchandise
                    </a>
                </li>
                <li class="list__item">
                    <a href="#">
                        <img src="../assets/buy-comics-subscriptions.png" alt="">
                        Subscription
                    </a>
                </li>
                <li class="list__item">
                    <a href="#">
                        <img src="../assets/buy-comics-shop-locator.png" alt="">
                        Comic Shop Locator
                    </a>
                </li>
                <li class="list__item">
                    <a href="#">
                        <img src="../assets/buy-dc-power-visa.svg" alt="">
                        Dc Power Visa
                    </a>
                </li>
            </ul>
        </div>
    </aside>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
    @import '../style/variables';
    @import '../style/mixins';

    .main-sidebar {
        background-color: $color-acc;
        color: $color-white;
        @include paddingBlock;
        .aside__list {
            display: flex;
            justify-content: space-around;
            .list__item {
                flex-basis: 15%;
                a {
                    display: flex;
                    align-items: center;       
                    height: 100%;    
                    white-space: nowrap;    
                    color: $color-white;
                    text-transform: uppercase;
                    font-size: 0.85rem;
                    img {
                        max-width: 50px;
                        max-height: 50px;
                        margin-right: 1rem;
                    }
                }
            }
        }
    }
</style>