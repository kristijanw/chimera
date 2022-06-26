<template>
	
    <footer>
        
        <div class="container">

            <div class="logo text-center">
                <img src="/logo_footer.png" alt="logo">
            </div>

            <hr>

            <div class="row">
                <div class="col-md-6">
                    <h2>CHIMERA </h2>

                    <div class="link">
                        <nuxt-link to="/about-us">About Us</nuxt-link>
                        <nuxt-link to="/projects">Projects</nuxt-link>
                        <nuxt-link to="/contact">Contact</nuxt-link>
                    </div>
                </div>
                <div class="col-md-6">
                    <div class="footer_contact">
                        <h2>KONTAKT</h2>

                        <div class="link">
                            <a href="mailto:info@chimera.hr">info@chimera.hr</a>
                            <a href="tel:091 233 2053">091 233 2053</a>
                        </div>
                    </div>
                </div>
            </div>

            <div class="row politica_link_social_icon">
                <div class="col-md-6">
                    <div class="politica_link">
                        <a href="">Impressum</a>
                        <a href="">Uvjeti poslovanja</a>
                        <a href="">Politika privatnosti</a>
                    </div>
                </div>
                <div class="col-md-6">
                    <div class="social_icon">
                        <img src="/face_logo.png" alt="face_logo">
                        <img src="/twitter_logo.png" alt="twitter_logo">
                        <img src="/instagram_logo.png" alt="instagram_logo">
                    </div>
                </div>
            </div>

        </div>

        <img class="footer_circle" src="/footer_circle.png" alt="footer_circle">
    </footer>

</template>

<script>

export default {
  name: 'Footer',
}
</script>

<style>
footer {
    background: #000;
}
footer hr {
    background: #FFFFFF;
    mix-blend-mode: normal;
    opacity: 0.1;
    margin-bottom: 50px;
}
.footer .logo {
    padding: 50px;
}

footer .footer_contact {
    max-width: fit-content;
    margin-left: auto;
    text-align: left;
}

footer h2 {
    font-family: 'Montserrat', sans-serif;
    font-size: 17px;
    font-weight: 400;
    color: #C8DBD9;
    margin-bottom: 22px;
}

footer div.link {
    display: flex;
    flex-direction: column;
}

footer div.link a {
    font-family: 'Montserrat', sans-serif;
    font-size: 15px;
    font-weight: 400;
    color: #fff;
    margin-bottom: 22px;
}

footer .politica_link {
    display: flex;
    align-items: center;
}

footer .politica_link a {
    margin-right: 40px;
    font-weight: 700;
    font-size: 12px;
    color: #C8DBD9;
}

footer .social_icon {
    display: flex;
    align-items: center;
    justify-content: flex-end;
}
footer .social_icon img {
    margin-left: 40px;
}

footer .politica_link_social_icon {
    padding-top: 100px;
}

footer .footer_circle {
    display: flex;
    margin: auto;
    padding-top: 20px;
}
</style>