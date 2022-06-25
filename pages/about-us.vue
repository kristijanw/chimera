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
    </div>

</template>

<style>
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
    width: 50%;
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
    padding-top: 50px;
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
</style>