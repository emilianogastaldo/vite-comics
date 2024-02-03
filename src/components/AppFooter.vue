<script>
import FooterMenu from './footer-components/FooterMenu.vue';
import FooterIcon from './footer-components/FooterIcon.vue';

export default {
    name: 'AppFooter',
    components: {
        FooterMenu,
        FooterIcon,
    },
    props: {
        menus: Array,
        icons: Array
    },
}
</script>

<template>
    <footer>
        <section id="footer-top" class="wrapper">
            <div class="row">
                <div v-for="(menu, i) in menus" :key="i" class="col">
                    <FooterMenu :menu="menu" />
                </div>
            </div>
        </section>
        <section id="footer-bottom">
            <nav class="wrapper flex">
                <div id="footer-bottom-nav-left">
                    <a href="#" class="btn btn-signup">SIGN-UP NOW!</a>
                </div>
                <div id="footer-bottom-nav-right">
                    <ul>
                        <li><a href="#" class="follow-btn">FOLLOW US</a></li>
                        <li v-for="(icon, i) in icons" :key="i">
                            <FooterIcon :icon="icon" />
                        </li>

                    </ul>
                </div>
            </nav>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
footer {
    background-image: url('../assets/img/footer_images/footer-bg.jpg');
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    color: white
}

#footer-top {
    background-image: url('../assets/img/logos/dc-logo-bg.png');
    background-repeat: no-repeat;
    background-position: right;
    padding: 2rem 0;
    height: 400px;

    .row {
        display: flex;
        height: 100%;
        gap: 1rem;
        flex-wrap: wrap;
        flex-direction: column;
        align-content: start;
    }
}

#footer-bottom {
    background-color: #303030;
    padding: 2rem 0;


}

.btn-signup {
    padding: 13px;
    font-family: 'Open Sans', sans-serif;
    background-color: transparent;
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