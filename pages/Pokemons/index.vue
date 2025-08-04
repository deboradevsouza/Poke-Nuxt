<template>
    <section class="flex bg-[#86A69D] items-center justify-center">
    <div class="flex flex-col">
        <div class="flex bg-[#F2E8DF] w-full p-4 m-4 rounded-xl ">
            <h2 class="flex text-center self-center">Pokémons da primeira geração:</h2>
        </div>


        <div v-for="pokemon in data.results" class="flex w-full p-4 m-4 rounded-xl bg-[#F2B263] justify-between content-between">
            <p>{{ pokemon.name }}</p>


            <NuxtLink to="/" class="flex justify-self-end self-end btn">Mais detalhes</NuxtLink>
            
        </div>
        
        
    </div>

    </section>
</template>

<script setup>

    const { data } = await useFetch('https://pokeapi.co/api/v2/pokemon?limit=150&offset=0');


</script>

<style scoped>

</style>