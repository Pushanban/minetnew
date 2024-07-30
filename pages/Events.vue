<template>
	<Layout>
		<div class="container">
			<div class="eight columns">
				<div>
					<br />
					<h1 class="zero semi">Events</h1>
					<p class="subtext">
						At X, we want all participants of a team to come together as a
						startup and Make something. All events are interconnected to each
						other, and add toward the final goal of creating a useful product.
						Each event will have a unique theme based around Make. The competition is 
						a compilation of both online and offline events conducted between 28th July to 2nd August.<br>
						You can view the events schedule at <a href="/schedule">X 2022 Schedule</a>.
					</p>
				</div>
			</div>

			<section>
				<b-modal
					v-model="isDesignModalActive"
					has-modal-card
					trap-focus
					:destroy-on-hide="false"
					aria-modal
				>
					<div class="modal-card">
						<h1 class="modalhead">Design</h1>
						<br />
						<div class="modaltext">
							<p>
								One of the two halves of Make, the design team has the
								responsibility of handling your startup and building it from the
								ground up.
							</p>
							<p>
								The prompt will be available at <b>Coming Soon</b>. You
								must make something novel, something you and only you have come
								up with.
							</p>
							<p>
								All teams are required to present a prototype of their product.
								This can be accompanied by any other multimedia presentation
								such as mockups, videos, websites or 3D models, it is completely
								up to you.
							</p>
							<p>These will be judged independently of the pitching event.</p>

							<p>
								<b>Number of Participants</b> : 3 <br>
								<b>Eligibility</b> : Open <br>
								<b>Format</b> : Online Submission
							</p>
							<div class="flex-center">
								<button class="close save" @click="isDesignModalActive = false">close</button>
							</div>
						</div>
					</div>
				</b-modal>

				<b-modal
					v-model="isPitchingModalActive"
					has-modal-card
					trap-focus
					:destroy-on-hide="false"
					aria-modal
				>
					<div class="modal-card">
						<h1 class="modalhead">Pitching</h1>
						<br />
						<div class="modaltext">
							<p>
								Following up on the product built by the design team, the
								pitchers will be presenting the designed project in front of a
								panel of judges, on the
								<span
									class="semi"
								>1st of August</span>
								<span>.</span>
							</p>
							<p>
								The winner, along with two runner-ups shall be decided.
								Alongside this, five teams will qualify to take part in Make,
								which will occur on the
								<span
									class="semi"
								>2nd of August</span>
								<span>.</span>
							</p>
							<p>
								Details regarding Make will be sent to the qualified teams in
								due time.
							</p>

							<p>
								<b>Number of Participants</b> : 2 <br>
								<b>Eligibility</b> : Open <br>
								<b>Format</b> : Offline
							</p>

						</div>
						<div class="flex-center">
							<button class="close save" @click="isPitchingModalActive = false">close</button>
						</div>
					</div>
				</b-modal>

				<b-modal
					v-model="isQuizModalActive"
					has-modal-card
					trap-focus
					:destroy-on-hide="false"
					aria-modal
				>
					<div class="modal-card">
						<h1 class="modalhead">Quiz</h1>
						<br />
						<div class="modaltext">
							<p> Around the irregular contours of Knowledge, seek to arrive at the answer not just with 
								what you know but from what you can read between. Seemingly normal? No. Welcome to Quiz
								at X. 
