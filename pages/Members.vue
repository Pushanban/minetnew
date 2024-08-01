<template>
	<Layout>
		<div class="container">
			<div class="row">
				<div class="seven columns">
					<div>
						<br />
						<h1 class="zero semi">Members</h1>
						<h6 class="subtext">
							A team of designers, developers, gamers, quizzers, photographers,
							filmmakers. This is MINET. We
							<i>Make</i>
							things.
						</h6>
					</div>
				</div>
				<div class="u-cf"></div>
			</div>

			<div class="flex-center">
				<div class="grid">
					<div v-for="member in members" :key="member.id" data-aos="fade" data-aos-duration="1000">
						<div class="cardn">
							<div class="center">
								<img
									:src="`/members${member.photo}`"
									class="memberimg"
									alt="Member"
									draggable="false"
									loading="lazy"
								/>
							</div>
							<h4 class="name">{{ member.name }}</h4>
							<h4 class="pos">{{ member.position }}</h4>
						</div>
					</div>
				</div>
			</div>
		</div>
	</Layout>
</template>

<script>
import members from '~/assets/data/members.json'

export default {
	metaInfo: {
		title: 'Members',
	},
	data() {
		return {
			members: members.members,
		}
	},
}
</script>

<style scoped>
.subtext {
	font-size: 1.3em;
	margin-bottom: 0.2em;
}

.cardn div.center {
	margin-bottom: 0.7em;
}

h1,
h2,
h3,
h4,
h5,
h6 {
	margin: 0;
}

.hoop {
	text-align: center;
}

.is-current {
	background-color: #6699ee;
	color: #fff;
}

.grid {
	display: grid;
	grid-gap: 3em;
	grid-template-columns: repeat(3, 1fr);
	margin: 2em 0;
}

@media (max-width: 750px) {
	.grid {
		display: grid;
		grid-gap: 1.4em;
		grid-template-columns: repeat(1, 1fr);
		width: 100%;
	}
	.columns {
		margin: 0 0 !important;
	}
}

.cardn {
	border-radius: 1.5em;
	padding: 1em 0.5em;
	text-align: center;
	text-transform: capitalize;
	transition: 0.5s;
	border: none;
}

.cardn:hover {
	transform: translateY(-4px);
	border-radius: 1.5em;
	background: #ffffff;
	box-shadow: 16px 16px 30px #d6d6d6, -16px -16px 30px #ffffff;
}

.memberimg {
	width: 50%;
	border-radius: 1em;
}

.name {
	font-size: 1.6em;
}

.pos {
	font-size: 1.2em;
	color: #6699ee;
}
</style>
