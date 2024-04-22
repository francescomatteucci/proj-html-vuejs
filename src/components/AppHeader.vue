<template>
    <header>
        <div class="top-header">
            <div>
                <a :href="linkData.url">
                    <img :src="linkData.imageLogo" alt="">
                </a>
            </div>
            <div>
                <a href="" v-html="linkData.plus"></a>
                <a href="" v-html="linkData.menu"></a>
            </div>
        </div>
        <div class="buttons">
            <button>
                <a href="">
                    <i class="fa-solid fa-folder-open"></i>
                    <strong>Demos</strong>
                </a>
            </button>
            <button>
                <a href="">
                    <div><i class="fa-solid fa-dollar-sign"></i><strong>39</strong></div>
                    <strong>On Sale</strong>
                </a>
            </button>
        </div>
        <div class="hero">
            <div class="title">
                <h2>A V A D A</h2>
                <h2>F R E E L A N C E</h2>
            </div>
            <h1>Art Director</h1>
            <div>
                <h4>I F </h4>  
                <h4>I T</h4>
                <h4>D O E S N'T</h4>
                <h4>C H A L L E N G E</h4>
                <h4>Y O U,</h4>
                <h4>I T</h4>
                <h4>D O E S N ' T</h4>
                <h4> C H A N G E</h4>
                <h4>Y O U</h4>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    components: {},
    props: {
        linkData: {
            type: Object,
            required: true,
        }
    }
}
</script>

<style lang="scss" scoped>
@import '/src/style/general';

header {
    background-image: url('imgs/banner_images.jpg');
    background-size: cover; 
    background-position: center; 
    background-repeat: no-repeat; 
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

.buttons {
    display: flex;
    flex-direction: column;
    gap: 6px;
    align-items: end;
    padding-top: 40px;
    padding-bottom: 40px;
    margin-right: 10px;

    a {

        width: 60px;
        color: $dark;
        display: flex;
        flex-direction: column;
        background-color: $white;
        border: 1px transparent;
        border-radius: 4px;
        padding-top: 10px;
        padding-bottom: 10px;
        padding-left: 5px;
        padding-right: 5px;

        i {
            font-size: 24px;
        }
    }

}

.buttons>button:nth-child(2) {

    a {
        color: $green;

        div {
            position: relative;

            i {
                font-size: 14px;
                font-weight: bold;
                position: absolute;
                top: 0;
                left: 0;
            }

            strong {
                font-size: 24px;
            }
        }

        strong {
            font-size: 12px;
        }
    }

    span {
        color: $dark;
    }

}

.hero {
    padding-bottom: 300px;
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
        gap:16px;

        h4 {
            color: $cyan-blue;
            font-weight: lighter;
            text-align: center;
        }
    }

}
</style>