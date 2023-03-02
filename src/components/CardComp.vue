<template>
    <div class="card">
        <div class="card-body">
            <h5 v-if="title" class="card-title"> <!-- v-if si title esta declarado se muestra en el componente -->
                {{ title }}
            </h5>
            <p v-if="paragraph" class="card-text"> <!-- v-if si paragraph esta declarado se muestra en el componente -->
                {{ paragraph }}
            </p>
            <slot>
                <!-- Permite insertar contenido html en el componente -->
            </slot>
            <div class="d-grid gap-2">
                <button 
                    v-for="btn in btns"
                    :key="btn.txt"
                    class="btn" 
                    :class="btn.class">
                    {{ btn.txt }}
                </button>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'CardComp',
        props: ['title', 'paragraph', 'btns'],
    }
</script>

<style scoped>
    .card{
        border: none;
        box-shadow:  0 2px 4px rgb(0 0 0 / 10%), 0 8px 16px rgb(0 0 0 / 10%);
    }
</style>