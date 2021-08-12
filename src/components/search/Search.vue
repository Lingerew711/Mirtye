<template>
    <div class="wrap">
   <div class="search">
      <input type="text" class="searchTerm" placeholder="search product...">
      <button type="submit" class="searchButton">
        <i class="fa fa-search"></i>
     </button>
     <Detail/>
     <button href="#" class="btn btn-outline-primary float-right ml-5" @click="openModal" data-toggle="modal" data-target="#myModal">Add Product</button>
   </div>
</div>
</template>
<script>
import Detail from '../detail/Detail'
export default{
    name: 'Search',
    components: {
        Detail
    },
    methods: {
        openModal(){
            let element = this.$refs.modal.$el
            element.modal('show')
        }
    }
}
</script>