<template>
    <a :href="href">
        <img :src="imageSrc" alt="">
        {{ text }}
    </a> 
</template>

<script>
    export default {
        props: {
            imageSrc: String,
            href: String,
            text: String
        }    
    }
</script>
<style lang="scss" scoped>
    @import '../style/variables';

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
</style>