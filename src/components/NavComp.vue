<template>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
        <div class="container-fluid">
          <router-link to="/" class="navbar-brand" >SOCIAL NET</router-link>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
              <li class="nav-item">
                <router-link to="/" class="nav-link active" aria-current="page" ><span class="material-icons-round">home</span></router-link>
              </li>
              <li class="nav-item">
                <router-link to="/about" class="nav-link" ><span class="material-icons-round">info</span></router-link>
              </li>
              <li class="nav-item">
                <router-link to="/posts" class="nav-link" ><span class="material-icons-round">featured_play_list</span></router-link>
              </li>
            </ul>
          </div>
        </div>
    </nav>
</template>

<script setup>

</script>

<style lang="scss" scoped>

</style>