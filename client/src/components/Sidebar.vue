<template>
  <div className="sidebar-container">
      <div className="box">
          <h1>About me</h1>
          <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
      </div>
      <div className="box">
          <h1>Skills</h1>
          <ul className="skills">
              <li>Javascript</li>
              <li>Python</li>
              <li>React</li>
              <li>Vue</li>
              <li>NodeJS</li>
              <li>Express</li>
              <li>GNU/Linux</li>
          </ul>
      </div>
      <div className="box">
          <h1>Contact</h1>
          <ul>
              <li>Vexiiry@gmail.com</li>
              <li>904-718-3071</li>
              <li>Nuvallo</li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
    name: "Sidebar"
}
</script>

<style>
.sidebar-container {
    background-color: #12232E;
    color: #fff;
    width: 80%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.box {
    padding: 17% 5%;
}

.box h1 {
    font-size: 25px;
    margin-bottom: 1%;
}

.box ul {
    list-style: none;
}

.box ul li {
    padding: 1%;
}

.box p {
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
</style>