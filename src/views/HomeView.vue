<template>
  <div class="w-full px-4 py-4 md:px-6 lg:px-20">
    <NavbarComponent />
    <div class="w-full my-4 rounded-xl">
      <img class="object-cover rounded-lg" src="../assets/img/image4.png" alt="banner">
    </div>
    <div class="w-full">
      <h2 class="font-medium text-lg">Trend Categories</h2>
      <div class="w-full grid grid-cols-4 gap-4 mt-3 lg:grid-cols-6 xl:grid-cols-8 lg:gap-8 xl:gap-9">
        <CategoryComponent />
      </div>
      <div class="w-full cursor-pointer flex lg:justify-end mt-3">
        <a href="#">
            <div class="px-6 pt-1 pb-2 text-base bg-primary text-white rounded-md shadow-md hover:bg-opacity-75">
                All catagories 
            </div>
        </a>
      </div>
      <div class="w-full mt-5">
        <h2 class="font-medium text-lg">New Products</h2>
        <div class="w-full grid grid-cols-2 gap-2 mt-3 lg:grid-cols-4">
          <ProductComponent />
        </div>
      </div>
      <div class="w-full cursor-pointer flex lg:justify-end mt-3">
        <a href="#">
            <div class="px-6 pt-1 pb-2 text-base bg-primary text-white rounded-md shadow-md hover:bg-opacity-75">
                All products 
            </div>
        </a>
      </div>
    </div>
  </div>
  <FooterComponent />
</template>

<script>
// @ is an alias to /src
import NavbarComponent from '@/components/NavbarComponent.vue'
import CategoryComponent from '@/components/CategoryComponent.vue'
import ProductComponent from '@/components/ProductComponent.vue'
import FooterComponent from '@/components/FooterComponent.vue'

export default {
  name: 'HomeView',
  components: {
    NavbarComponent,
    CategoryComponent,
    ProductComponent,
    FooterComponent,
  }
}
</script>
