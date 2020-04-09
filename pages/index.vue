<template lang="pug">
.container
	Header
	Navbar
	News
	br
	h1.title lhv2.0
	h2.subtitle Kasutajaliideste disain ja arendus
	.links
		a.button--green(href="https://nuxtjs.org/" target="_blank") Documentation
		a.button--grey(href="https://github.com/nuxt/nuxt.js" target="_blank") GitHub
	Footer
</template>

<script>
import Footer from '~/components/Footer.vue'
import Header from '~/components/Header.vue'
import Navbar from '~/components/Navbar.vue'
import News from '~/components/News.vue'

export default {
  components: {
	Footer,
	Header,
	Navbar,
	News
  }
}
</script>