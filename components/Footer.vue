<template>
	<div class="footer">
		<div class="container">
			<div class="flexer">
				<h6>
					<a href="http://themis.in" target="_blank">The Mother's International School</a>
				</h6>

				<h6>
					<a href="//madewithlove.org.in" target="_blank">
						Made with
						<font-awesome-icon :icon="['fas', 'heart']" />&nbsp;in India
					</a>
				</h6>
			</div>
			<div class="u-cf"></div>
		</div>
	</div>
</template>

<style lang="scss" scoped>
h6,
a {
	margin: 0;
}

footer.footer .container {
	margin: 0;
	padding: 0;
}

.footer {
	border-top: solid 1px rgba(34, 34, 34, 0.199);
	margin: 0;
	padding: 0;
	padding: 1em 0;
	a {
		color: #222;
		transition: 0.2s;
	}
	a:hover {
		color: #6699ee;
	}
}

.flexer {
	display: flex;
	justify-content: space-between;
	align-items: center;
}

@media (max-width: 550px) {
	.flexer {
		flex-direction: column;
	}
}

.heart {
	width: 15px;
	color: rgb(209, 74, 74);
}

.teams {
	display: flex;
}

.extra {
	margin-top: 1em;
	h5 {
		margin: 0;
	}
	p {
		margin: 0;
	}
	.firstrow {
		margin-right: 2em;
	}
}
</style>
