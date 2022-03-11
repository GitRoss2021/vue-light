<template>
<div class="side-navbar">
<div class="sidebar">
  <a class="active" href="/">Home</a>
  <a href="/About">About</a>
  <a href="/Profile">Resume</a>
  <a href="/Testimonials">Testimonials</a>
  <a href="/Contact">Contact</a>
  
  <!-- icons -->
<div class="icons">
  <a href="#"><i class="fa fa-github"></i></a>
     <a href="#"><i class="fa fa-android"></i></a>
     <a href="#"><i class="fa fa-linkedin-square"></i></a>
    <a href="#"><i class="fa fa-trello"></i></a>
    <a href="#"><i class="fa fa-windows"></i></a>   
    <a href="#"><i class="fa fa-youtube"></i></a>
</div>
     
</div>
</div>
</template>

<script>


export default {

}
</script>

<style scoped>
/* NAVIGATION START */
body {
  margin-top: 30px !important;
  font-family: "Lato", sans-serif;
}

.sidebar {
    z-index: 100;
  /* margin: 0 !important; */
  padding: 0;
  width: 250px;
  background-color: black;
  position: fixed;
  height: 100%;
  overflow: auto;
  margin-right: 30% !important;
}

.active{
  background-color: #d66b18;
}

.sidebar a {
  display: block;
  font-weight: bold;
  color: white;
  font-size: 20px;
  padding: 16px;
  text-decoration: none;
}
 

.sidebar a:hover:not(.active) {
  background-color: #d66b18;
  color: white;
}

div.content {
  margin-left: 200px;
  padding: 1px 16px;
  height: 1000px;
}

@media screen and (max-width: 700px) {
  .sidebar {
    width: 100%;
    height: auto;
    position: relative;
  }
  .sidebar a {float: left;}
  div.content {margin-left: 0;}
}

@media screen and (max-width: 400px) {
  .sidebar a {
    text-align: center;
    float: none;
  }
}
/* NAVIGATION ENDS*/

.icons{
  margin-top: 100px;
}

.icons:hover{
  transform: scale(1.1);
}

</style>