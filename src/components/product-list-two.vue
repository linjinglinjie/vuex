<template>
	<ul>
		<li v-for="product in saleProducts">
			<span>{{product.name}}</span>
			<span>${{product.price}}</span>
		</li>
	</ul>
</template>
<script>
	export default{
		data(){
			return {
				
			}
		},
		computed:{
			products(){
				return this.$store.state.products;
			},
			saleProducts(){
				return this.$store.getters.saleProducts;
			}
		}
	}
</script>
<style scoped>
	
</style>