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
                <div class="col-6">
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Distinctio cum qui sapiente
                        amet et ipsum magnam corporis dolor nam incidunt quasi possimus, debitis ullam totam earum unde
                        quia! Eveniet quos aspernatur saepe, delectus voluptas et neque eum cum unde, itaque nobis
                        inventore, pariatur sapiente! Quod aspernatur veniam expedita id odit.</p>
                </div>
                <div class="col-6">
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Minima iusto, a veniam
                        libero culpa assumenda sint accusamus nobis ad neque corporis, quos debitis quam quibusdam
                        molestiae! Hic quasi debitis accusamus blanditiis suscipit. Ipsam numquam ipsum saepe dolor,
                        quis
                        aliquam eum velit quia blanditiis fugit sit est possimus nostrum et libero.</p>
                </div>
            </div>
        </div>
    </section>
    <Appskills />
    <section class="trust-section">
        <img src="../assets/quotes-1.png" alt="">
        <p>"That's been one of my mantras - focus and simplicity. Simple can be harder than complex; you have to work
            hard to get your thinking clean to make it simple."</p>
        <strong>STEVE JOBS - APPLE</strong>
        <span>TRUSTED BY GLOBAL BRANDS</span>
        <div class="container-xxl">
            <div class="row">
                <div><img src="../assets/lorem.png" alt=""></div>
                <div><img src="../assets/america.png" alt=""></div>
                <div><img src="../assets/gerrard.png" alt=""></div>
                <div><img src="../assets/roodney.png" alt=""></div>
                <div><img src="../assets/zanneti.png" alt=""></div>
            </div>
        </div>

    </section>
    <section class="device-section">
        <h2>Expert Design Advice</h2>
        <span>TRENDING DESIGN NEWS</span>
        <div class="break-line"></div>
    </section>
    <AppCard/>
</template>

<script>
import Appskills from './Appskills.vue';
import AppCard from './AppCard.vue';
export default {
    components: {
        Appskills,
        AppCard,

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
    background-color: #20232c;
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

p {
    color: $cyan-blue
}

.trust-section {
    position: relative;
    background-image: url('../assets/testimonial_bkgd.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20px;

    img {
        padding-top: 140px;
    }

    i {
        color: $red;
        font-size: 100px;
        padding-top: 100px;
    }

    p {
        color: $white;
        font-style: italic;
    }

    strong {
        letter-spacing: 1px;
        color: $white;
        margin-top: 20px;
        margin-bottom: 200px;
    }

    span {
        color: $white;
        letter-spacing: 2px;
    }

    .container-xxl {
        .row {

            display: flex;
            justify-content: center;
            gap: 100px;

            div {
                width: 120px;
                padding-bottom: 140px;
            }
        }

    }

}

.trust-section::after {
    content: '';
    position: absolute;
    bottom: -60px;
    left: 0;
    width: 100%;
    height: 80px;
    background-image: url('../assets/testimonial_bkgd.jpg');
    background-position: bottom;
    transform: skewY(-2deg);
    transform-origin: bottom left;
    z-index: 999;
}

.device-section{
    background-color:#49629B;
    display:flex;
    flex-direction: column;
    align-items: center;
    padding-top: 100px;
    span{
        letter-spacing: 4px;
        color:white;
        padding:20px;
    }

}
</style>