</p>

							<p>
								A timed preliminary round will be held <b>online</b>.
							</p>
							<p>
								Participants scoring the most points will proceed to the final
								round, which will be held offline during the <b>offline</b> dates.
							</p>

							<p>
								Details are available on our
								<a href="/discord">Discord Server</a>
								<span>.</span>
							</p>
							
							<p>
								<b>Number of Participants</b> : 2 <br>
								<b>Eligibility</b> : Open <br>
								<b>Format</b> : 
									Round 1 : Online <b>|</b> Round 2 : Offline
							</p>
						</div>
						<div class="flex-center">
							<button class="close save" @click="isQuizModalActive = false">close</button>
						</div>
					</div>
				</b-modal>

				<b-modal
					v-model="isCrossModalActive"
					has-modal-card
					trap-focus
					:destroy-on-hide="false"
					aria-modal
				>
					<div class="modal-card">
						<h1 class="modalhead">Crossword</h1>
						<br />
						<div class="modaltext">

							<p>
								 -(WORD)-
							</p>

							<p>
								Join our
								<a href="/discord" target="_blank">Discord Server</a> to stay updated.
							</p>

							<p>
								<b>Number of Participants</b> : 1 <br>
								<b>Eligibility</b> : Open <br>
								<b>Format</b> : Online
							</p>
						</div>
						<div class="flex-center">
							<button class="close save" @click="isCrossModalActive = false">close</button>
						</div>
					</div>
				</b-modal>


				<b-modal
					v-model="isGamingModalActive"
					has-modal-card
					trap-focus
					:destroy-on-hide="false"
					aria-modal
				>
					<div class="modal-card">
						<h1 class="modalhead">Gaming</h1>
						<br />
						<h2 class="quote">"Video games foster the mindset that allows creativity to flow"</h2>
						<p class="gamequote">- Nolan Bushnell</p>
						<div class="modaltext">
							<p>
								 A marathon of dexterity, agility, coordination and sheer presence of mind, participants 
								are tested to the limit in a wide range of games, ranging from obscure to popular. Remember, 
								you can run, but you can never hide.

							</p>
							<p>
								With games being revealed on the spot, we test your ability to
								think fast in difficult situations and how fast you can react to
								change.
							</p>
							<p>Good luck gamers, you will need it.</p>

							<p>
								<b>Number of Participants</b> : 2 <br>
								<b>Eligibility</b> : Open <br>
								<b>Format</b> : 
									Round 1 : Online <b>|</b> Rest of the Rounds : Offline
							</p>
						</div>
						<div class="flex-center">
							<button class="close save" @click="isGamingModalActive = false">close</button>
						</div>
					</div>
				</b-modal>
				<b-modal
					v-model="isProgModalActive"
					has-modal-card
					trap-focus
					:destroy-on-hide="false"
					aria-modal
				>
					<div class="modal-card">
						<h1 class="modalhead">Programming</h1>
						<br />
						<div class="modaltext">
							<p>
								This year the programming event will consist of two independent parts.
							</p>
							<p><b>Online Prompt Release</b>
								<ul>
							<li>A ‘very-specific’ prompt will be released on the 29th July, 2022 (Friday) at 9:41am. </li>
							<li>Participants are required to make a fully-functioning program based on the prompt.</li>
							<li>Note that plus points for projects involving GUI and web-based developments</li>
							<li>The final project needs to be submitted by 31st July, 2022 (Sunday) 9:41pm through google forms, via link of the google drive containing the project, a ‘README’ file and all other prerequisites required to run the project.</li>
								</ul>
							</p>

							<p><b>Offline Competitive Programming</b>
								<ul>
							<li>The offline event to be held on the 1st August, 2022 in offline mode at school. </li>
							<li>The event would be 2 hours long and conducted through HackerRank using the school’s systems</li>
							<li>All languages endorsed by HackerRank can be used by the participants.</li>
								</ul>
							</p>

							<p>
								None is a qualifying round, and participants can take part in both the rounds. The Offline CP is compulsory, while the Online Prompt Release is optional, though recommended. The final scores will be obtained by clubbing the scores of both the parts in ratio 36% (Online Prompt Release) and 64% (Offline CP)
							</p>
								
							<p>
								<b>Number of Participants</b> : 2 <br>
								<b>Eligibility</b> : Open <br>
								<b>Format</b> : Offline
							</p>
						</div>
						<div class="flex-center">
							<button class="close save" @click="isProgModalActive = false">close</button>
						</div>
					</div>
				</b-modal>

				<b-modal
					v-model="isGDModalActive"
					has-modal-card
					trap-focus
					:destroy-on-hide="false"
					aria-modal
				>
					<div class="modal-card">
						<div class="anti"></div>
						<h1 class="modalhead">Group Discussion</h1>
						<br />
						<div class="modaltext">
							<p>
								 Enlightening conversation centered around the questions that plague 
								technology today. Participants will have to discuss constructively and come to a collaborative 
								conclusion.

							</p>

							<p>
								This event will test your critical thinking process as well as
								your ability to formulate and present your views and thoughts.
								Showcase your knowledge, thinking and verbal skills in this
								highly competitive event in front of the judges to come out as
								the victor.
							</p>
							<p>
								Standard criteria for judging group discussion will be followed
								and adequate research time will be provided for the topic if
								required.
							</p>

							<p>
								Prelims will be held on the
								<span class="semi">1st of August</span>
								<span>.</span>
							</p>

							<p>
								Those participants selected will appear for the Finals on
								<span class="semi">2nd of August</span>
								for the top positions.
							</p>

							<p>
								Join our
								<a href="/discord" target="_blank">Discord Server</a> to stay updated.
							</p>

							<p>
								<b>Number of Participants</b> : 1 <br>
								<b>Eligibility</b> : Open <br>
								<b>Format</b> : Offline
							</p>
						</div>
						<div class="flex-center">
							<button class="close save" @click="isGDModalActive = false">close</button>
						</div>
					</div>
				</b-modal>

				<b-modal
					v-model="isCryptModalActive"
					has-modal-card
					trap-focus
					:destroy-on-hide="false"
					aria-modal
				>
					<div class="modal-card">
						<h1 class="modalhead">CryptX</h1>
						<br />
						<div class="modaltext">
							<p>
								Our trademark cryptic hunt, CryptX will take commence at
								<span
									class="semi"
								>9:41 AM on the 28th of July</span>
								<span>,</span>
								and will conclude at
								<span class="semi">9:41 PM, on the 29th of July</span>
								<span>.</span>
							</p>
							<p>
								The hunt will take place at
								<a href="//cryptx.co" target="_blank">cryptx.co</a>
								<span>.</span>
							</p>
							<p class="zero">
								Hints shall be provided over our traditional point of CryptX
								communication - Slack. Details for accounts will be provided
								soon.
							</p><br>
							<p>
								Join our
								<a href="/discord" target="_blank">Discord Server</a> to stay updated.
							</p>

							<p>
								<b>Number of Participants</b> : Infinite <br>
								<b>Eligibility</b> : Open <br>
								<b>Format</b> : Online
							</p>
						</div>
						<div class="flex-center">
							<button class="close save" @click="isCryptModalActive = false">close</button>
						</div>
					</div>
				</b-modal>

				<b-modal
					v-model="isPhotographyModalActive"
					has-modal-card
					trap-focus
					:destroy-on-hide="false"
					aria-modal
				>
					<div class="modal-card">
						<h1 class="modalhead">Photography</h1>
						<br />
						<div class="modaltext">
							<p>
								Carved in illusions so persuasive, and molded to the vibrance of monochrome 
								and the paradoxes of colour; each emotion so distinct in its singularity and yet so compellingly 
								similar in conformity, sparked by creativity, forged by perfection, and founded by a story. Artists 
								will have to work with intense determination to produce the best piece of art in this 
								theme-specific event.
							</p>
							<p>
								You will be asked to submit a photo within the given timeframe
								after the reveal of the prompt in school during the <b>offline dates</b>.
							</p>
							<p>
								The topics will test your out-of-the-box thinking, and ability
								to relate and convert the prompts to actual photos.
							</p>
							<p>
								<b>Number of Participants</b> : 1 <br>
								<b>Eligibility</b> : Open <br>
								<b>Format</b> : Offline
							</p>
						</div>
						<div class="flex-center">
							<button class="close save" @click="isPhotographyModalActive = false">close</button>
						</div>
					</div>
				</b-modal>

				<b-modal
					v-model="isFilmModalActive"
					has-modal-card
					trap-focus
					:destroy-on-hide="false"
					aria-modal
				>
					<div class="modal-card">
						<div class="anti"></div>
						<h1 class="modalhead">Filmmaking</h1>
						<br />
						<div class="modaltext">
							<h5>
								Prompt:
								<span class="semi"><a href="https://minet.co/filmmakingprompt">Here</a></span>
							</h5>
							<br />
							<h5>
								Submission Deadline:
								<span class="semi"> 9:41 PM 31st July</span>
							</h5>
							<br />You will be judged upon the following:
							<ul class="filmul">
								<li>Relevance to Theme</li>
								<li>Originality</li>
								<li>Creativity</li>
								<li>Cinematography</li>
							</ul>

							<p>
								<b>Number of Participants</b> : 4 <br>
								<b>Eligibility</b> : Open <br>
								<b>Format</b> : Submission
							</p>
							<div class="flex-center">
								<button class="close save" @click="isFilmModalActive = false">close</button>
							</div>
						</div>
					</div>
				</b-modal>

				<b-modal
					v-model="isSurpriseModalActive"
					has-modal-card
					trap-focus
					:destroy-on-hide="false"
					aria-modal
				>
					<div class="modal-card">
						<div class="centermod">
							<h1 class="modalhead" style="text-align:left">You expected an event description</h1>
							<br />
							<g-image draggable="false" class="dio" src="~/assets/images/icons/pikapika.png" />

							<p style="text-align:left">
								<b>Number of Participants</b> : 2 <br>
								<b>Eligibility</b> : Open <br>
								<b>Format</b> : Round 1 : Online <b>|</b> Rest of the Rounds : Offline
							</p>
						</div>
						<div class="flex-center">
							<button class="close save" @click="isSurpriseModalActive = false">close</button>
						</div>
					</div>
				</b-modal>
			</section>

			<div class="u-cf"></div>
			<div class="flex-center">
				<div id="events" data-aos="fade">

					<div class="event card" @click="isDesignModalActive = true">
						<div class="cardhed">
							<g-image class="eventimg" src="~/assets/images/icons/Design.png" alt />
							<h2>Design</h2>
						</div>
						<div class="content">
							<p>Premier Product Design by Professional Practitioners.</p>
						</div>
						<br />
						<br />
						<hr />
						<div class="info">
							<div class="mem">
								<span class="no">3</span>
								<h5>Members</h5>
							</div>
							<a href="#" class="read">READ MORE</a>
						</div>
					</div>

					<div class="event card" @click="isPitchingModalActive = true">
						<div class="cardhed">
							<g-image class="eventimg" src="~/assets/images/icons/Pitching.png" alt />
							<h2>Pitching</h2>
						</div>
						<div class="content">
							<p>Premier Product Pitching by Professional Practitioners.</p>
						</div>
						<br />
						<br />
						<hr />
						<div class="info">
							<div class="mem">
								<span class="no">2</span>
								<h5>Members</h5>
							</div>
							<a href="#" class="read">READ MORE</a>
						</div>
					</div>
					
					

					

					<div class="event card" @click="isQuizModalActive = true">
						<div class="cardhed">
							<g-image class="eventimg" src="~/assets/images/icons/Quiz.png" alt />
							<h2>Quiz</h2>
						</div>
						<div class="content">
							<p>
								X has always been known for turning the traditional Quiz format
								on its head, and this year is no different.
							</p>
						</div>
						<br />
						<hr />
						<div class="info">
							<div class="mem">
								<span class="no">2</span>
								<h5>Members</h5>
							</div>
							<a href="#" class="read">READ MORE</a>
						</div>
					</div>

					<div class="event card" @click="isCrossModalActive = true">
						<div class="cardhed">
							<g-image class="eventimg" src="~/assets/images/icons/Cross.png" alt />
							<h2>Crossword</h2>
						</div>
						<div class="content">
							<p>
								Time for wordplay and bad puns. <br> 
								Good Luck.
							</p>
						</div>
						<br />
						<hr />
						<div class="info">
							<div class="mem">
								<span class="no">1</span>
								<h5>Member</h5>
							</div>
							<a href="#" class="read">READ MORE</a>
						</div>
					</div>

					<div class="event card" @click="isGamingModalActive = true">
						<div class="cardhed">
							<g-image class="eventimg" src="~/assets/images/icons/Game.png" alt />
							<h2>Gaming</h2>
						</div>
						<div class="content">
							<p>You like playing games? We like watching you rage :)</p>
							<br />
							<br />
						</div>
						<hr />
						<div class="info">
							<div class="mem">
								<span class="no">2</span>
								<h5>Members</h5>
							</div>
							<a href="#" class="read">READ MORE</a>
						</div>
					</div>

					<div class="event card" @click="isGDModalActive = true">
						<div class="cardhed">
							<g-image class="eventimg" src="~/assets/images/icons/GD.png" alt />
							<h2>GD</h2>
						</div>
						<div class="content">
							<p>
								Forget the conventional GD. We test your desicion-making skills under immense, immense pressure. 
								Are you up for this task?
							</p>
						</div>
						<hr />
						<div class="info">
							<div class="mem">
								<span class="no">1</span>
								<h5>Member</h5>
							</div>
							<a href="#" class="read">READ MORE</a>
						</div>
					</div>

					<div class="event card" @click="isProgModalActive = true">
						<div class="cardhed">
							<g-image class="eventimg" src="~/assets/images/icons/Programming.png" alt />
							<h2 class="proghead">Programming</h2>
						</div>
						<div class="content">
							<p>Materials required: Brain.	<br />
							Maybe a computer but mostly a brain. Yes, that's about it.</p>
							<br />
							<!-- <br /> -->
						</div>
						<hr />
						<div class="info">
							<div class="mem">
								<span class="no">2</span>
								<h5>Members</h5>
							</div>
							<a href="#" class="read">READ MORE</a>
						</div>
					</div>

					

					<div class="event card" @click="isSurpriseModalActive = true">
						<div class="cardhed">
							<g-image class="eventimg" src="~/assets/images/icons/Surprise.png" alt />
							<h2>Surprise</h2>
						</div>
						<div class="content">
							<p>At this point you've read all variations of</p>
							<p>
								"expect the unexpected", but lets be honest hum dono ko pata hai
								kya hota hai.
							</p>
							
						</div>
						<hr />
						<div class="info">
							<div class="mem">
								<span class="no">2</span>
								<h5>Members</h5>
							</div>
							<a href="#" class="read">READ MORE</a>
						</div>
					</div>



					<div class="event card" @click="isCryptModalActive = true">
						<div class="cardhed">
							<g-image class="eventimg" src="~/assets/images/icons/Crypt.png" alt />
							<h2>CryptX</h2>
						</div>
						<div class="content">
							<p>
								Our trademark cryptic hunt, is back online, again.
								Wait, it always has been.
								<br />
								<br />	
							</p>
						</div>
						<hr />
						<div class="info cryptpt">
							<div class="mem">
								<!-- <span class="no">∞</span> -->
								<h5>infinite</h5>
							</div>
							<a href="#" class="read">READ MORE</a>
						</div>
					</div>

					<div class="event card" @click="isPhotographyModalActive = true">
						<div class="cardhed">
							<g-image class="eventimg" src="~/assets/images/icons/Photo.png" alt />
							<h2 class="proghead">Photography</h2>
						</div>
						<div class="content">
							<p>Take picture - > Get gud - > Win prize.</p>
							<br />
						
						</div>
						<br />
						<hr />
						<div class="info">
							<div class="mem">
								<span class="no">1</span>
								<h5>Member</h5>
							</div>
							<a href="#" class="read">READ MORE</a>
						</div>
					</div>

					<div class="event card" @click="isFilmModalActive = true">
						<div class="cardhed">
							<g-image class="eventimg" src="~/assets/images/icons/Film.png" alt />
							<h2>Filmmaking</h2>
						</div>
						<div class="content">
							<p>Picture abhi baaki hai ( actually picture abhi banani hai ), mere participant.</p>
						</div>
					
						<br />
						<hr />
						<div class="info">
							<div class="mem">
								<span class="no">4</span>
								<h5>Members</h5>
							</div>
							<a href="#" class="read">READ MORE</a>
						</div>
					</div>
				</div>
			</div>
		</div>
	</Layout>
