<template>
    
    <div class="project">

        <div class="project_header">
            <div class="container">
                <div class="breadcrumbs">
                    Home / <strong>Projects</strong>
                </div>
            </div>
        </div>

        <div class="container project_container">
            <div class="row">
                <div class="col-md-12">
                    <div class="projects">

                        <div class="project_item" v-for="(mountain, index) in mountains" :key="index">
                            <NuxtLink :to="mountain.slug">
                                <img :src="`${mountain.img_url}`" alt="project">
                                <div class="title">{{ mountain.title }}</div>
                                <div class="subtitle">{{ mountain.subtitle }}</div>
                            </NuxtLink>
                        </div>

                    </div>
                </div>
            </div>
        </div>

    </div>

</template>

<script>
import projects from '~/assets/projects.json';

export default {
    data() {
      return {
        mountains: []
      }
    },
    async fetch() {
      this.mountains = projects;
    }
}
</script>

<style>
.project .project_container {
    margin-top: -370px;
}

.project .project_header {
    background: #F4F4F4;
}

.project .project_header .breadcrumbs {
    font-family: 'Montserrat', sans-serif;
    font-size: 18px;
    font-weight: 400;
    padding-top: 100px;
    padding-bottom: 400px;
    color: #000;
}

.project .projects {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    padding-bottom: 100px;
}
.project .projects .project_item a {
    text-decoration: none;
}
.project .projects .project_item {
    width: 49%;
}
.project .projects .project_item img {
    width: 100%;
}

.project .projects .project_item .title {
    font-family: 'Libre Baskerville', serif;
    font-weight: 400;
    text-transform: uppercase;
    color: #000;
    font-size: 25px;
    padding-top: 35px;
}
.project .projects .project_item .subtitle {
    font-family: 'Montserrat', sans-serif;
    font-weight: 300;
    color: #000;
    font-style: italic;
    font-size: 20px;
    padding-bottom: 35px;
}
</style>