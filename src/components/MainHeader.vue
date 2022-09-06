<template>
    <header class="main-header">
        <div class="container">
            <div class="logo">
                <img src="../assets/dc-logo.png" alt="">
            </div>
            <nav class="nav">
                <ul class="nav__list">                
                    <li v-for="(link, index) in links" :key="index" class="list__item"><a :href="link.href">{{ link.title }}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
import { links } from '../data';

export default {
    data() {
        return {
            links
        }
    }
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
                        border-bottom: 5px solid transparent;                    
                        &.active, &:hover {
                            color: $color-acc;
                            border-bottom-color: $color-acc;
                        }
                        a {
                            color: $color-dark;
                        }
                    }
                }
            }
        }
    }

</style>