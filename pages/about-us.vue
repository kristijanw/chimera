<template>
    
    <div class="about">
        <div class="header_about">
            <div class="container">
                <img src="/about_circle.png" alt="about_circle">

                <div class="breadcrumbs">
                    Home / <strong>About us</strong>
                </div>

                <h1>
                    Shaping the space
                    of your new chapter
                </h1>
            </div>
        </div>

        <div class="container">
            <div class="row">
                <div class="col-md-12">

                    <div class="about_section2">
                        <p>
                            Chimera allows you to transform your home into the space of your dreams with no hassle. 
                            We provide everything you need to create the home of your dreams, including:
                        </p>
                    </div>

                </div>
            </div>

            <div class="row">
                <div class="col-md-4">
                    <div class="including">
                        <img src="/about1.png" alt="about1">
                        <p>
                            Interior design of private houses and apartments, rental apartments, interior 
                            or office spaces, design of exteriors and gardens
                        </p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="including">
                        <img src="/about2.png" alt="about2">
                        <p>
                            Interior design of private houses and apartments, rental apartments, interior 
                            or office spaces, design of exteriors and gardens
                        </p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="including">
                        <img src="/about3.png" alt="about3">
                        <p>
                            Interior design of private houses and apartments, rental apartments, interior 
                            or office spaces, design of exteriors and gardens
                        </p>
                    </div>
                </div>
            </div>
        </div>

        <div class="about_section2">
            <div class="row m-0">
                <div class="col-md-8">
                    <img class="img1" src="/about_images/1.png" alt="">
                </div>
                <div class="col-md-4 p-5 d-flex justify-content-center">
                    <img class="img2" src="/about_images/2.png" alt="">
                </div>
            </div>

            <div class="row m-0 pt-5">
                <div class="col-md-3">

                </div>
                <div class="col-md-9">
                    <img class="img3" src="/about_images/3.png" alt="">
                </div>
            </div>

            <div class="row m-0 pt-5">
                <div class="col-md-6">
                    <img class="img4" src="/about_images/4.png" alt="">
                </div>
                <div class="col-md-6">
                    
                </div>
            </div>

            <div class="row m-0 pt-5" id="img5">
                <div class="col-md-4">

                </div>
                <div class="col-md-8">
                    <img class="img5" src="/about_images/5.png" alt="">
                </div>
            </div>
        </div>

    </div>

</template>

<style>
.about {
    background: #F4F4F4;
}
.about .container {
    position: relative;
}
.header_about {
    position: relative;
    background: url("/about_bg_header.png");
    background-repeat: no-repeat;
    background-size: cover;
}
.about .header_about > div > img {
    position: absolute;
    left: -150px;
    top: 30px;
}
.about .breadcrumbs {
    font-family: 'Montserrat', sans-serif;
    font-size: 18px;
    font-weight: 400;
    padding: 100px 0px;
    color: #fff;
}
.about h1 {
    font-family: 'Libre Baskerville', serif;
    font-size: 60px;
    font-weight: 400;
    max-width: 50%;
    color: #fff;
    padding-bottom: 200px;
}

.about_section2 {
    padding: 100px 0px;
    font-family: 'Montserrat', sans-serif;
}

.about_section2 > p {
    font-size: 30px;
    font-weight: 500;
    color: #000;
    max-width: 50%;
    margin: auto;
    text-align: center;
}

.about .including {
    padding: 50px 30px;
    position: relative;
}
.about .including img {
    position: absolute;
    left: 0px;
    top: 0px;
}
.about .including p {
    font-family: 'Montserrat', sans-serif;
    font-size: 20px;
    color: #000;
    padding: 20px;
}

.about .about_section2 img {
    width: 100%;
}

.about .about_section2 .img2 {
    padding: 50px;
}

.about .about_section2 #img5 {
    margin-top: -25% !important;
}
</style>