</template>

<script>
export default {
	metaInfo: {
		title: 'Events',
	},
	data() {
		return {
			isDesignModalActive: false,
			isPitchingModalActive: false,
			isQuizModalActive: false,
			isCrossModalActive: false,
			isGamingModalActive: false,
			isGDModalActive: false,
			isProgModalActive: false,
			isPhotographyModalActive: false,
			isFilmModalActive: false,
			isSurpriseModalActive: false,
			isCryptModalActive: false,
		}
	},
	
}
</script>

<style scoped lang="scss">
.modalhead {
	font-size: 30px;
}

hr {
	margin-bottom: 0em;
	margin-top: 0.2em;
	width: 100%;
	background-color: transparent !important;
}

.blue {
	background: #92c8f1;
	margin: none;
	border-radius: 17px;
}
.info {
	display: flex;
	justify-content: space-between;
	align-items: center;
	h5 {
		font-size: 1.0em;
	}
	.mem {
		display: flex;
		justify-content: flex-start;
		align-items: center;
		text-transform: uppercase;
		h5 {
			font-family: "EuroBold";
			font-size: 1em;
			letter-spacing: 1.3px;
			// margin-bottom: 0.5em;
			color: rgb(116, 116, 116);
		}
		.no {
			font-size: 3em;
			font-family: "EuroBold";

			margin-right: 0.3em;
			-webkit-text-stroke: 1px #000;
			color: transparent;
		}
	}
}
.content p,
.filmul li {
	margin: 0;
}

