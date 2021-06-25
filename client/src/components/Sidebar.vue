<template>
  <div className="sidebar-container">
      <div className="sidebar-box">
          <h1>About me</h1>
          <p>My name is Tyler and I love development, engineering, and working with people to solve everyday problems. I have worked in numerous customer-service-oriented jobs and a few technical skilled jobs, such as; Website development, user interface design, backend development, etc. I mostly enjoy programming and working within command-line interfaces. I've worked with businesses that use slack, discord, zoom, and other software. I am very familiar with Linux (Arch, Redhat, and Debian), Mac OS-X, and Windows.</p>
      </div>
      <div className="sidebar-box">
          <h1>Skills</h1>
          <ul className="skills">
              <li>Javascript</li>
              <li>Python</li>
              <li>React</li>
              <li>Vue</li>
              <li>NodeJS</li>
              <li>Express</li>
              <li>SQLite</li>
              <li>GNU/Linux</li>
              <li>Adobe Software</li>
              <li>HTML5 / CSS3</li>
          </ul>
      </div>
      <div className="sidebar-box">
          <h1>Contact</h1>
          <ul>
              <li>Vexiiry@gmail.com</li>
              <li>904-718-3071</li>
          </ul>
          <a className="icon" href="https://github.com/nuvallo" target="_blank"><i class="fab fa-github fa-2x icon"></i></a>
          <a className="icon" href="https://www.linkedin.com/feed/?trk=homepage-basic_signin-form_submit" target="_blank"><i class="fab fa-linkedin fa-2x icon"></i></a>
      </div>
  </div>
</template>

<script>
export default {
    name: "Sidebar"
}
</script>

<style>
@media (max-width: 761px) {
 .sidebar-container {
    width: 100% !important;
 } 
 .box {
    padding: 10% 5% !important;
 }
}
.sidebar-container {
    background-color: #12232E;
    color: #fff;
    width: 80%;
    display: flex;
    flex-direction: column;
    
}

.sidebar-box {
    padding: 5%;
}

.sidebar-box h1 {
    font-size: 30px;
    margin-bottom: 1%;
}

.sidebar-box ul {
    list-style: none;
}

.sidebar-box ul li {
    padding: 1%;
}

.sidebar-box p {
    line-height: 1.5;
}

.skills {
    display: flex;
    flex-wrap: wrap;
}

.skills li {
    margin: 2%;
    border: 2px solid #fff;
}

.icon {
    padding: 1%;
    color: #fff;
}
</style>