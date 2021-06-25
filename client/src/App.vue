<template>
  <div>
    <Header />
    <div className="grid">
      <Sidebar />
      <Content v-bind:experiences="experience" v-bind:educations="education" v-bind:projects="projects"/>
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Sidebar from './components/Sidebar.vue';
import Content from './components/Content.vue';
import './App.css';

export default {
   data() {
    return {
      experience: [],
      education: [],
      projects: []
    }
  },
  created() {
    this.experience = [{
        id: 1,
        title: 'Developer / Laborer',
        job: 'Just Smash It',
        date: 'since December 2019',
        description: 'Hired to create the entire front-end website with ReactJS and Material-UI.'
      },{
        id: 2,
        title: "Sales associate",
        job: 'AutoZone',
        date: 'September 2018 - August 2019',
        description: 'Part time sales associate at AutoZone!'
      },{
        id: 3,
        title: 'Sales associate',
        job: 'Miller Automotive Group',
        date: 'May 2016 - August 2018',
        description: 'Hired on as a sales associate for selling cars and keeping up with the maintenance of each vehicle.'
      }],
    this.education = [{
        id: 1,
        title: 'Oakleaf High School',
        degree: 'diploma',
        year: '2019'
      }],
    this.projects = [{
        id: 1,
        title: 'Just Smash It',
        framework: 'ReactJS and Material-UI',
        description: 'Just Smash It Rage Rooms hired me to build a front-end website with React that was responsive for mobile, tablet, and desktop view.'
      },
      {
        id: 2,
        title: 'Resume',
        framework: 'VueJS',
        description: 'Created my entire resume front-end using vue.'
      }]
  },
  name: 'App',
  components: { Header, Sidebar, Content },
}
</script>

<style>
@media (max-width: 761px) {
  .grid { 
    display: flex !important;
    flex-direction: column-reverse !important; 
  }
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.grid {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  height: 100%;
}
</style>
