<template>
    <footer class="main-footer">
        <FooterNav/>
        <FooterActions/>
    </footer>
</template>

<script>
import FooterNav from './FooterNav.vue';
import FooterActions from './FooterActions.vue';

export default {
    components: {
        FooterNav,
        FooterActions
    }
}
</script>

<style lang="scss" scoped>

</style>