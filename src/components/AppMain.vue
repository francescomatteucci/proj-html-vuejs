<template>
    <section>
        <div class="hero">
            <div class="title">
                <h2>A V A D A</h2>
                <h2>F R E E L A N C E</h2>
            </div>
            <h1>Art Director</h1>
            <div>
                <h4>IF IT DOESN'T CHALLENGE YOU, IT DOESN'T CHANGE YOU</h4>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
@import '/src/style/general';
.hero {
    height: 600px;
    display: flex;
    flex-direction: column;
    justify-content: center;

    .title {
        display: flex;
        gap: 20px;
        justify-content: center;

        h2 {
            color: $white;
        }

    }

    h1 {
        color: $red;
        font-size: 120px;
        text-align: center;
    }

    div {
        display: flex;
        justify-content: center;
        gap: 16px;

        h4 {
            color: $cyan-blue;
            font-weight: lighter;
            text-align: center;
            letter-spacing: 2px;
        }
    }

    
}
</style>