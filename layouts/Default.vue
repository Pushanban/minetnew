<template>
	<div class="layout">
		<ClientOnly>
			<Header />
			<transition name="fade" tag="div" appear>
				<main>
					<slot />
				</main>
			</transition>
			<Footer class="footer" />
		</ClientOnly>
	</div>
</template>

<script>
import Footer from '../components/Footer'
import Header from '../components/Header'

export default {
	components: {
		Footer,
		Header,
	},
}
</script>

<style>
.fade-enter-active {
	transition: opacity 0.5s;
}

.fade-enter {
	opacity: 0;
}
</style>
