<template>
    <div v-for="product in products" :key="product.name" class="w-full flex flex-col gap-3 rounded-lg">
        <img class="object-cover rounded-lg w-full h-full" src="../assets/img/Vector.png" alt="banner">
        <div class="flex flex-col gap-1">
            <a href="#" class="text-base font-medium">{{ product.name }}</a>
            <span class="text-sm font-medium text-active"> Rp {{ product.price.toLocaleString() }}</span>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ProductComponent',
        data() {
            return {
                products: [
                    {
                        name: 'Apple Watch 4',
                        price: 1200000
                    },
                    {
                        name: 'Apple Watch 3',
                        price: 1000000
                    },
                ]  
            }
        }
    }
</script>

<style scoped>

</style>