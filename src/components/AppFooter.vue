<script>
export default {
    name: 'AppFooter'
}
</script>

<template>
    <footer>

        <section id="footer-top" class="wrapper">
            <div class="row">
                <div class="col">
                    <h4>dc comics</h4>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                    <h4>shop</h4>
                    <ul>
                        <li><a href="#">shop DC</a></li>
                        <li><a href="#">shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div class="col">
                    <h4>dc</h4>
                    <ul>
                        <li><a href="#">Terms of use</a></li>
                        <li><a href="#">privacy policy (new)</a></li>
                        <li><a href="#">Ad choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#"></a></li>
                        <li><a href="#"></a></li>
                        <li><a href="#"></a></li>
                        <li><a href="#"></a></li>
                        <li><a href="#"></a></li>
                        <li><a href="#">shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div class="col">
                    <h4>sites</h4>
                    <ul>
                        <li><a href="#">provafe</a></li>
                    </ul>
                </div>
            </div>
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

.row {
    display: flex;
    gap: 1rem;
}

.row .col h4 {
    text-transform: uppercase;
    font-size: larger;
}

.row .col ul {
    margin: 1rem 0;
}

.row .col ul li a {
    color: #818181;
    text-transform: capitalize;
}
</style>