<template>
    <aside class="main-sidebar">
        <div class="container">
            <ul class="aside__list">
                <li v-for="(widget, index) in sidebarWidget" :key="index" class="list__item">
                    <SidebarWidget :imageSrc="widget.imageSrc" :href="widget.href" :text="widget.text"/>               
                </li>                
            </ul>
        </div>
    </aside>
</template>

<script>
    import SidebarWidget from './SidebarWidget.vue';

    export default {
        data() {
            return {
                sidebarWidget: [
                    {
                        imageSrc: require('../assets/buy-comics-digital-comics.png'),
                        text: 'Digital Comics',
                        href: '#'
                    },
                    {
                        imageSrc: require('../assets/buy-comics-merchandise.png'),
                        text: 'Dc Merchandise',
                        href: '#'
                    },
                    {
                        imageSrc: require('../assets/buy-comics-subscriptions.png'),
                        text: 'Subscription',
                        href: '#'
                    },
                    {
                        imageSrc: require('../assets/buy-comics-shop-locator.png'),
                        text: 'Comic Shop Locator',
                        href: '#'
                    },
                    {
                        imageSrc: require('../assets/buy-dc-power-visa.svg'),
                        text: 'Dc Power Visa',
                        href: '#'
                    },
                ]
            }
        },
        components: {
            SidebarWidget
        }
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
            }
        }
    }
</style>