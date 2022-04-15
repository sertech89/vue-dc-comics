<template>
    <div>
        <div class="bottom-footer">
            <div class="container">
                <div class="bottom-footer-content">
                    <!-- Sign Up -->
                    <div class="sign-up">
                        <a class="btn btn-trans" href="#">SIGN-UP NOW!</a>
                    </div>

                    <!-- Follow -->
                    <div class="follow">
                        <span class="follow-us">FOLLOW US</span>
                        <div class="social-icons">
                            <img src="../assets/img/footer-facebook.png" alt="Facebook">
                            <img src="../assets/img/footer-twitter.png" alt="Twitter">
                            <img src="../assets/img/footer-youtube.png" alt="Youtube">
                            <img src="../assets/img/footer-pinterest.png" alt="Pinterest">
                            <img src="../assets/img/footer-periscope.png" alt="Periscope">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
</script>

<style scoped>
    .bottom-footer {
        background-color: #303030;
        padding: 30px 0;
    }
    .bottom-footer-content {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    
    a {
        text-decoration: none;
    }
    .btn {
        padding: 10px;
        font-weight: bold;
        font-size: 17px;
    }
    .btn-trans {
        color: white;
        background-color: transparent;
        border: 3px solid #0282f9;
    }
    .follow {
        display: flex;
    }
    .follow-us {
        color: #0282f9;
        font-weight: bold;
        font-size: 20px;
    }
    .social-icons {
        margin-left: 30px;
    }
    .social-icons img {
        margin: 0 10px;
    }
</style>