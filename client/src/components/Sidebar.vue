<template>
  <div className="sidebar-container">
      <div className="sidebar-box">
          <h1>About me</h1>
          <p>I was born in Jacksonville, Florida and currently live in Orange Park, Florida. When i was young I grew a huge passion for technology. I would spend my time playing around with computers, ipods, and other devices learning how they operate. After working a couple jobs in autmotive I quickly learned it wasn't for me and that I needed to surround myself with technology. I started self teaching myself programming and other technologies such as Linux and other operating systems. I am now a year into my growth and I love every minute I spend in font of my computer. </p>
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
              <li>GNU/Linux</li>
              <li>Adobe Software</li>
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