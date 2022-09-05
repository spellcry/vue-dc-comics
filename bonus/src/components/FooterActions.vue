<template>
    <div class="footer__actions">
        <div class="container">
            <button class="cta">Sign-up now!</button>
            <div class="socials">
                Follow us
                <img src="../assets/footer-facebook.png" alt="">
                <img src="../assets/footer-twitter.png" alt="">
                <img src="../assets/footer-youtube.png" alt="">
                <img src="../assets/footer-pinterest.png" alt="">
                <img src="../assets/footer-periscope.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
    @import '../style/variables';
    
    .footer__actions {
        background-color: #303030;
        .container {
            display: flex;
            align-items: center;
            padding-block: 1.5rem;
        }
        .cta {
            padding: 1rem;
            border: 2px solid $color-acc;
            color: $color-white;
            background-color: transparent;
            text-transform: uppercase;
            cursor: pointer;
        }
        .socials {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin-left: auto;
            font-size: 1.4rem;
            font-weight: bold;
            color: $color-acc;
            text-transform: uppercase;
            img {
                cursor: pointer;
            }
        }
    }

</style>