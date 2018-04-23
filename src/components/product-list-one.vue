<template>
	<div>
		<ul>
			<li v-for="product in saleProducts">
				<span>{{product.name}}</span>
				<span>${{product.price}}</span>
			</li>
		</ul>
		<button @click="reducePrice(4)">降价</button>
	</div>
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
		},
		methods:{
			reducePrice:function(amont){
				this.$store.dispatch('reducePrice',amont);
			}
		}
	}

</script>
<style scoped>
	
</style>