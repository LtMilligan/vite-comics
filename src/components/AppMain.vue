<script>
import comics from '../data/dc-comics.json'
export default {
    data() {
        return {
            comics
        }
    }
}
</script>
<template>
    <main>
        <div class="bg-jumbotron position-relative">
            <span class="badge position-absolute rounded-0">CURRENT SERIES</span>
        </div>
        <div class="bg-grey p-5">
            <div class="container">
                <div class="row content-grey d-flex">
                    <div class="col-2 d-flex" v-for="(comic, index) in comics" :key="index">
                        <div class="card border-0 bg-transparent w-100 mx-3">
                            <img :src="comic.thumb" :alt="comic.series" class="card-img-top img-fluid">
                            <div>
                                <h5 class="text-white text-center pt-2">{{ comic.series }}</h5>
                            </div>
                        </div>
                    </div>
                    <div class="text-center">
                        <button class="btn btn-primary w-auto px-5 rounded-0"><strong>LOAD MORE</strong></button>
                    </div>
                </div>
            </div>
        </div>
        <div class="bg-primary p-5">
            <div class="container">
                <div class="row content-primary justify-content-between">
                    <div class="col">
                        <img src="../../public/img/buy-comics-digital-comics.png" alt="digital-comics">
                        <p>DIGITAL COMICS</p>
                    </div>
                    <div class="col">
                        <img src="../../public/img/buy-comics-merchandise.png" alt="merch">
                        <p>DC MERCHANDISE</p>
                    </div>
                    <div class="col">
                        <img src="../../public/img/buy-comics-subscriptions.png" alt="sub">
                        <p>SUBSCRIPTION</p>
                    </div>
                    <div class="col">
                        <img src="../../public/img/buy-comics-shop-locator.png" alt="locator">
                        <p>COMIC SHOP LOCATOR</p>
                    </div>
                    <div class="col">
                        <img src="../../public/img/buy-dc-power-visa.svg" alt="visa">
                        <p>DC POWER VISA</p>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>
<style lang="scss" scoped>
@use '../styles/partials/variables';

    .bg-jumbotron {
        background-image: url(../../public/img/jumbotron.jpg);
        background-repeat: no-repeat;
        height: 450px;

        .badge {
            background-color: variables.$primary_color;
            font-size: 30px;
            padding: 14px 40px;
            bottom: -25px;
            left: 190px;
        }
    }

    .bg-grey {
        background-color: rgb(39, 39, 39);
    }

    .card {
        img {
            width: 200px;
            height: 250px;
        }
    }

    .bg-primary {
        background-color: variables.$primary_color;
    }
    .content-grey {
        color: white;
    }
    .content-primary {
        color: white;
    }
    .col-12 {
        p {
            margin: 0;
            font-size: 30px;
        }
    }

    .col {
        align-self: center;
        text-align: center;

        img {
            max-width: 60px;
            max-height: 60px;
        }

        p {
            display: inline-block;
            margin-left: 10px;
            margin-bottom: 0;
            font-size: 16px;
        }
    }
</style>