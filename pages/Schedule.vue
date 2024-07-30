<template>
	<Layout>
		<div class="container">
			<div class="desk">
				<div class="page-content">
					<div class="eight columns">
						<div>
							<br />
							<h1 style="color:#2b2b2b" class="zero semi">Schedule</h1>

						<p class="subtext">28 July - 02 August, 2022</p>
						</div>
					</div>
					
					<div class="u-cf"></div>
					<DayOne />
				</div>
			</div>

			<div class="download">
				<div class="flex-center">
					<h1 class="semi zero">Schedule</h1>
					<h5 class="zero">28 July - 02 August, 2022</h5>
					<a href="/x22.pdf">
						<button class="button-primary save cool">Download</button>
					</a>
				</div>
			</div> 
			
		</div>
	</Layout>
</template>


<script>
import DayOne from '../components/dayone.vue'
import DayTwo from '../components/daytwo.vue'

export default {
	metaInfo: {
		title: 'Schedule',
	},
	components: {
		DayOne,
		DayTwo,
	},
}
</script>

<style scoped>
.subtext {
	font-size: 1.3em;
}
.subtext:last-child {
	margin-bottom: 0.2em;
}
a {
	color: #6699ee;
	transition: all 0.3s;
}
a:hover {
	color: #b721ff;
}

.tabbed {
	overflow-x: hidden;
	margin: 32px 0;
	padding-bottom: 16px;
}

.tabbed [type="radio"] {
	display: none;
}

.tabs {
	display: flex;
	justify-content: center;
	align-items: center;
	list-style: none;
	padding: 0;
}

.tab > label {
	display: block;
	margin-bottom: -1px;
	border: 1px solid #ccc;
	background: #eee;
	color: #666;
	font-size: 12px;
	font-weight: 600;
	text-transform: uppercase;
	letter-spacing: 1px;
	cursor: pointer;
	transition: all 0.3s;
	border: none;
	padding: 0.5em 2em;
}

.tab.day1 > label {
	border-radius: 1em 0 0 1em;
}

.tab.day2 > label {
	border-radius: 0 1em 1em 0;
}

.tab:hover label {
	color: #333;
}

.tab-content {
	display: none;
	color: #777;
}

.tabbed [type="radio"]:nth-of-type(1):checked ~ .tabs .tab:nth-of-type(1) label,
.tabbed [type="radio"]:nth-of-type(2):checked ~ .tabs .tab:nth-of-type(2) label,
.tabbed [type="radio"]:nth-of-type(3):checked ~ .tabs .tab:nth-of-type(3) label,
.tabbed [type="radio"]:nth-of-type(4):checked ~ .tabs .tab:nth-of-type(4) label,
.tabbed
	[type="radio"]:nth-of-type(5):checked
	~ .tabs
	.tab:nth-of-type(5)
	label {
	border-bottom-color: #fff;
	background: #6699ee;
	color: #fff;
}

.tabbed [type="radio"]:nth-of-type(1):checked ~ .tab-content:nth-of-type(1),
.tabbed [type="radio"]:nth-of-type(2):checked ~ .tab-content:nth-of-type(2),
.tabbed [type="radio"]:nth-of-type(3):checked ~ .tab-content:nth-of-type(3),
.tabbed [type="radio"]:nth-of-type(4):checked ~ .tab-content:nth-of-type(4) {
	display: block;
}

.download {
	height: 80vh;
	display: flex;
	justify-content: center;
	align-items: center;
	display: none;
	flex-direction: column;
	padding-top: 20vh;
}

@media (max-width: 1000px) {
	.download {
		display: block;
	}
	.desk {
		display: none;
	}
}
</style>
