<script>
export default {
    
}
</script>
<template >
    <footer>
        <div class="jumbo">
            <div class="container">
                <div class="row d-flex justify-content-start">
                    <div class="col-2">
                        <h3>DC COMICS</h3>
                        <ul class="list-unstyled">
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                        <h3>SHOP</h3>
                        <ul class="list-unstyled">
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                    <div class="col-2">
                        <h3>DC</h3>
                        <ul class="list-unstyled">
                            <li><a href="#">Terms Of Use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Rating</a></li>
                            <li><a href="#">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                        </ul>
                    </div>
                    <div class="col-2">
                        <h3>SITES</h3>
                        <ul class="list-unstyled">
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="bg-grey">
            <div class="container">
                <div class="row">
                    <div class="col">
                        <button type="button" class="btn p-3 my-5">SIGN-UP NOW!</button>
                    </div>
                    <div class="col d-flex align-self-center justify-content-end">
                        <h4>FOLLOW US</h4>
                        <ul class="list-unstyled d-flex">
                            <li><a href="#"><img src="../../public/img/footer-facebook.png" alt="facebook"></a></li>
                            <li><a href="#"><img src="../../public/img/footer-twitter.png" alt="twitter"></a></li>
                            <li><a href="#"><img src="../../public/img/footer-youtube.png" alt="youtube"></a></li>
                            <li><a href="#"><img src="../../public/img/footer-pinterest.png" alt="pinterest"></a></li>
                            <li><a href="#"><img src="../../public/img/footer-periscope.png" alt="periscope"></a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>
<style lang="scss" scoped>
@use '../styles/partials/variables';

    .bg-grey {
        background-color: rgb(45, 45, 45);
        .container {
            .row {
                .col {
                    .btn {
                        border-radius: 0;
                        border: 2px solid variables.$primary_color;
                        color: white;
                        font-weight: bold;
                    }
                    h4 {
                        color: variables.$primary_color;
                        font-weight: bold;
                    }
                    ul {
                        li {
                            margin-left: 20px;
                        }
                    }
                }
            }
        }
    }
    .jumbo {
        background-image: url('../../public/img/footer-bg.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        .row {
            padding-top: 30px;
            padding-bottom: 30px;
            background-image: url('../../public/img/dc-logo-bg.png');
            background-repeat: no-repeat;
            background-position: right;
            .col-2 {
                h3 {
                    color: white;
                    margin: 20px 0;
                }
                ul{
                    li{
                        a{
                            text-decoration: none;
                            color: gray;
    
                            &:hover {
                                color: white;
                            }
                        }
                    }
                }
            }
        }
    }
</style>