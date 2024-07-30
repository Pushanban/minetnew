<template>
	<Layout>
		<div class="container">
			<br />
			<h1 class="zero semi">FAQs</h1>
			<h5 class="subtext">Frequently Asked Questions about X.</h5>
			<div class="flex-center">
				<div class="widthcust">
					<b-collapse class="collapse card" animation="slide" aria-id="q1">
						<div slot="trigger" slot-scope="props" class="card-header" role="button" aria-controls="q1">
							<p class="card-header-title">What is X? Who can attend?</p>
							<a class="card-header-icon">
								<font-awesome v-if="props.open" :icon="['fas', 'times']" />
								<font-awesome v-else :icon="['fas', 'plus']" />
							</a>
						</div>
						<div class="card-content">
							<div class="content">
								X is The Mother’s International School’s annual technology
								symposium. X is an exclusive invite-only event, and invites are
								extended to a select number of the very best schools in India,
								based on significant achievements in the previous years.
							</div>
						</div>
					</b-collapse>

					<b-collapse :open="false" class="card" animation="slide" aria-id="q2">
						<div slot="trigger" slot-scope="props" class="card-header" role="button" aria-controls="q2">
							<p class="card-header-title">How is X going to be held this time?</p>
							<a class="card-header-icon">
								<font-awesome v-if="props.open" :icon="['fas', 'times']" />
								<font-awesome v-else :icon="['fas', 'plus']" />
							</a>
						</div>
						<div class="card-content">
							<div class="content">
								In light of the pandemic, X 2022 will be held partially online and partially offline. While most
								preliminary rounds will take place online, the finals will be held offline at The Mother’s 
								International School. All events and information to be communicated will be through MINET X’s 
								official discord which can be found <a
									href="//minet.co/discord"
								>here</a>
								. Otherwise, head over to

								<g-link to="/events/">minet.co/events</g-link>
								<span>.</span>
							</div>
						</div>
					</b-collapse>

					<b-collapse :open="false" class="card" animation="slide" aria-id="q2">
						<div slot="trigger" slot-scope="props" class="card-header" role="button" aria-controls="q2">
							<p class="card-header-title">When is X? How do I register for it?</p>
							<a class="card-header-icon">
								<font-awesome v-if="props.open" :icon="['fas', 'times']" />
								<font-awesome v-else :icon="['fas', 'plus']" />
							</a>
						</div>
						<div class="card-content">
							<div class="content">
								<p class="zero">
									X will be held from 28th July - 2nd August 2022. Confirmatory registration of the events will be provided 
									at the start itself. You can request an invite to X at 

									<g-link to="/request/">minet.co/request</g-link>
									<span>.</span> You can view the registration tutorial <g-link to="https://youtu.be/1MRQ0cO67zg">here</g-link> <span>.</span>
								</p>
							</div>
						</div>
					</b-collapse>

					<b-collapse :open="false" class="card" animation="slide" aria-id="q2">
						<div slot="trigger" slot-scope="props" class="card-header" role="button" aria-controls="q2">
							<p class="card-header-title">
								What exactly is Make? How does it work?
							</p>
							<a class="card-header-icon">
								<font-awesome v-if="props.open" :icon="['fas', 'times']" />
								<font-awesome v-else :icon="['fas', 'plus']" />
							</a>
						</div>
						<div class="card-content">
							<div class="content">
								<p class="zero">
									Make is the cumulative event that's made up of Design and Pitching.<br>
									<br>
									<b>What comprises design?</b><br>
									The design team ( 3 members ) has the responsibility of handling the startup and building it from the ground up. All teams are required to present a prototype of their product that can be accompanied by any other multimedia presentation
									such as mockups, videos, websites or 3D models, etc.<br>
									It is an online submission-based event, i.e the team has to hand in their deliverables via google drive before the deadline on the 31st of August. These will be judged independently of the pitching event.
									<br><i>Only people submitting their designs can participate in Pitching and Make.</i><br>
									Following up on the product built by the design team, the pitching team ( 2 Members ) will be presenting the fully prototyped project in front of a panel of judges, on the 1st of August, offline.
									<br><br>
									<b>Who can participate in Pitching?</b><br>

									The Pitching event requires two members for each team. These members can be from the Design team itself, but registering two new members is recommended.<br>

									The winner, along with two runner-ups shall be decided. Alongside this, a few handpicked teams will be qualified to take part in Make. The judges-turned-mentors will then be helping the same teams better their product. The teams will thus present their refurbished projects on the 2nd of August, offline in order to compete for the Make winner title.
								</p>
							</div>
						</div>
					</b-collapse>

					<b-collapse :open="false" class="card" animation="slide" aria-id="q2">
						<div slot="trigger" slot-scope="props" class="card-header" role="button" aria-controls="q2">
							<p class="card-header-title">What is the last date of registration?</p>
							<a class="card-header-icon">
								<font-awesome v-if="props.open" :icon="['fas', 'times']" />
								<font-awesome v-else :icon="['fas', 'plus']" />
							</a>
						</div>
						<div class="card-content">
							<div class="content">
								<p class="zero">
									The last date of requesting an invite is 26th July 2022 at 2:00 PM. You can do so at
									<g-link to="/request/">minet.co/request</g-link>
									<span>.</span><br>

									The last date of registering your team is 29th July 2022 at 2:00 PM. You can do so at
									<g-link to="https://app.minet.co/rsvp">app.minet.co/rsvp</g-link>
									<span>.</span>
								</p>
							</div>
						</div>
					</b-collapse>

					<b-collapse :open="false" class="card" animation="slide" aria-id="q2">
						<div slot="trigger" slot-scope="props" class="card-header" role="button" aria-controls="q2">
							<p class="card-header-title">My school hasn’t received an invite code yet. What do I do?</p>
							<a class="card-header-icon">
								<font-awesome v-if="props.open" :icon="['fas', 'times']" />
								<font-awesome v-else :icon="['fas', 'plus']" />
							</a>
						</div>
						<div class="card-content">
							<div class="content">
								We’re sending out invite codes on a rolling basis. If your
								school hasn’t received an invite code, you can request one at
								<g-link to="/request/">minet.co/request</g-link>
								<span>.</span>
								For specific information regarding the events, head to
								<g-link to="/events/">minet.co/events</g-link>
								<span>.</span>
							</div>
						</div>
					</b-collapse>

					<b-collapse :open="false" class="card" animation="slide" aria-id="q2">
						<div slot="trigger" slot-scope="props" class="card-header" role="button" aria-controls="q2">
							<p class="card-header-title">
								Can I participate in clashing events? And is there a limit to
								how many events I can attend?
							</p>
							<a class="card-header-icon">
								<font-awesome v-if="props.open" :icon="['fas', 'times']" />
								<font-awesome v-else :icon="['fas', 'plus']" />
							</a>
						</div>
						<div class="card-content">
							<div class="content">
								<p class="zero">
									There is no limit to how many events you can participate in.
									It's upto you whether or not you can manage clashing events
									and timings.
								</p>
							</div>
						</div>
					</b-collapse>

					

					<b-collapse :open="false" class="card" animation="slide" aria-id="q3">
						<div slot="trigger" slot-scope="props" class="card-header" role="button" aria-controls="q3">
							<p class="card-header-title">How does the scoring system work?</p>
							<a class="card-header-icon">
								<font-awesome v-if="props.open" :icon="['fas', 'times']" />
								<font-awesome v-else :icon="['fas', 'plus']" />
							</a>
						</div>
						<div class="card-content">
							<div class="content">
								<p>
									Winning each event rewards teams with a certain amount of
									funding, which contributes to their overall valuation:
								</p>
								<ul>
									<li>1st: $100,000</li>
									<li>2nd: $75,000</li>
									<li>3rd: $50,000</li>
								</ul>
								<p>Teams can also raise funds by the following means:</p>
								<ol>
									<li>
										$5,000 for each level completed in CryptX along with bonuses
										for top 3 positions.
									</li>
									<li>
										Upto $100,000 from each investor in the fundraising session
										on August 2nd.
									</li>
									<li>For each event you participate you get $5,000.</li> 
								</ol>
								<p>The team with the maximum valuation wins the overall prize.</p>
							</div>
						</div>
					</b-collapse>
				</div>
			</div>
			<div class="u-cf"></div>

			<div class="fkn">
				<section id="more">
					<div class="seven columns">
						<div>
							<h1 class="zero semi">Need help?</h1>
							<h6 class="subtext less">
								We're here to help. Reach out to us via our official
								<a
									href="//instagram.com/minetclub"
									target="_blank"
								>
									<span>Instagram</span>
								</a>
								<span>,&nbsp;</span>
								<a href="mailto:minet@themis.in">Email</a>
								<span>,&nbsp;</span>
								<a href="//facebook.com/minet.mis">Facebook</a>
								or
								<a href="//minet.co/discord">Discord Server</a>
								<span>.</span>
								If you want to speak to us over the phone, DM us on Instagram
								and we’ll arrange a call with an official.
							</h6>
							<div class="buttons noselect">
								<a href="//minet.co/discord" target="_blank">
									<button class="button-primary save cool mright">
										<font-awesome :icon="['fab', 'discord']" style="width:1.2em; margin-top: 0.3em;"/>&nbsp;Discord
									</button>
								</a>
								<br class="anti" />
								<a href="//instagram.com/minetclub" target="_blank">
									<button class="button-primary save cool mright">
										<font-awesome :icon="['fab', 'instagram']" style="width:1.2em; margin-top: 0.3em;"/>&nbsp;minetclub
									</button>
								</a>
								<br class="anti" />
								<a href="mailto:minet@themis.in" target="_blank">
									<button class="button-primary save cool mright">
										<font-awesome :icon="['fas', 'envelope']" style="width:1.2em; margin-top: 0.3em;" />&nbsp;minet@themis.in
									</button>
								</a>
							</div>
						</div>
					</div>
					<div class="five columns">
						<div class="yoinsta flex-center">
							<img
								draggable="false"
								@click="igRedirect()"
								loading="lazy"
								class="insta"
								src="../assets/images/nametag.png"
							/>
						</div>
					</div>
					<div class="u-cf"></div>
				</section>
			</div>
		</div>
		<br />
	</Layout>
