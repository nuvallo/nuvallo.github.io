<template>
  <div className="content-container">
      <div className="container">
          <h1>Experience</h1>
          <ul v-bind:key="experience.id" v-for="experience in experiences">
              <li><h2>{{experience.title}}</h2></li>
              <li><h3>{{experience.job}}</h3></li>
              <li><h4>{{experience.date}}</h4></li>
              <li><h5>{{experience.description}}</h5></li>
          </ul>
      </div>
      <div className="container">
          <h1>
              Education
          </h1>
          <ul v-bind:key="education.id" v-for="education in educations">
              <li><h2>{{education.title}}</h2></li>
              <li><h3>{{education.degree}}</h3></li>
              <li><h4>{{education.year}}</h4></li>
          </ul>
      </div>
       <div className="container">
          <h1>
             Projects 
          </h1>
          <ul v-bind:key="project.id" v-for="project in projects">
              <li><h2>{{project.title}}</h2></li>
              <li><h3>{{project.framework}}</h3></li>
              <li><h5>{{project.description}}</h5></li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
    props: ['experiences', 'educations', 'projects'],
    name: 'Content',
}
</script>

<style>
.content-container {
    background-color: #EEFBFB;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.container {
    padding: 5%;
}

.container h1 {
    font-size: 30px;
    padding-bottom: 2%;
}

.container ul {
    list-style: none;
    margin: 3%;
    
}

.container li {
    padding: 1%;
}

.container ul li h2 {
    font-size: 20px;
    font-weight: 500;

}

.container ul li h3 {
    color: #333;
    font-size: 15px;
    font-weight: 200;
}

.container ul li h4 {
    color: #333;
    font-size: 10px;
    font-weight: 200;
}

.container ul li h5 {
    font-size: 15px;
    color: #333;
    font-weight: 200;
}
</style>