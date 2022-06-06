<template>
<div id="mySidenav" class="sidenav" ref="mySidenav">
         <div class="sidebar mr-2" v-if="toggle">
        <div class="header text-light">
          <a href=""><i class="fa fa-hourglass-end " aria-hidden="true"></i></a>
          <a href="">
            <p class="">Bhumlu</p>
          </a>
      <a href="#"><i class="fa fa-bars ml-3 bar" aria-hidden="true" @click="toggleSideNav()"></i>
</a>
        </div>
        <a href="#home"><i class="fa fa-fw fa-home"></i> Dashboards <button class="btn btn-danger p-0">HOT</button><i
            class="ml-1 fa fa-caret-left" aria-hidden="true"></i></a>
        <a href="#services"><i class="bi bi-stack"></i> Widget <button class="btn btn-primary p-0 ml-4">100+</button><i
            class="ml-2 fa fa-caret-down" aria-hidden="true"></i>
          <div class="ml-4">
            <a href="">Simple</a>
            <a href="">Data</a>
            <a href="">Social</a>
            <a href="">Chart</a>
          </div>
        </a>
        <hr class="bg-light">

        <h5><i class="fa fa-umbrella" aria-hidden="true"></i>Component</h5>
        <a href="#home"><i class="fa fa-file-text" aria-hidden="true"></i> Topography</a>
        <a href="#services"><i class="fa fa-bold" aria-hidden="true"></i> Basic UI <i class="ml-1 fa fa-caret-left"
            aria-hidden="true"></i> </a>
        <a href="#services"><i class="fa fa-user-md" aria-hidden="true"></i> Advance UI <i class="ml-1 fa fa-caret-left"
            aria-hidden="true"></i> </a>
        <hr class="bg-light">

        <h5> Forms & Tables</h5>
        <a href="#home"><i class="fa fa-book" aria-hidden="true"></i> Forms</a>
        <a href="#services"><i class="fa fa-table" aria-hidden="true"></i> Tables <i class="ml-1 fa fa-caret-left"
            aria-hidden="true"></i> </a>
        <hr class="bg-light">

        <h5>Forms & Tables</h5>
        <a href="#home"><i class="fa fa-location-arrow" aria-hidden="true"></i> Gmaps</a>
        <a href="#services"><i class="fa fa-pie-chart" aria-hidden="true"></i> Charts <i class="ml-1 fa fa-caret-left"
            aria-hidden="true"></i> </a>
      </div>
      <i v-else class="fa fa-bars ml-3 mt-2 bar" aria-hidden="true" @click="toggleSideNav()"></i>

      </div>
     
</template>

<script>
export default {
  data(){
return{
    toggle:true
}
  },
methods:{
  toggleSideNav() {
  this.toggle = !this.toggle
}
}
}
</script>

<style>
@media (max-width:480px) {
  .sidenav{
    display: none;
  }
}
.sidebar {
    height: 100vh;
    position: sticky;
    z-index: 1;
    top: 0;
    left: 0;
    background-color: #111;
    padding: 10px;
    /* overflow-x: hidden; */
    
  }
  
  .bar{
      font-size: 20px;
      background-color: white;
      border-radius: 5px;
      padding: 5px;
      /* margin-top: 5px; */
      border: #111 1px solid;
      color: silver;
  }
  
  .header{
    display: flex;
  }
  
  
  .sidebar a {
    padding: 4px 8px 4px 10px;
    text-decoration: none;
    font-size: 15px;
    color: #818181;
    display: block;
  }
  
  
  .sidebar a:hover {
    color: #f1f1f1;
    background-color: #818181;
  }
  
  .i{
    font-size: 2rem;
    color: purple;
  }
</style>
