<template>
    <div class="container-xxl">
        <div class="row">
            <div class="col-6"><div class="flat">FLAT PICTURE FRAMES</div><img src="../assets/portfolio1_featured_item-400x320.jpg" alt=""></div>
            <div class="col-6"><div class="flat">FLAT PICTURE FRAMES</div><img src="../assets/portfolio2_featured_item-800x640.jpg" alt=""></div>
            <div class="col-6"><div class="flat">FLAT PICTURE FRAMES</div><img src="../assets/portfolio3_featured_item-400x320.jpg" alt=""></div>
            <div class="col-6"><div class="flat">FLAT PICTURE FRAMES</div><img src="../assets/portfolio4_featured_item-400x320.jpg" alt=""></div>
            <div class="col-6"><div class="flat">FLAT PICTURE FRAMES</div><img src="../assets/portfolio5_featured_item-400x320.jpg" alt=""></div>
            <div class="col-6"><div class="flat">FLAT PICTURE FRAMES</div><img src="../assets/portfolio6_featured_item-800x640.jpg" alt=""></div>
        </div>
    </div>
    <div class="container-xxl">
        <button><span>VIEW ALL WORK</span></button>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
@import '/src/style/general';
.row{
    display: flex;
    flex-wrap: wrap;
}
img{
    aspect-ratio: 1/1;
    width: 100%;
}
button{
    background-color: $red;
    width:100%;
    height:100px;
    cursor: pointer;
    transition: background-color 0.6s ease-in;

    
}
button:hover{
    background-color: $white;
        span{
            color: $red;
        }
}
span{
    letter-spacing: 2px;
    text-align: center;
    color: $white;
}

.flat{
    display:none;
}

.col-6:hover{
    display:flex;
    justify-content: center;
    align-items: center;
    background-color: rgb(249, 61, 97);
    .flat{
        display:block;
        position: absolute;
        color:$white;
        z-index: 999;
        font-size: 20px;
        
    }
    img{
        position:relative;
        opacity: 0.5;
        transition: opacity 0.5s ease-in;
    }
    
}
</style>