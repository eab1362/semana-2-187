<template>
<div class="container-fluid p-0 m-0">
 <nav class=" d-flex navbar navbar-expand-sm bg-dark navbar-dark align-self-start">
  <!-- Brand/logo -->
  <a class=" mr-auto p-2 navbar-brand" href="#">GRUPO 187</a>
  
  <!-- Links -->
  <ul class=" p-2 navbar-nav align-self-end"  >
    <li class="nav-item">
      <a class="nav-link" href="#">Inicio</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" href="#noticias">Noticias</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" href="#team">Integrantes</a>
    </li>
  </ul>
</nav>
  <div id="demo" class="carousel slide" data-ride="carousel">

  <!-- Indicators -->
  <ul class="carousel-indicators">
    <li data-target="#demo" data-slide-to="0" class="active"></li>
    <li data-target="#demo" data-slide-to="1"></li>
    <li data-target="#demo" data-slide-to="2"></li>
  </ul>

  <!-- The slideshow -->
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="https://placeimg.com/1000/300/nature" alt="Los Angeles">
    </div>
    <div class="carousel-item">
      <img src="https://placeimg.com/1000/300/tech" alt="Chicago">
    </div>
    <div class="carousel-item">
      <img src="https://placeimg.com/1000/300/arch" alt="New York">
    </div>
  </div>

  <!-- Left and right controls -->
  <a class="carousel-control-prev" href="#demo" data-slide="prev">
    <span class="carousel-control-prev-icon"></span>
  </a>
  <a class="carousel-control-next" href="#demo" data-slide="next">
    <span class="carousel-control-next-icon"></span>
  </a>

</div>  
</div>

</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.carousel-inner img {
    width: 100%;
    height: 100%;
  }
</style>