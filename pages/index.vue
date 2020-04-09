<template lang="pug">
.container
	div
		Header
		br
		br
		h1.title lhv2.0
		h2.subtitle Kasutajaliideste disain ja arendus
		.links
			a.button--green(href="https://nuxtjs.org/" target="_blank") Documentation
			a.button--grey(href="https://github.com/nuxt/nuxt.js" target="_blank") GitHub
		Footer
</template>

<script>
import Logo from "~/components/Logo.vue"
import Footer from "~/components/Footer.vue"
import Header from "~/components/Header.vue"

export default {
  components: {
	Logo,
	Footer,
	Header
  }
}
</script>