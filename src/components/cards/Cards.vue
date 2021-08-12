<template>
  <div class="pro">
    <Detail v-if="show"/>
    <div class="card m-3" style="width: 20rem">
      <img
        class="card-img-top"
        src="@/assets/images/sho.jpg"
        alt="Card image cap"
      />
      <div class="card-body">
        <h5 class="card-title">{{ text }}</h5>
        <p class="card-text">
          Some quick example text to build on the card title and make up the
          bulk of the card's content.
        </p>
        <button
          @click.prevent="showModal"
          class="btn btn-outline-primary float-right ml-1"
          title="details"
        >
          <i class="fa fa-th-list"></i>
        </button>
        <button
          href="#"
          class="btn btn-outline-primary float-right"
          title="add to cart"
        >
          <i class="fa fa-shopping-cart"></i>
        </button>
      </div>
    </div>
  </div>
</template>

<script>

import Detail from '../detail/Detail.vue'
export default {
  name: "Cards",
  components: {
    Detail
  },
  props: {
    text: String,
  },
 data(){
  return{
     isVisiblity: false
  }
 },
 methods: {
   showModal(){
     this.isVisiblity = !this.isVisiblity;
   }
 }
};
</script>

