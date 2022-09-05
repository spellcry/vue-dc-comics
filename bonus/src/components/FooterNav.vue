<template>
    <div class="footer__nav">
        <div class="container">
            <FooterNavList/>
            <FooterNavList/>
            <FooterNavList/>
            <FooterNavList/>
        </div>
    </div>
</template>

<script>
import FooterNavList from './FooterNavList.vue';

export default {
    components: {
        FooterNavList
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/mixins';

    .footer__nav {
        background-image: url('../assets/footer-bg.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        .container {
            display: flex;
            flex-direction: column;
            flex-wrap: wrap;
            align-content: flex-start;
            gap: 2rem;
            max-height: 500px;
            @include paddingBlock;
            background-image: url('../assets/dc-logo-bg.png');
            background-repeat: no-repeat;
            background-position: center right;
        }
    }

</style>