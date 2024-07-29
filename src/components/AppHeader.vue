<script>
export default {
    
}
</script>
<template>
    <header>
        <div class='container'>
            <div class='row'>
                <div class='col-3'>
                    <img src="../../public/img/dc-logo.png" alt="logoDC">
                </div>
                <div class='col-9 align-self-center'>
                    <ul class="list-unstyled">
                        <li>
                            <a href="#">characters</a>
                        </li>
                        <li>
                            <a href="#">comics</a>
                        </li>
                        <li>
                            <a href="#">movies</a>
                        </li>
                        <li>
                            <a href="#">tv</a>
                        </li>
                        <li>
                            <a href="#">games</a>
                        </li>
                        <li>
                            <a href="#">collectibles</a>
                        </li>
                        <li>
                            <a href="#">videos</a>
                        </li>
                        <li>
                            <a href="#">fans</a>
                        </li>
                        <li>
                            <a href="#">news</a>
                        </li>
                        <li>
                            <a href="#">shop</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>
<style lang="scss">
@use '../styles/partials/variables';


img {
    margin: 10px 0;
}

ul {
    display: flex;
    justify-content: flex-end;

    li {
        padding: 20px 15px;

        a {
            text-decoration: none;
            color: black;
            font-weight: bold;
            padding-bottom: 50px;
            text-transform: uppercase;

            &:hover {
                color: variables.$primary-color;
                border-bottom: 5px solid variables.$primary-color;
            }
        }
    }
}
</style>