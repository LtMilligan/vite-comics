<script>
export default {
    
}
</script>
<template>
    <main>
        <div class="bg-grey p-5">
            <div class="container">
                <div class="row content-grey">
                    <div class="col-12 align-self-center">
                        <p>--- Content goes here ---</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="bg-primary p-5">
            <div class="container">
                <div class="row content-primary justify-content-evenly">
                    <div class="col-2">
                        <img src="../../public/img/buy-comics-digital-comics.png" alt="digital-comics">
                        <p>DIGITAL COMICS</p>
                    </div>
                    <div class="col-2">
                        <img src="../../public/img/buy-comics-merchandise.png" alt="merch">
                        <p>DC MERCHANDISE</p>
                    </div>
                    <div class="col-2">
                        <img src="../../public/img/buy-comics-subscriptions.png" alt="sub">
                        <p>SUBSCRIPTION</p>
                    </div>
                    <div class="col-2">
                        <img src="../../public/img/buy-comics-shop-locator.png" alt="locator">
                        <p>COMIC SHOP LOCATOR</p>
                    </div>
                    <div class="col-2">
                        <img src="../../public/img/buy-dc-power-visa.svg" alt="visa">
                        <p>DC POWER VISA</p>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>
<style lang="scss">
@use '../styles/partials/variables';

    .bg-grey {
        background-color: rgb(39, 39, 39);
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

    .col-2 {
        align-self: center;

        img {
            max-width: 50px;
            max-height: 50px;
        }

        p {
            display: inline-block;
            margin-left: 10px;
            margin-bottom: 0;
            font-size: 14px;
        }
    }
</style>