.centermod {
	margin: 5em;
	text-align: center;
}

.quote {
	font-size: 1.4em;
}

.gamequote {
	margin-bottom: 1em;
	text-align: right;
}
.cardhed {
	display: flex;
	justify-content: flex-start;
	align-items: center;
	margin-top: 1em;
	margin-bottom: 0.5em;
	h2 {
		-webkit-text-stroke: 0.8px #000;
		color: #fff;
		font-size: 35px;
		letter-spacing: 0em;
		margin-top: -0.5em;
		font-family: "EuroBold";
	}
	::-moz-selection {
		-webkit-text-stroke: transparent;
	}
	::selection {
		-webkit-text-stroke: transparent;
	}
}

.info.cryptpt {
	margin: 1.5em 0;
}

.proghead {
	font-size: 30px;
}

.eventimg {
	width: 20%;
	margin-right: 3%;
	margin-bottom: 1em;
	background: #92c8f1;
	border-radius: 13px;
}

a.read {
	font-size: 0.8em;
	font-family: "EuroBold";
	letter-spacing: 1.3px;
}

.event.card {
	padding: 1em 2em 0.3em 1em;
	width: 100%;
	border-radius: 1em;
	margin-bottom: 2em;
	box-shadow: 10px 10px 24px #e6e6e6, -10px -10px 24px #fff;
}

