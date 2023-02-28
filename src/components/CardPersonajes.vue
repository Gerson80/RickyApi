<script setup>
    import Personajes from '@/components/Personajes.vue'
    defineProps({
    Datos: {
        type: String,
        required: true
    }
    })



    
</script>

<template>

        <div class="max-w-sm w-full lg:max-w-full lg:flex p-10 ">

            <button @click.prevent="ventana=true" class=" hover:bg-green-500  bg-lime-400 rounded-3xl overflow-hidden shadow-xl rounded-b  lg:rounded-xl p-4 flex flex-col justify-between leading-normal">
                <div class="">
                    <img class="w-40 h-48 rounded-xl mr-4" v-bind:src=  Datos.image  alt="Avatar of Jonathan Reinink">
                    <div class="h-28">
                        <h1 class="font-bold text-4xl mb-2 text-center">{{ Datos.name }}</h1>
                    </div>
                    
                </div>
            
            </button>

            <div v-bind="ventana" v-if="ventana">
                <form action="">
                    <input type="date" name="" id="">
                    <input @click.prevent="ventana=false" type='button' value='Gurdar'>
                
                </form>
            
            
            </div>
            
        </div>


        


</template>

