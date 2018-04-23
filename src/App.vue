<template>
  <div id="app">
  	<productListOne></productListOne>
    <productListTwo></productListTwo>
  </div>
</template>

<script>
	
	import productListOne from './components/product-list-one.vue'
	import productListTwo from './components/product-list-two.vue'
export default {
  name: 'app',
  data () {
    return {
     
    }
  },
  components:{
  	productListOne,
  	productListTwo
  }
}
</script>

<style>

</style>
