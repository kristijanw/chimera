<template>
	<header class="header">
        <div class="container nav">
            <div class="logo">
                <img src="/logo.png" alt="logo">
            </div>

            <div class="link">
                <nuxt-link to="/about-us">ABOUT US</nuxt-link>
                <nuxt-link to="/projects">PROJECTS</nuxt-link>
                <nuxt-link to="/contact">CONTACT</nuxt-link>
            </div>
        </div>
    </header>
</template>

<script>

export default {
  name: 'Header',
}
</script>