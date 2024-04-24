<template>
    <div>
        <div class="container-xxl">
            <div class="row">
                <div class="col-4">
                    <div class="card-header">
                        <img src="../assets/blog3-featured-600x400.jpg" alt="">
                    </div>
                    <div class="card-body">
                        <h3>Live The Design Process</h3>
                        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Necessitatibus voluptatem
                            consectetur
                            incidunt quisquam tempora ratione, distinctio expedita perferendis, molestias fuga in ad ea
                            dolor provident! Molestias nemo exercitationem facilis velit.</p>
                    </div>
                </div>
                <div class="col-4">
                    <div class="card-header">
                        <img src="../assets/blog3-featured-600x400.jpg" alt="">
                    </div>
                    <div class="card-body">
                        <h3>Live The Design Process</h3>
                        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Necessitatibus voluptatem
                            consectetur
                            incidunt quisquam tempora ratione, distinctio expedita perferendis, molestias fuga in ad ea
                            dolor provident! Molestias nemo exercitationem facilis velit.</p>
                    </div>
                </div>
                <div class="col-4">
                    <div class="card-header">
                        <img src="../assets/blog3-featured-600x400.jpg" alt="">
                    </div>
                    <div class="card-body">
                        <h3>Live The Design Process</h3>
                        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Necessitatibus voluptatem
                            consectetur
                            incidunt quisquam tempora ratione, distinctio expedita perferendis, molestias fuga in ad ea
                            dolor provident! Molestias nemo exercitationem facilis velit.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '/src/style/general';

.row {
    display: flex;

    .col-4 {
        background-color: $dark;

        .card-body{
            padding-left: 14px;
            padding-right: 14px;

        }
        h3 {
            color: $red;
        }

        p {
            color: $cyan-blue;
            line-height: 2;
        }
    }
}
</style>