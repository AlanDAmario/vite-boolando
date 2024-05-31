<script>
import CardImg from './MainComponents/CardImg.vue';
import products from '../data/db.json'
export default {
    name: 'AppMain',
    components: {
        CardImg,
    },
    data() {
        return {
            products,
        }
    }
}
</script>
<template>
    <main>
        <div class="container">
            <div class="row-flex">
                <div class="col-33" v-for="(product, index) in products.products">
                    <div class="content position-relative ">

                        <img class="main-image" :src="`/img/${product.frontImage}`" alt="modello">
                        <img class="hover-image" :src="`/img/${product.backImage}`" alt="modello">

                        <div class="position-absolute" v-for="badge in product.badges" :class="badge.type">
                            <span> {{ badge.value }}</span>
                        </div>
                        <div class="hearts">
                            <span>&#10084;</span>
                        </div>
                    </div>
                    <div class="text-items">
                        <div class="brand">
                            <span>{{ product.brand }}</span>
                        </div>
                        <div class="stuff">
                            <h5>{{ product.name }}</h5>
                        </div>
                        <div class=" red-price">
                            <span>{{ product.price }}</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
.container {
    max-width: 900px;
    margin: 0 auto;
}

.row-flex {
    display: flex;
    flex-wrap: wrap;
}

.col-33 {
    margin: 50px 10px;
    width: calc(100% / 3 - 20px);
}

.position-relative {
    position: relative;
    top: 25px;
}

.position-absolute {
    position: absolute;
}

.discount {
    background-color: red;
    width: auto;
    left: 0;
    bottom: 60px;
    font-size: 12px;
    color: white;
    text-align: center;
    padding: 3px;
}

.tag {
    background-color: green;
    bottom: 60px;
    font-size: 12px;
    color: white;
    text-align: center;
    width: auto;
    left: 38px;
    padding: 3px;
}

.hearts {
    width: auto;
    padding: 3px;
    position: relative;
    left: 85%;
    bottom: 380px;
}

.hearts:hover {
    padding: 3px;
    display: inline-block;
    color: red;
}

.green-bg-left {
    background-color: green;
    bottom: 60px;
    font-size: 12px;
    color: white;
    text-align: center;
    width: auto;
    left: 0px;
    padding: 3px;
}

.text-items {
    text-align: left;
}

.brand {
    font-size: 12px;
}

.red-price {
    color: red;
    font-size: 12px;
    font-weight: bold;
}


.content:hover .main-image {
    display: none;
}

.content:hover .hover-image {
    display: inline-block;
}

.hover-image {
    display: none;
}

.foot-info-booleano {
    font-weight: bold;
    color: white;
    font-size: 20px;
    padding: 0 10px;
}

.social-info {
    padding: 0 10px;
    font-size: 10px;
    color: white;
    font-weight: bold;
}

.social-logo {
    margin-top: 10px;
    display: flex;
    margin-left: 85%;
    width: 15px;
    filter: invert(100%);
}

.margin-left {
    margin-left: 83%;
}
</style>