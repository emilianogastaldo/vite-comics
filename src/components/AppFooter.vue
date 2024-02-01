<script>
export default {
    name: 'AppFooter'
}
</script>

<template>
    <footer>

        <section id="footer-top" class="wrapper">


        </section>
        <section id="footer-bottom">
            <div class="wrapper"></div>
        </section>

    </footer>
</template>

<style scoped>
footer {

    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    color: white
}

#footer-top {
    background-image: url('../assets/img/dc-logo-bg.png');
    background-repeat: no-repeat;
    background-position: right;
    padding: 2rem 0;
}

#footer-bottom {
    background-color: #303030;
    padding: 2rem 0;
}

.wrapper {
    width: 1200px;
    margin: 0 auto;
}
</style>