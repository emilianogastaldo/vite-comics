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
                        <li><a href="#">jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">talent workshop</a></li>
                        <li><a href="#">CPSC certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">shop help</a></li>
                        <li><a href="#">contact us</a></li>
                    </ul>
                </div>
                <div class="col">
                    <h4>sites</h4>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC universe</a></li>
                        <li><a href="#">DC power visa</a></li>
                    </ul>
                </div>
            </div>
        </section>
        <section id="footer-bottom">
            <nav class="wrapper flex">
                <div id="footer-bottom-nav-left">
                    <a href="#" class="button">SIGN-UP NOW!</a>
                </div>
                <div id="footer-bottom-nav-right">
                    <ul>
                        <li><a href="#" class="follow-btn">FOLLOW US</a></li>
                        <li><a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a></li>
                    </ul>
                </div>
            </nav>
        </section>

    </footer>
</template>

<style lang="scss" scoped>
footer {

    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    color: white
}

#footer-bottom {
    background-color: #303030;
    padding: 2rem 0;
}

#footer-top {
    background-image: url('../assets/img/dc-logo-bg.png');
    background-repeat: no-repeat;
    background-position: right;
    padding: 2rem 0;

    .row {
        display: flex;
        gap: 1rem;

        .col h4 {
            text-transform: uppercase;
            font-size: larger;
            font-weight: 500;
        }

        .col ul {
            margin: 1rem 0;

            li a {
                font-family: 'Open Sans', sans-serif;
                color: #818181;
                text-transform: capitalize;
                font-size: small;

                &:hover {
                    color: white;
                }
            }

        }
    }
}

#footer-bottom-nav-right ul {
    display: flex;
    align-items: center;
    gap: 1.5rem;


    .follow-btn {
        color: #0282F9;
        font-size: 1.4rem;
    }
}
</style>