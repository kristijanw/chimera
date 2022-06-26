<template>
    
    <div class="contact_page">
        <div class="container">
            <div class="row">
                <div class="col-md-12">
                    <div class="contact">
                        <img src="/contact_circle.png" alt="contact_circle">

                        <h1>Contact us</h1>
                        <p>
                            Maecenas accumsan lacus vel facilisis volutpat est velit. Lectus magna fringilla 
                            urna porttitor rhoncus dolor purus non enim. Molestie a iaculis at erat pellentesque 
                            adipiscing commodo purus. Sit amet volutpat mauris consequat nunc cradi. 
                        </p>

                        <p class="tel">Tel: <a href="tel:+385 99 233 2053">+385 99 233 2053</a></p>
                        <p class="mail"><a href="mailto:info@chimera.hr">info@chimera.hr</a></p>
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>

<style>
.contact_page {
    background: #F4F4F4;
}
.contact_page .contact {
    position: relative;
    padding-top: 150px;
    padding-bottom: 300px;
    padding-left: 50px;
    max-width: 60%;
    z-index: 1;
}
.contact_page .contact img {
    position: absolute;
    top: 10%;
    left: -13%;
    z-index: -1;
}
.contact_page .contact h1 {
    font-family: 'Libre Baskerville', serif;
    font-weight: 400;
    font-size: 70px;
    color: #000;
}
.contact_page .contact p {
    font-family: 'Montserrat', sans-serif;
    font-weight: 300;
    font-size: 18px;
    color: #000;
    margin-top: 30px;
}
.contact_page .contact p.tel {
    font-weight: 700;
}
.contact_page .contact p.tel a,
.contact_page .contact p.mail a {
    font-weight: 700;
    text-decoration: none;
    color: #000;
}
</style>