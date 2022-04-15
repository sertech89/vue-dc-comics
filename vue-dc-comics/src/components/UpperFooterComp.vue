<template>
    <div class="upper-footer">
        <div class="container">
            <div class="upper-footer-content">
                <!-- Footer Menus -->
                <div class="footer-menus">
                    <div class="col">
                        <h4>DC COMICS</h4>
                        <ul>
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Comics</a>
                            </li>
                            <li>
                                <a href="#">Movies</a>
                            </li>
                            <li>
                                <a href="#">TV</a>
                            </li>
                            <li>
                                <a href="#">Games</a>
                            </li>
                            <li>
                                <a href="#">Videos</a>
                            </li>
                            <li>
                                <a href="#">News</a>
                            </li>
                        </ul>

                        <h4>SHOP</h4>
                        <ul>
                            <li>
                                <a href="#">Shop DC</a>
                            </li>
                            <li>
                                <a href="#">Shop DC Collectibles</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col">
                        <h4>DC</h4>
                        <ul>
                            <li>
                                <a href="#">Terms of Use</a>
                            </li>
                            <li>
                                <a href="#">Privacy policy (New)</a>
                            </li>
                            <li>
                                <a href="#">Ad Choices</a>
                            </li>
                            <li>
                                <a href="#">Advertising</a>
                            </li>
                            <li>
                                <a href="#">Jobs</a>
                            </li>
                            <li>
                                <a href="#">Subscription</a>
                            </li>
                            <li>
                                <a href="#">Talent Workshop</a>
                            </li>
                            <li>
                                <a href="#">CPSC Certificates</a>
                            </li>
                            <li>
                                <a href="#">Ratings</a>
                            </li>
                            <li>
                                <a href="#">Shop Help</a>
                            </li>
                            <li>
                                <a href="#">Contact Us</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col">
                        <h4>SITES</h4>
                        <ul>
                            <li>
                                <a href="#">DC</a>
                            </li>
                            <li>
                                <a href="#">MAD Magazine</a>
                            </li>
                            <li>
                                <a href="#">DC Kids</a>
                            </li>
                            <li>
                                <a href="#">DC Universe</a>
                            </li>
                            <li>
                                <a href="#">DC Power Visa</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <!-- Footer Logo -->
                <div class="footer-logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="DC Logo">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
</script>

<style scoped>
    .upper-footer-content {
        display: flex;
        justify-content: space-between;
        overflow: hidden;
    }
    .upper-footer {
        background-image: url('../assets/img/footer-bg.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        height: 90vh;
        padding: 20px 0;
        color: white;
        overflow: hidden;
    }
    .footer-menus {
        width: 50%;
    }
    .footer-logo {
        width: 50%;
    }
    .footer-menus ul {
        list-style-type: none;
        display: flex;
        flex-direction: column;
        text-transform: none;
        padding: 0;
    }
    .col {
        width: calc(100% / 3);
        height: 100%;
        float: left;
    }
    a {
        text-decoration: none;
        color: gray;
        font-size: 14px;
    }
    img {
        margin-left: 60px;
        width: 450px;
    }
</style>