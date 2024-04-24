<template>
    <section class="bg-img">
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
    <section class="about-info-wrapper">
        <div class="about-info">
            <h2>About Me</h2>
            <span>UI & UX EXPERT</span>
            <div class="break-line"></div>
        </div>
        <div class="container-lg">
            <div class="row">
                <div class="col-6"><p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Distinctio cum qui sapiente
                    amet et ipsum magnam corporis dolor nam incidunt quasi possimus, debitis ullam totam earum unde
                    quia! Eveniet quos aspernatur saepe, delectus voluptas et neque eum cum unde, itaque nobis
                    inventore, pariatur sapiente! Quod aspernatur veniam expedita id odit.</p></div>
                <div class="col-6"><p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Minima iusto, a veniam
                    libero culpa assumenda sint accusamus nobis ad neque corporis, quos debitis quam quibusdam
                    molestiae! Hic quasi debitis accusamus blanditiis suscipit. Ipsam numquam ipsum saepe dolor, quis
                    aliquam eum velit quia blanditiis fugit sit est possimus nostrum et libero.</p></div>
            </div>
        </div>
    </section>
        <Appskills/>

</template>

<script>
import Appskills from './Appskills.vue';
export default {
    components: {
    Appskills,
  },
}
</script>

<style lang="scss" scoped>
@import '/src/style/general';

.bg-img {
    background-image: url('imgs/banner_images.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    margin-top: -80px;
}

.hero {
    height: 600px;
    display: flex;
    flex-direction: column;
    justify-content: center;

    .title {
        display: flex;
        gap: 20px;
        justify-content: center;

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

.about-info-wrapper {
    background-color:#20232c;
    position: relative;
    margin-bottom: 80px;
    padding-bottom: 80px;

    .about-info {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding-top: 100px;

        h2 {
            padding-bottom: 24px;
        }

    }
    
}

.row {
    display: flex;

}

p{
        color:$cyan-blue
    }


</style>