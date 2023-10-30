<template>
    <div v-for="category in categories" :key="category.name" class="p-3 md:p-4 lg:p-6 bg-slate-100 w-24 md:w-32 lg:w-36 flex flex-col justify-center items-center gap-3 rounded-lg shadow-sm">
        <img class="w-12 h-12 md:w-16 md:h-16 lg:w-20 lg:h-20" src="../assets/img/Group14.png" alt="">
        <span class="text-sm font-medium md:text-base lg:text-lg">{{ category.name }}</span>
    </div>
</template>

<script>
    export default {
        name: 'CategoryComponent',
        data() {
            return {
                categories : [
                {
                    name : 'Gadget',
                },
                {
                    name : 'Electronic',
                }
            ]
            }
        }
    }
    
</script>

<style scoped>

</style>