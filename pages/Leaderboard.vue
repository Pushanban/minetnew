<template>
	<Layout>
		<div class="container">
			<br />
			<h1 class="zero semi">Leaderboard</h1>
			<h5 class="subtext">Overall Leaderboard</h5>
			<table class="leaderboardtable">
				<thead>
					<tr class="header">
						<th class="center">Rank</th>
						<th class="center">School</th>
						<th class="center">Level</th>
					</tr>
				</thead>

				<tbody>
					<tr v-for="(team, index) in info" :key="team.school">
						<td class="center ranking">{{ index + 1 }}</td>
						<td id="name">
							<a href="#">{{ team.school }}</a>
						</td>
						<td class="center">${{ team.funds.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ',') }}</td>
					</tr>
				</tbody>
			</table>
		</div>
	</Layout>
</template>

<script>
import leaderboard from '@/assets/data/leaderboard.json'

export default {
	metaInfo: {
		title: 'Leaderboard',
	},
	data() {
		return {
			info: leaderboard.info,
			loading: false,
		}
	},
}
</script>

<style scoped lang="scss">
.leaderboardtable {
	margin-top: 2em;
	margin-bottom: 5em;
}

table {
	width: 100%;
	border-collapse: collapse;
	overflow: scroll;
	margin-bottom: 4em;
}

.center {
	text-align: center;
}

td:hover {
	background-color: #f5f5f5;
}

td,
th {
	padding: 12px;
}

.iconldrb {
	width: 20%;
}

@media (max-width: 750px) {
	td,
	th {
		font-size: 1em;
	}
	.tableimg {
		width: 3em;
	}
}

.loadingcont {
	height: 80vh;
	display: flex;
	justify-content: center;
	align-items: center;
}

.loadbro {
	color: #3567be;
	font-size: 20px;
	margin: 100px auto;
	width: 1em;
	height: 1em;
	border-radius: 50%;
	position: relative;
	text-indent: -9999em;
	-webkit-animation: load4 1.3s infinite linear;
	animation: load4 1.3s infinite linear;
	-webkit-transform: translateZ(0);
	-ms-transform: translateZ(0);
	transform: translateZ(0);
}

@-webkit-keyframes load4 {
	0%,
	100% {
		box-shadow: 0 -3em 0 0.2em, 2em -2em 0 0em, 3em 0 0 -1em, 2em 2em 0 -1em,
			0 3em 0 -1em, -2em 2em 0 -1em, -3em 0 0 -1em, -2em -2em 0 0;
	}
	12.5% {
		box-shadow: 0 -3em 0 0, 2em -2em 0 0.2em, 3em 0 0 0, 2em 2em 0 -1em,
			0 3em 0 -1em, -2em 2em 0 -1em, -3em 0 0 -1em, -2em -2em 0 -1em;
	}
	25% {
		box-shadow: 0 -3em 0 -0.5em, 2em -2em 0 0, 3em 0 0 0.2em, 2em 2em 0 0,
			0 3em 0 -1em, -2em 2em 0 -1em, -3em 0 0 -1em, -2em -2em 0 -1em;
	}
	37.5% {
		box-shadow: 0 -3em 0 -1em, 2em -2em 0 -1em, 3em 0em 0 0, 2em 2em 0 0.2em,
			0 3em 0 0em, -2em 2em 0 -1em, -3em 0em 0 -1em, -2em -2em 0 -1em;
	}
	50% {
		box-shadow: 0 -3em 0 -1em, 2em -2em 0 -1em, 3em 0 0 -1em, 2em 2em 0 0em,
			0 3em 0 0.2em, -2em 2em 0 0, -3em 0em 0 -1em, -2em -2em 0 -1em;
	}
	62.5% {
		box-shadow: 0 -3em 0 -1em, 2em -2em 0 -1em, 3em 0 0 -1em, 2em 2em 0 -1em,
			0 3em 0 0, -2em 2em 0 0.2em, -3em 0 0 0, -2em -2em 0 -1em;
	}
	75% {
		box-shadow: 0em -3em 0 -1em, 2em -2em 0 -1em, 3em 0em 0 -1em, 2em 2em 0 -1em,
			0 3em 0 -1em, -2em 2em 0 0, -3em 0em 0 0.2em, -2em -2em 0 0;
	}
	87.5% {
		box-shadow: 0em -3em 0 0, 2em -2em 0 -1em, 3em 0 0 -1em, 2em 2em 0 -1em,
			0 3em 0 -1em, -2em 2em 0 0, -3em 0em 0 0, -2em -2em 0 0.2em;
	}
}
@keyframes load4 {
	0%,
	100% {
		box-shadow: 0 -3em 0 0.2em, 2em -2em 0 0em, 3em 0 0 -1em, 2em 2em 0 -1em,
			0 3em 0 -1em, -2em 2em 0 -1em, -3em 0 0 -1em, -2em -2em 0 0;
	}
	12.5% {
		box-shadow: 0 -3em 0 0, 2em -2em 0 0.2em, 3em 0 0 0, 2em 2em 0 -1em,
			0 3em 0 -1em, -2em 2em 0 -1em, -3em 0 0 -1em, -2em -2em 0 -1em;
	}
	25% {
		box-shadow: 0 -3em 0 -0.5em, 2em -2em 0 0, 3em 0 0 0.2em, 2em 2em 0 0,
			0 3em 0 -1em, -2em 2em 0 -1em, -3em 0 0 -1em, -2em -2em 0 -1em;
	}
	37.5% {
		box-shadow: 0 -3em 0 -1em, 2em -2em 0 -1em, 3em 0em 0 0, 2em 2em 0 0.2em,
			0 3em 0 0em, -2em 2em 0 -1em, -3em 0em 0 -1em, -2em -2em 0 -1em;
	}
	50% {
		box-shadow: 0 -3em 0 -1em, 2em -2em 0 -1em, 3em 0 0 -1em, 2em 2em 0 0em,
			0 3em 0 0.2em, -2em 2em 0 0, -3em 0em 0 -1em, -2em -2em 0 -1em;
	}
	62.5% {
		box-shadow: 0 -3em 0 -1em, 2em -2em 0 -1em, 3em 0 0 -1em, 2em 2em 0 -1em,
			0 3em 0 0, -2em 2em 0 0.2em, -3em 0 0 0, -2em -2em 0 -1em;
	}
	75% {
		box-shadow: 0em -3em 0 -1em, 2em -2em 0 -1em, 3em 0em 0 -1em, 2em 2em 0 -1em,
			0 3em 0 -1em, -2em 2em 0 0, -3em 0em 0 0.2em, -2em -2em 0 0;
	}
	87.5% {
		box-shadow: 0em -3em 0 0, 2em -2em 0 -1em, 3em 0 0 -1em, 2em 2em 0 -1em,
			0 3em 0 -1em, -2em 2em 0 0, -3em 0em 0 0, -2em -2em 0 0.2em;
	}
}
</style>
