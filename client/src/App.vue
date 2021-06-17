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
        description: 'I have created their entire website with React JS. I also worked as a laborer at Just Smash It.'
      },{
        id: 2,
        title: "Sales associate",
        job: 'AutoZone',
        date: 'September 2018 - August 2019',
        description: 'I worked as a sales associate at AutoZone!'
      },{
        id: 3,
        title: 'Sales associate',
        job: 'Miller Automotive Group',
        date: 'May 2016 - August 2018',
        description: 'I maintained the vehicles exterior and interior and other maintenance.'
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
        framework: 'ReactJS, Material-UI',
        description: 'Just Smash It Rage Rooms was my first client to build a front end website with React that was responsive for mobile, ipad, and desktop.'
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
    flex-direction: column !important; 
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
