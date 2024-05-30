<script>
export default {
    name: 'ColRight',
}
</script>

<template>
    <div class="col">
        <div class="logo-contain">
            <a href="*"><img class="logo-inline-block" src="/img/user.png" alt="mini-logo"></a>
            <a href="*"><img class="logo-inline-block" src="/img/shopping-bag.png" alt="mini-logo"></a>
            <a href="*"><img class="logo-inline-block" src="/img/like--v1.png" alt="mini-logo"></a>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.col {
    width: 25%;
}

.logo-inline-block {
    width: 15px;
}

.logo-contain {
    margin-left: 75%;
    filter: invert(100%);
}

.logo-contain a {
    padding: 0 3px;
}

img {
    width: 100%;
}
</style>