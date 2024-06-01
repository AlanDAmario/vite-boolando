<script>
import ColLeft from './HeaderComponents/ColLeft.vue';
import LogoHead from './HeaderComponents/LogoHead.vue';
import ColRight from './HeaderComponents/ColRight.vue';
export default {
    name: 'AppHeader',
    components: {
        ColLeft,
        LogoHead,
        ColRight,
    }
};
</script>

<template>
    <header>
        <div class="container">
            <div class="col-100 row-flex">
                <!-- Coll left -->
                <ColLeft></ColLeft>
                <!-- // LOGO HEADER// -->
                <LogoHead></LogoHead>
                <!-- // COL RIGHT// -->
                <ColRight></ColRight>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
.container {
    max-width: 900px;
    margin: 0 auto;



    .row-flex {
        display: flex;
        flex-wrap: wrap;
    }

    .col-100 {
        width: 100%;
    }

}
</style>