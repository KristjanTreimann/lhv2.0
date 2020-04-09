<template lang="pug">
footer
	.container
		.row
			.col-xs-12.col-md-10.col-md-offset-1.footer-navbar
				.column-50
					h2 Tekst siia
					p
						span 123456
					.col
						p
							| Tekst siia
</template>

<script>
export default {
	name: 'Footer',
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
      ]
		}
	},

}
</script>

<style>

</style>