</template>

<script>
export default {
	metaInfo: {
		title: 'FAQs',
	},
	methods: {
		igRedirect() {
			window.open('https://instagram.com/minetclub', '_blank');
		}
	}
}
</script>

<style scoped lang="scss">
.subtext.less {
	margin-bottom: 0em;
}
#more {
	margin-top: 8em;
	padding-bottom: 4em;
	.mright {
		margin-right: 2em;
	}
	button i {
		color: #fff;
	}
}

.fkn {
	margin-top: 4em;
}

.flex-center {
	display: flex;
	justify-content: center;
	align-items: center;
	flex-direction: column;
}

.insta {
	width: 70%;
	border-radius: 15px;
	border: solid rgba(102, 152, 238, 0.5) 1px;
	transition: 0.3s;
}

.insta:hover {
	border: solid rgba(102, 152, 238, 1) 1px;
	cursor: pointer;
}

.yoinsta.flex-center {
	align-items: flex-end;
}

.widthcust {
	width: 70%;
}

.contactmore {
	margin-top: 8em;
}

.card-header-title {
	font-weight: 200;
	font-family: "eurobold";
	font-size: 1.1em;
}

@media (max-width: 550px) {
	.subtext.less {
		margin-bottom: 2em;
	}
}

@media (max-width: 750px) {
	.insta {
		margin: 0 !important;
	}
	.yoinsta.flex-center {
		align-items: center;
		margin-top: 2em;
		margin-bottom: -1em;
	}
}
@media (max-width: 700px) {
	.widthcust {
		width: 100%;
	}
	.buttons {
		display: flex;
		flex-direction: column;
		margin-bottom: 2em;
		width: 100%;
		a {
			width: 100%;
		}
	}
	button {
		width: 100% !important;
		margin: 0;
	}
	#more .mright {
		margin-right: 0;
	}
	button.button-primary.save.dash {
		width: 100%;
	}
}

.collapse.card {
	background-color: rgb(250, 250, 250);
	.card-header-title {
		margin: 0;
		margin: 0.5em 0;
	}
}

.card-content {
	background-color: rgb(240, 240, 240);
	:hover {
		background-color: rgb(240, 240, 240);
	}
}

.subtext.butt {
	margin-bottom: 0.5em;
}
</style>
