<template>
  <div class="home">
    <div class="row">
      <div class="col-lg-6">
        <div class="img-cont">
          <img alt="Vue logo" src="../assets/img/SocialNet.svg">
          <h2 class="text-center text-lg-start">Conéctate con amigos y el resto del mundo usando SocialNet</h2>
        </div>
      </div>
      <div class="col-lg-6">
        <!-- Uso del componente creado -->
        <card-comp :btns="btnArray" class="mx-auto card-comp">
          <div class="mb-3 mt-2">
            <input type="email" 
              class="form-control"
              placeholder="Ingresa tu correo" />
          </div>
          <div class="mb-3 mt-2">
            <input type="password" 
              class="form-control"
              placeholder="Contraseña" />
          </div>
        </card-comp>
      </div>
    </div>
  </div>
</template>

<script>
  import CardComp from '@/components/CardComp.vue';

  export default {
    name: 'HomeView',
    components: {
      CardComp
    },

    data() {
      return {
        btnArray:[
          {
            txt: 'Iniciar Sesión',
            class: 'btn-primary',
          },
          {
            txt: 'Borrar',
            class: 'btn-danger',
          },
        ]
      }
    },
  }
</script>

<style scoped>
  .home {
    max-width: 895px;
    margin: auto;
  }

  .card-comp {
    max-width: 398px;
    margin-top: 2.6em;
  }

  .img-cont {
    display: flex;
    flex-direction: column;
  }

  .img {
    max-width: 315px;
    margin-top: 2.6em;
  }

  @media (min-width: 992px) {
    .home {
      margin: 4em auto;
    }
    .img {
      margin: 0;
      margin-top: 5.6em;
    }

    .h2 {
      margin: 0;
      margin-top: -0.8em;
      margin-left: 0.8em;
    }
  }
</style>
