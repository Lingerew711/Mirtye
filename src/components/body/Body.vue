<template>
  <div class="product-body">
  <div class="row">
      <Search />
      <div class="co1-4">
          <Cards text = "Product Name"/>
      </div>
      <div class="co1-4">
          <Cards text = "Product Name"/>
      </div>
      <div class="co1-4">
          <Cards text = "Product Name"/>
      </div>
  </div>
  
  </div>
</template>

<script>
import Cards from "../cards/Cards"
import Search from "../search/Search"

export default {
  name: "Body",
  components: {
      Cards,
      Search,
  }
};
</script>