<template lang="pug">
#footer
	.container
		block extra
			.colums.links-secondary(v-if="menuLinks")
				.column(v-for="link in menuLinks")
					h3.section-subtitle(v-text="link.label")
					ul.is-unstyled
						li(v-for="sublink in link.submenu")
							a(v-bind:href="sublink.link") {{ sublink.label }}
</template>
<script>
export default {
  name: 'Links',
  data() {
    return {
      menuLinks: [
        {
          label: 'TULE KLIENDIKS',
          submenu: [
            {
              label: 'Eraklient',
              slug: 'eraklient',
              link: 'https://lhv.ee'
            },
            {
              label: 'Äriklient',
              slug: 'ariklient'
            },
            {
              label: 'Noortepank',
              slug: 'noortepank'
            },
            {
              label: 'Lapsekonto',
              slug: 'lapsekonto'
            },
            {
              label: 'Au-klient'
            },
            {
              label: 'Privaatpangandus'
            },
            {
              label: 'Ava konto'
            }
          ]
        },
        {
          label: 'LEIA KIIRELT',
          submenu: [
            {
              label: 'Hinnakiri ja tingimused',
              slug: 'eraklient',
              link: 'https://lhv.ee'
            },
            {
              label: 'Ettepanekud ja kaebused',
              slug: 'ariklient'
            },
            {
              label: 'Turvalisus',
              slug: 'noortepank'
            },
            {
              label: 'Teata petulehest',
              slug: 'lapsekonto'
            },
            {
              label: 'KKK'
            },
            {
              label: 'Privaatpangandus'
            }
          ]
        },
        {
          label: 'LHV',
          submenu: [
            {
              label: 'Ettevõttest',
              slug: 'eraklient',
              link: 'https://lhv.ee'
            },
            {
              label: 'Tööpakkumised',
              slug: 'ariklient'
            },
            {
              label: 'Uudised',
              slug: 'noortepank'
            },
            {
              label: 'Investor',
              slug: 'lapsekonto'
            },
            {
              label: 'Finantsportaal'
            }
          ]
        },
        {
          label: 'KONTAKT',
          submenu: [
            {
              label: 'Kontaktid',
              slug: 'eraklient',
              link: 'https://lhv.ee'
            },
            {
              label: 'Kontorid',
              slug: 'ariklient'
            },
            {
              label: 'Broneeri kohtumisaeg',
              slug: 'noortepank'
            },
            {
              label: 'Sularahaautomaadid',
              slug: 'lapsekonto'
            }
          ]
        }
      ],
      lang: 'et'
    }
  }
}
</script>
<style lang="stylus">
#extra {
  padding: 1.5rem 1rem;
  box-sizing: border-box;
  display: flex;
  background: #f8f8f8;
  right: 0;
  bottom: 0;
  left: 0;
  padding-top: 40;
  padding-bottom: 30;
  font-size: 12px;
  line-height: 18px;
  font-size: 13px;
}

.columns {
  display: block;
  flex-direction: row;
  flex-basis: 25%;
}

.column {
  flex-basis: 100%;
}
</style>