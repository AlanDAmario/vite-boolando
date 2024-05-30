<script>

import ColLeft from './ColLeft.vue';
export default {
    name: 'AppHeader',
};
</script>

<template>
    <header>
        <div class="container">
            <div class="row-flex">
                <div class="col-100 row-flex">
                    <!-- Coll left -->
                    <ColLeft></ColLeft>
                    <!-- // LOGO HEADER// -->
                    <!-- // COL RIGHT// -->
                    <div class="col-50">
                        <img class="logo" src="./boolean-logo.png" alt="logo">
                    </div>
                    <div class="col-25">
                        <div class="logo-contain">
                            <a href="*"><img class="logo-inline-block" src="./img/user.png" alt="mini-logo"></a>
                            <a href="*"><img class="logo-inline-block" src="./img/shopping-bag.png" alt="mini-logo"></a>
                            <a href="*"><img class="logo-inline-block" src="./img/like--v1.png" alt="mini-logo"></a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>

* {
    margin: 0 auto;
    padding: 0;
    box-sizing: border-box;

}

body {
    font-family: Arial, Helvetica, sans-serif;
    overflow-x: hidden;
}

header {
    background-color: rgb(255, 111, 0);
    padding: 20px;
    position: fixed;
    width: 100%;
    z-index: 1;
}

.col-25 {
    width: 25%;
}

.row-flex {
    display: flex;
    flex-wrap: wrap;
}

.col-25 {
    width: 25%;

}

.col-50 {
    width: 50%;
}

.logo {
    width: 95px;
    display: inline-block;
    margin-left: 35%;
}

.logo-inline-block {
    width: 15px;
}

.logo-contain {
    margin-left: 75%;
    filter: invert(100%);
}

img {
    width: 100%;
}
</style>