<template lang="pug">
nav.navbar.navbar-default.light-shadow.container-fluid.hidden-xs(id="main-menu")
    .text-center
        ul.nav.navbar-nav(role="navigation")
            li.dropdown
                a.dropdown-toggle(aria-expanded="false" data-toggle="dropdown" v-for="(link, i) in importantLinks" :key="i" href="link.href") {{link.text}}
</template>
<script>
export default {
    name: 'Navbar',
    data() {
        return {
        importantLinks: [
            {
            text: 'IGAPÄEVAPANGANDUS',
            href: 'https://vuetifyjs.com',
            },
            {
            text: 'RAHA KASVATAMINE',
            href: 'https://community.vuetifyjs.com',
            },
            {
            text: 'LAEN JA LIISING',
            href: 'https://madewithvuejs.com/vuetify',
            },
            {
            text: 'PENSION',
            href: 'https://twitter.com/vuetifyjs',
            },
            {
            text: 'VAJAD ABI?',
            href: 'https://medium.com/vuetify',
            }
      ]
        }
    },
}
</script>