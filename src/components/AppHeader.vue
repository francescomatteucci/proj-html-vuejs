<template>
    <header>
        <div class="top-header">
            <div>
                <a :href="linkHeaderData.url">
                    <img :src="linkHeaderData.imageLogo" alt="">
                </a>
            </div>
            <div>
                <a href="" v-html="linkHeaderData.plus"></a>
                <a href="" v-html="linkHeaderData.menu"></a>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    components: {},
    props: {
        linkHeaderData: {
            type: Object,
            required: true,
        }
    }
}
</script>

<style lang="scss" scoped>
@import '/src/style/general';

header {
    
    a {
        color: $white;
    }

    .top-header {
        display: flex;
        align-items: center;
        justify-content: space-between;
        height: 80px;
        margin-left: 60px;
        margin-right: 60px;

    }
}


.top-header>div:nth-child(2) {

    a {
        padding: 14px;
        font-size: 24px;
    }
}

</style>