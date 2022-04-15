<template>
    <div class="blue-background">
        <div class="container">
            <div class="col">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital Comix">
                <div class="buy-text">Digital Comix</div>
            </div>
            <div class="col">
                <img src="../assets/img/buy-comics-merchandise.png" alt="Comix Merchandise">
                <div class="buy-text">DC Merchandise</div>
            </div>
            <div class="col">
                <img src="../assets/img/buy-comics-subscriptions.png" alt="Subscription">
                <div class="buy-text">Subscription</div>
            </div>
            <div class="col">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="Comic Shop Locator">
                <div class="buy-text">Comic Shop Locator</div>
            </div>
            <div class="col">
                <img src="../assets/img/buy-dc-power-visa.svg" alt="DC Power Visa">
                <div class="buy-text">DC Power Visa</div>
            </div>
        </div>
    </div>
</template>

<script>
</script>

<style lang="scss" scoped>
    .container {
        display: flex;
    }
    .blue-background {
        display: flex;
        flex-direction: row;
        background-color: #0282f9;
        color: white;
        padding: 40px 0;
    }
    .col {
        display: flex;
        justify-content: center;
        align-items: center;
        width: calc((100% / 5) - 20px);
    }
    img {
        width: 40px;
    }
    .buy-text {
        font-size: 14px;
        text-transform: uppercase;
        margin-left: 10px;
    }
</style>