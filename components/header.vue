<template>
	<header class="header">
        <div class="container nav">
            <div class="logo">
                <NuxtLink to="/">
                    <img src="/logo.png" alt="logo" />
                </NuxtLink>
            </div>

            <div class="link">
                <NuxtLink to="/about-us">ABOUT US</NuxtLink>
                <NuxtLink to="/projects">PROJECTS</NuxtLink>
                <NuxtLink to="/contact">CONTACT</NuxtLink>
            </div>
        </div>
    </header>
</template>

<script>

export default {
  name: 'Header',
}
</script>

<style>
header.header {
    background: #F4F4F4;
    padding: 20px 0px;
}

header.header .nav .logo > img {
    max-width: 70%;
    margin-bottom: 10px;
}

header.header .nav {
    align-items: center;
    justify-content: space-between;
}

header.header .link a {
    font-family: 'Montserrat', sans-serif;
    font-weight: 400;
    color: #000;
    font-size: 18px;
    margin-left: 40px;
    text-decoration: none;
    position: relative;
}

header.header .link a:last-child {
    color: #11897D;
}

header.header .link a:hover {
    color: #11897D;
}

header.header .link .nuxt-link-active {
    font-weight: 700;
    z-index: 1;
}

header.header .link .nuxt-link-active:before {
    content: url("/active_link_meni.png");
    position: absolute;
    left: 10px;
    top: -25px;
    z-index: -1;
}
</style>