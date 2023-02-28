<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-primary">
        <div class="container justify-content-evenly">
          <router-link to="/" class="nav-link active" aria-current="page" ><span class="material-icons-round">home</span></router-link>
          <router-link to="/about" class="nav-link" ><span class="material-icons-round">info</span></router-link>
          <router-link to="/posts" class="nav-link" ><span class="material-icons-round">featured_play_list</span></router-link>
        </div>
    </nav>
</template>

<script>
  export default {
    name : "NavComp"
  }
</script>

<style scoped>
  .material-icons-round {
    color: white;
    font-size: 1.4em;
    background-color:  rgba(128, 128, 128, 0.351);
    padding: 0.4em;
    border-radius: 50%;
    margin: 0.1em;
  }

  .navbar {
    padding-top: 0;
    padding-bottom: 0;
  }
</style>