.modal-card {
	overflow: none;
	background: #fff;
	color: #222;
	padding: 2em;
	border-radius: 2em;
	.flex-center {
		.save {
			color: #fff;
			display: none;
		}
	}
}

@media (max-width: 750px) {
	.modal-card {
		.flex-center {
			.save {
				display: block;
			}
		}
	}
}

.modal-contain {
	align-items: center;
	margin-left: 50vh;
}

li {
	margin-left: 1em;
}

.width100 {
	width: 100%;
	background-color: #6699ee;
	border: none;
}

h1,
h2,
h3,
h4,
h5,
h6 {
	margin: 0;
}

.event.card:hover {
	cursor: pointer;
}

#events {
	display: grid;
	grid-gap: 2em;
	grid-template-columns: repeat(3, 1fr);
	margin-top: 2em;
	margin-bottom: 1em;
}

@media (max-width: 970px) {
	#events {
		grid-template-columns: repeat(2, 1fr);
	}
}
@media (max-width: 550px) {
	.modal-card {
		height: 120vh;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		overflow: scroll;
		.modalhead {
			margin-top: 2em;
		}
	}
}

@media (max-width: 700px) {
	#events {
		display: grid;
		grid-gap: 2em;
		grid-template-columns: repeat(1, 1fr);
		width: 100%;
	}

	.subtext {
		font-size: 1.15em;
	}
}

.anti {
	display: none;
}

@media (max-height: 600px) {
	.anti {
		display: block;
		margin-top: 50vh;
	}
}
</style>
