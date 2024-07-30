<template>
	<Layout>
		<div class="container vh">
			<div class="shi">
				<h1 class="sad">:(</h1>
				<h2 class="oopsie">
					Oopsie Woopsie! Uwu we made a yucky wucky!! A wittle messy boingo! The
					code monkeys at our headquarters are working VEWY HAWD to fix this!
				</h2>
				<h5>404</h5>
				<h5 class="homelink">
					<g-link to="/">go back home 🥺</g-link>
				</h5>
			</div>
		</div>
	</Layout>
</template>

<script>
export default {
	metaInfo: {
		title: '404',
	},
}
</script>

<style scoped>
.sad {
	font-size: 10em;
	margin-bottom: 0.1em;
}
.vh {
	height: 80vh;
	display: flex;
	justify-content: center;
	align-content: center;
	flex-direction: column;
	margin-bottom: 5em;
}

@media (max-width: 550px) {
	.vh {
		height: auto;
		display: block;
		margin-top: 2em;
	}
	.sad {
		margin-top: 0.3em;
		margin-bottom: 0.3em;
		font-size: 5em;
		z-index: -2;
	}
	.oopsie {
		font-size: 2em;
	}
	h5.homelink {
		margin-bottom: 6em;
	}
}
</style>
