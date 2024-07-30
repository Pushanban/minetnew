<template>
	<header class="header">
				<div class="nav">
			<div class="container">
				<nav>
					<div>
						<nuxt-link to="/" class="minet">MINET</nuxt-link>
					</div>
					<div class="right">
						<nuxt-link to="/events/">Events</nuxt-link>
						<nuxt-link to="/members/">Members</nuxt-link>
						<nuxt-link to="/schedule/">Schedule</nuxt-link>
						<nuxt-link to="/faqs/">FAQs</nuxt-link>

						<div class="tog" @click="open = true">
							<p class="rightbro">
								<img src="../assets/images/side.png" alt />
							</p>
						</div>
					</div>
				</nav>
			</div>
		</div>
	</header>
</template>


<script>
export default {
	data() {
		return {
			open: false,
			overlay: true,
			fullheight: true,
			fullwidth: true,
			right: true,
		}
	},
}
</script>

<style>
.mobminet {
	width: 4em;
}
.closebtn {
	width: 1.5em;
	position: absolute;
	top: 2em;
	right: 2em;
}
.sideside .minet {
	margin-top: 3em;
}
.sideside .top {
	margin-top: 5em;
}
.sideside a.active--exact.active {
	color: rgb(17, 73, 170);
}
.blue {
	color: #6699ee;
}
.tog {
	display: none;
	border: none;
	padding-top: 0.8em;
}
.tog img {
	padding: 0.2em;
	width: 1.8em;
	height: 1.8em;
}

.tog img:hover {
	background: #6698ee5d;
	border-radius: 2em;
	border: none;
	outline: none;
	transition: 1s;
}

.tog:focus {
	outline: none;
}

.navbarside {
	width: 100%;
}
.test-modal .modal-dialog {
	max-width: 100%;
	margin: 0;
	top: 0;
	bottom: 0;
	left: 0;
	right: 0;
	height: 100vh;
	display: flex;
	position: fixed;
	z-index: 100000;
}
.heart {
	color: #e74c3c;
}

div#app {
	display: flex;
	flex-direction: column;
	height: 100%;
}

footer.footer {
	margin-top: auto;
	margin-top: 3em;
	padding-top: 1em;
	border-top: solid #a1a1a13b;
	background-color: #f7f7f7a9;
}

nav {
	display: flex !important;
	justify-content: space-between;
	align-items: center;
	padding: 1.5em 0;
	z-index: 2;
	margin: 0;
}

.minet {
	font-size: 2.5em;
}

.right {
	text-transform: uppercase;
	display: flex;
}

.rightbro {
	text-align: right;
}

.right a {
	margin-left: 1.5em;
	font-size: 1.1em;
	color: #7f879b;
}

a.active--exact.active {
	color: #962B44;
}

/* @media (max-width: 750px) {
  .right {
    display: none;
    margin-top: 10em;
  }
} */

@media (max-width: 750px) {
	.right a {
		flex-wrap: wrap;
		flex-direction: column;
		display: none;
	}
	.tog {
		display: block;
	}
	nav {
		margin-top: -1em;
		/* margin: auto; */
		/* padding: auto; */
	}
}

#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	color: #2c3e50;
}

.zero {
	margin: 0;
}

.rightside {
	text-align: right;
}

/* .footer p {
  margin: 0;
} */

@media (max-width: 750px) {
	.rightside {
		text-align: center;
	}
	.footer {
		text-align: center;
	}
}
</style>
