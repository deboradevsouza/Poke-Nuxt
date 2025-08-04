<template>
    <div>
        <div v-for="pokemon in data.results" class="flex w-full p-4 m-4 rounded-xl bg-[#F2B263] justify-between content-between">
            <p>{{ pokemon.name }}</p>


            <NuxtLink to="/" class="flex justify-self-end self-end btn">Mais detalhes</NuxtLink>
            
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>

</style>