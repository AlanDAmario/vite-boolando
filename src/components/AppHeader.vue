<script>
import ColLeft from './ColLeft.vue'
import LogoHead from './LogoHead.vue';
import ColRight from './ColRight.vue';
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
    max-width: 1200px;
    margin: 0 auto;
}

header {
    background-color: rgb(255, 111, 0);
    padding: 20px;
    position: fixed;
    width: 100%;
    z-index: 1;
}


.row-flex {
    display: flex;
    flex-wrap: wrap;
}

.col-100 {
    width: 100%;
}
</style>