<template>
    <div class="skills-wrapper">
        <h2>Why Work With Me</h2>
        <span>WEB - BRANDING - UX/UI</span>
        <div class="break-line"></div>
        <div class="container-lg">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi ipsa amet commodi ex ratione quae nostrum,
                recusandae sit quis debitis? Voluptatibus vero amet iste, error voluptatum atque veritatis tenetur
                tempore
                odit expedita neque consequuntur officiis maxime laudantium eaque pariatur adipisci perferendis?
                Blanditiis,
                molestias totam. Aliquid fugit dolorem rem quaerat eius?</p>
        </div>
    </div>
    <section>
        <div class="work-header-section">
            <h2>Recent Work</h2>
            <span>WEB - BRANDING - UX/UI</span>
            <div class="break-line"></div>
        </div>
    </section>
    <AppCard/>
</template>

<script>
import AppCard from './AppCard.vue';
export default {
   components:{
    AppCard,
   }
}
</script>

<style lang="scss" scoped>
@import '/src/style/general';

.skills-wrapper {
    background-color: #191C23;
    margin-top: -80px;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20px;

    &::after {
        content: '';
        position: absolute;
        bottom: -160px;
        left: 0;
        width: 100%;
        height: 80px;
        background-color: #20232c;
        transform: skewY(2.5deg);
        transform-origin: bottom left;
        z-index: 999;
    }


    h2 {
        padding-top: 200px;

    }

    p {
        color: $cyan-blue;
        text-align: center;
        padding-left: 200px;
        padding-right: 200px;
        padding-bottom: 200px;

    }

}

.work-header-section{
    background-color: $green;
    position: relative;
    display:flex;
    flex-direction: column;
    align-items: center;
    padding-top: 100px;
    &::before {
        content: '';
        position: absolute;
        bottom: 190px;
        left: 0;
        width: 100%;
        height: 80px;
        background-color: $green;
        transform: skewY(-2.5deg);
        transform-origin: bottom left;
        z-index: 999;
    }
}

</style>