<template>
    <div class="card">
        <img class="card__img" :src="imageSrc" alt="title">
        <h4 class="title">{{ title }}</h4>
    </div>
</template>

<script>
export default {
    props: {
        imageSrc: {
            type: String
        },
        title: {
            type: String
        }
    }
}
</script>

<style lang="scss" scoped>
    .card {
        text-align: left;
        cursor: pointer;
        transition: transform 150ms ease-in-out;
        .card__img {
            margin-bottom: 1rem;
            aspect-ratio: 1;
            object-fit: cover;
            object-position: top;
        }
        .title {
            text-transform: uppercase;
            color: #bbb;
        }
        &:hover {
            transform: scale(1.02);
        }
    }
</style>