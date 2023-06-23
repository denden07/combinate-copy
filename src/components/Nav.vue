<template>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <router-link  class="navbar-brand logo" to="/">
        <img src="../assets/images/logo-horizontal.svg" alt="" width="200" >
    </router-link>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav ms-auto mb-2 mb-lg-0 navbar-items">
        <li class="nav-item dropdown">
          <a class="nav-link" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Services
          </a>
          <div class="dropdown-menu">
            <li><a class="dropdown-item" href="#">Custom Software Development</a></li>
            <li><a class="dropdown-item" href="#">Website Development</a></li>
            <li><a class="dropdown-item" href="#">AWS Technology Partner</a></li>
            <li><a class="dropdown-item" href="#">Automation Consultancy</a></li>
            <li><a class="dropdown-item" href="#">Software Consultancy</a></li>
            <li><a class="dropdown-item" href="#">UI/UX</a></li>  
            <li><a class="dropdown-item" href="#">Sass/Marketplace Development</a></li>  
            <li><a class="dropdown-item" href="#">Technical Documentation</a></li>  
            <li><a class="dropdown-item" href="#">Workflow Automation</a></li>  
        </div>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Our Team</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
           Case Studies
          </a>
          <div class="dropdown-menu">
            <li><a class="dropdown-item" href="#">National Police Check</a></li>
            <li><a class="dropdown-item" href="#">Steadfast Group</a></li>
          </div>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Showcase</a>
        </li>
        <li>
            <button @click="$router.push('/enquire-now')" class="btn btn-primary">ENQUIRE NOW</button>
        </li>
      </ul>
    </div>
  </div>
</nav>
</template>

<style scoped>
.dropdown:hover .dropdown-menu {
    display: block;
}

nav {
    width: 100% !important;
    height: 88px !important;
    background:transparent !important;
    z-index: 2;
}

.navbar-items {
    margin-right:17%;
}

.logo{
    margin-left: 17%;
}
*{
    border-radius: 0 !important;
}
.btn {
    background: none !important;
    color: #0d6efd;
}

.btn:hover {
    background: #0d6efd !important;
}
</style>