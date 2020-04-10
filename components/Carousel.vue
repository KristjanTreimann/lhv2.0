<template>
<client-only>
	<carousel :autoplay="true">
		<img src="../assets/elements/app-store-et.svg" alt="">
	</carousel>
</client-only>
</template>
<script>
import carousel from 'v-owl-carousel'
const carouselPlugin = process.client ? require('~/plugins/owl') : () => {}

export default {
	name: 'Carousel',
	components: carousel,
	created() {
		carouselPlugin()
	}
}
</script>
<style lang="stylus">
</style>