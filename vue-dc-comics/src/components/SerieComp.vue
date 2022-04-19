<template>
    <div class="serie">
        <div class="box">
            <img :src="details.thumb" alt="Serie Image">
            <h3>{{ details.series }}</h3>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'SerieComp',
        props: ['details']
    }
</script>

<style lang="scss" scooped>
    .serie {
        display: flex;
        flex-basis: calc((100% / 6) - 10px);
        .box {
            background-color: transparent;
            img {
                width: 100%;
                margin-bottom: 10px;
            }
            h3 {
                font-size: 16px;
                font-weight: 400;
                text-transform: uppercase;
            }
        }
    }
</style> 