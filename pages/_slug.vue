<template>

  <div class="single_page">

    <div class="single_project_header">
        <div class="container">
            <div class="breadcrumbs">
                Home / Projects / <strong>{{ project[0].title }}</strong>
            </div>
        </div>

        <div class="container">
          <div class="row">
            <div class="col-md-8">
              <h1 class="title">{{ project[0].title }}</h1>

              <p class="content">
                {{ project[0].content }}
              </p>
            </div>
            <div class="col-md-4">
              <ul class="project_info">
                <li><strong>ARCHITECT:</strong> {{ project[0].architect }}</li>
                <li><strong>CLIENT:</strong> {{ project[0].client }}</li>
                <li><strong>LOCATION:</strong> {{ project[0].location }}</li>
                <li><strong>DATE:</strong> {{ project[0].date }}</li>
                <li><strong>CATEGORY:</strong> {{ project[0].category }}</li>
              </ul>
            </div>
          </div>
        </div>
    </div>

    <div class="container project_images">
      <div class="row">
        <div class="col-md-12">
          <div class="single_img">
            <img :src="project[0].single_img_url" alt="">
            <img :src="project[0].single_img_url" alt="">
            <img :src="project[0].single_img_url" alt="">
          </div>
        </div>
      </div>

      <div class="row">
        <div class="col-md-12">
          <div class="arrow_and_back">
            <img src="/arrow_left.png" alt="arrow_left">
            
            <NuxtLink to="/projects">
              <img src="/back_to_projects.png" alt="back_to_projects">
            </NuxtLink>
            
            <img src="/arrow_right.png" alt="arrow_right">
          </div>
        </div>
      </div>
    </div>

  </div>

</template>

<script>
const getProject = () => import('~/assets/projects.json').then(m => m.default || m)

export default {
  async asyncData ({ params, req }) {
    const projects = await getProject()
    const project = []

    projects.forEach(element => {
      if( element.slug === params.slug ){
        project.push(element)
      }
    });

    return { project }
  }
}
</script>

<style>
.single_page .single_project_header {
  background: #F4F4F4;
  padding-bottom: 170px;
}
.single_page .single_project_header .breadcrumbs {
  font-family: 'Montserrat', sans-serif;
  font-size: 18px;
  font-weight: 400;
  padding-top: 100px;
  padding-bottom: 20px;
  color: #000;
}
.single_page .single_project_header .breadcrumbs strong {
  text-transform: capitalize;
}
.single_page .single_project_header h1.title {
  font-family: 'Libre Baskerville', serif;
  font-weight: 400;
  color: #000;
  font-size: 70px;
  text-transform: uppercase;
}
.single_page .single_project_header p.content {
  font-family: 'Montserrat', sans-serif;
  font-weight: 300;
  color: #000;
  font-size: 18px;
  line-height: 28px;
  padding-top: 20px;
}
.single_page .single_project_header .project_info {
  font-size: 18px;
  line-height: 39px;
}
.single_page .single_project_header .project_info li {
  font-family: 'Montserrat', sans-serif;
  list-style: none;
}
.single_page .project_images {
  margin-top: -100px;
}
.single_page .single_img {
  padding-bottom: 100px;
}
.single_page .single_img img {
  width: 100%;
  margin-bottom: 20px;
}
.single_page .arrow_and_back {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding-bottom: 100px;
}
</style>