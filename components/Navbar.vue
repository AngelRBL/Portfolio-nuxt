<template>
  <div>
    <b-navbar toggleable="lg" variant="danger">
      <b-navbar-brand class="name" :to="to.home">
        <h4>{{ name }}</h4>
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav>
        <!-- About -->
        <b-navbar-nav>
          <b-nav-item class="routers" :to="to.about">
            <h4>{{ about }}</h4>
          </b-nav-item>
        </b-navbar-nav>
        <!-- Services -->
        <b-navbar-nav>
          <b-nav-item class="routers" :to="to.services">
            <h4>{{ services }}</h4>
          </b-nav-item>
        </b-navbar-nav>
        <!-- PROYECTS -->
        <b-navbar-nav>
          <b-nav-item class="routers" :to="to.projects">
            <h4>{{ projects }}</h4>
          </b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  data: () => ({
    name: "ROBLES",
    about: "SOBRE MI",
    services: "SERVICIOS Y HABILIDADES",
    projects: "PROYECTOS Y CONTACTO",
    to: {
      home: "/",
      about: "/",
      services: "/services",
      projects: "/projects"
    }
  })
};
</script>

<style scoped>
@font-face {
  font-family: "Quantum";
  src: url("../assets/font/Quantum.otf");
}

.name {
  text-decoration: none !important;
  color: black;
  font-family: "Quantum", sans-serif;
  margin: 0px 5px;
}

.name h4 {
  font-size: 33px;
  letter-spacing: 3px;
}

.routers h4 {
  /* text-decoration: none; */
  color: #fff;
  padding: 3px 2px;
  font-size: 16px;
  font-weight: 600;
}

#nav-collapse {
  justify-content: flex-end;
}
</style>
