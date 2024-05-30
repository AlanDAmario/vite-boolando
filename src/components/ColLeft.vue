<script>
export default {
    name: 'ColLeft',
};
</script>

<template>
    <div class="col">
        <ul>
            <li><a href="*">Donna</a></li>
            <li><a href="§">Uomo</a></li>
            <li><a href="*">Bambini</a></li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
.col {
    width: 25%;
}

ul {
    margin-left: 5%;
}

ul li {
    list-style-type: none;
    text-align: center;
    display: inline-block;
    color: white;
    font-weight: bold;
    font-size: 12px;
}

ul a {
    text-decoration: none;
    color: white;
}

img {
    width: 100%;
}
</style>