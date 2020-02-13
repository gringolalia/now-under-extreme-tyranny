<template lang="pug">
	.page-container
		md-app(md-mode='reveal')
			md-app-toolbar.md-primary
				.md-toolbar-section-start
					md-button.md-icon-button(@click='menuVisible = !menuVisible')
						md-icon menu

					span.md-title
						i.fas.fa-sun.fa-2x
						| &nbsp; Engenho Novo LLC

				.md-toolbar-section-end.ml-0
					i.material-icons.mr-3(n-link="/repentista") waves
					i.material-icons directions_bike

					md-menu(md-direction='bottom-end' mdCloseOnSelect="closeOnSelect")
						md-icon-button(md-menu-trigger)
							i.material-icons more_vert

						md-menu-content.with.dignity
							md-menu-item Peixes
							md-menu-item Porcos
							md-menu-item Bovinos
							md-menu-item Frango e Peru

			md-app

			md-app-drawer(:md-active.sync='menuVisible')
				md-toolbar.md-primary.text-right(md-elevation='0')
					i.material-icons waves
					| &nbsp; San Pavlov, Meu Amor

				md-list(@click="menuVisible = false")

					md-list-item(to="/")
						md-icon transform

						span.md-list-item-text In Principio

					md-list-item(to="/tour-samboja")
						md-icon directions_bike

						span.md-list-item-text Tour de Samboja

					md-list-item(to="/sob-medida")
						md-icon transform

						span.md-list-item-text Sob Medida

					md-list-item(to="/ubatuba")
						md-icon tune

						span.md-list-item-text Afinando Ubatuba

					md-list-item(to="/navegar")
						md-icon flight

						span.md-list-item-text Navegar é Preciso

					md-list-item(to="/malandro")
						md-icon casino

						span.md-list-item-text O Malandro

					md-list-item(to="/repentista")
						md-icon radio

						span.md-list-item-text O Repentista

					md-list-item(to="/remando")
						md-icon rowing

						span.md-list-item-text Remando na Maré

			md-app-content
				nuxt
</template>

<style lang="scss" scoped>
	.md-app {
		height: 100vh;
	}

	 // Demo purposes only
	.md-drawer {
		width: 230px;
		max-width: calc(100vw - 125px);
	}

  .md-menu {
    margin: 24px;
  }
</style>

<script>
export default {
	name: 'Reveal',
	data: () => ({
		menuVisible: false
	})
}
</script>
