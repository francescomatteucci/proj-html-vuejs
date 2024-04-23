<template>
    <footer>
        <div class="footer-logo">
            <a :href="linkFooterData.url">
                <img :src="linkFooterData.imageLogo" alt="">
            </a>
        </div>
        <div class="footer-info">
            <span v-html="linkFooterData.copyInfo"></span>
            <span v-html="linkFooterData.themeInfo"></span>
            <a :href="linkFooterData.url">Theme Fusion</a>
            <span v-html="linkFooterData.privacy"></span>
            <span v-html="linkFooterData.powered"></span>
            <a :href="linkFooterData.url">WordPress</a>
        </div>
        <div class="social-icons">
            <button><i class="fa-brands fa-facebook-f"></i></button>
            <button><i class="fa-brands fa-twitter"></i></button>
            <button><i class="fa-brands fa-instagram"></i></button>
            <button><i class="fa-brands fa-youtube"></i></button>
        </div>
    </footer>
</template>

<script>
export default {
    props: {
        linkFooterData: {
            type: Object,
            required: true,
        }
    }
}
</script>

<style lang="scss" scoped>
@import '/src/style/general';

footer {
    background-color: $dark;
    padding-top: 60px;
    padding-bottom: 30px;
    text-align: center;

    .footer-info {
        font-size: 14px;
        padding-top: 30px;

        span {

            color: gray;

        }

        a {
            color: $white;
        }

        i {
            color: $dark;
        }

    }

    .social-icons {
        padding:20px;
            button {
                cursor: pointer;
                padding: 10px;
                border: 1px transparent;
                background-color: $white;
                margin:8px;
                aspect-ratio: 1/1;

                i {
                    color: $dark;
                    font-size: 24px;
                }
            }

        }

}
</style>