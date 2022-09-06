<template>
    <div class="list-wrapper">
        <h4 class="title">{{ listLinks.title }}</h4>
        <ul class="nav__list">
            <li v-for="(link, index) in listLinks.links" :key="index" class="list__item"><a :href="link.href">{{ link.text }}</a></li>
        </ul>
    </div>
</template>

<script>

export default {
    props: {
        listLinks: {
            type: Object
        }
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/variables';

    .list-wrapper {
        .title {
            margin-bottom: 0.3rem;
            font-size: 1.2rem;
            color: $color-white;
            text-transform: uppercase;
        }
        .nav__list {
            display: flex;
            flex-direction: column;
            gap: 0.3rem;
            .list__item {
                a {
                    font-size: 0.8rem;
                    color: #888;
                }
            }
        }
    }
</style>