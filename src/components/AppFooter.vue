<script>
export default {
    name: 'AppFooter'
}
</script>
<template>
    <footer>

        <div class="container">
            <div class="row-flex">
                <div class="col-100 row-flex">
                    <div class="col-50">
                        <span class="foot-info-booleano">Boolando s.r.l.</span>
                        <div>
                            <span class="social-info">Informazioni legali</span>
                        </div>
                    </div>
                    <div class="col-50">
                        <span class="found-us "> Trovaci anche su</span>
                        <br>
                        <div class="social-logo">
                            <img src="/img/user.png" alt="social">
                            <img src="/img/user.png" alt="social">
                            <img src="/img/user.png" alt="social">
                            <img src="/img/user.png" alt="social">
                            <img src="/img/user.png" alt="social">
                        </div>
                    </div>
                </div>
            </div>
        </div>

    </footer>
</template>

<style lang="scss" scoped >
.container {
    width: 900px;

    .col-100 {
        width: 100%;
    }

    .row-flex {
        display: flex;
        flex-wrap: wrap;
    }

    .col-50 {
        width: 50%;
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

    .found-us {
        padding: 0 10px;
        font-size: 10px;
        color: white;
        font-weight: bold;
        margin-left: 77%;
    }

    .social-logo {
        margin-top: 10px;
        display: flex;
        margin-left: 81%;
        width: 15px;
        filter: invert(100%);
    }

    .margin-left {
        margin-left: 83%;
    }
}
</style>