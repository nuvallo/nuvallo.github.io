<template>
  <div className="content-container">
      <div className="container">
          <h1>Experience</h1>
          <ul>
              <li>title: </li>
              <li>Job:</li>
              <li>Date:</li>
              <li>Description:</li>
          </ul>
      </div>
      <div className="container">
          <h1>
              Education
          </h1>
          <ul>
              <li>title:</li>
              <li>degree:</li>
              <li>Year:</li>
          </ul>
      </div>
       <div className="container">
          <h1>
             Projects 
          </h1>
          <ul>
              <li>title:</li>
              <li>framework:</li>
              <li>Description:</li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
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
    font-size: 25px;
}

.container ul {
    list-style: none;
}
</style>