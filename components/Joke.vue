<template>
<nuxt-link :to="'jokes/' + id">
<div class="joke">
        <p>{{ joke }}</p>
    </div>
</nuxt-link>
    
</template>

<script>

export default {
   name: 'joke',
   props: ['joke', 'id']
}
</script>

<style scoped>
.joke{
    padding: 3rem;
    border: 1px dotted #ccc;
    margin: 1rem 0;
}
</style>