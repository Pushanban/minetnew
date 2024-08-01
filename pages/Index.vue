<template>
  <div>
    <Layout>
      <div class="container">
        <div class="home">
          <div class="flex-center">
            <video width="1220" height="880" autoplay loop muted inline>
              <source src="../assets/images/final14.mp4" type="video/mp4" />
              Your browser does not support the video tag.
            </video>
            <div class="dash">
              <h5 class="semi center date" style="z-index:15">July 28 - August 02, 2022 </h5>
              <div class="butt" style="z-index:10">
                <nuxt-link to="/request/">
                  <button class="left">Request Invite</button>
                </nuxt-link>
                <a href="https://app.minet.co">
                  <button class="right">Access Dashboard</button>
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="u-cf"></div>
      <div class="belowlanding">
        <section id="makes" data-aos="fade">
          <div class="container">
            <div class="makesec">
              <div class="imagemake">
                <div class="center">
                  <img
                    src="../assets/images/make2.svg"
                    alt="Make."
                    class="make"
                    style="margin-bottom:1em; margin-top: 3em"
                    draggable="false"
                  />
                </div>
                <p class="center subtitle semi" style="color: #696969;">
                  Started in Fall 2014, Make is an initiative by the MINET team
                  to celebrate and promote the spirit of entrepreneurship and to
                  <i class="semi">Make</i>
                  useful things.
                </p>
              </div>
              <div class="textmake">
                <h1 class="semi">Make at X.</h1>
                <p>Humans innovate.</p>

                <p>
                  When faced with the seemingly insurmountable, we resort to our
                  inherent ingenuity to deal with it. We make things. Things of
                  utility. Things of majesty. Things that make you stop and
                  think how you didn’t think of a solution so elegant to a
                  problem so daunting.
                </p>

                <p>
                  Every once in a while, one of these things also happens to be
                  a thing of beauty. A paragon of design.
                </p>

                <p>At X, we celebrate just that. And try our best to Make.</p>
              </div>
            </div>
          </div>
        </section>

        <section id="x20" data-aos="fade">
          <div class="container">
            <div class="makesec">
              <div class="textmake">
                <h1 class="semi">X 2022</h1>
                <p>
                  We’re organizing our annual IT symposium, X, from
                  <span class="semi">28 July - 2 August, 2022</span>
                  <span>.</span>
                </p>
                <p>
                  X is an exclusive invite-only event, witnessing participation
                  from all over India. Invites are extended to a select number
                  of the very best schools, based on significant achievements in
                  the previous years.
                </p>
                <p>
                  The event will consist of our online hunt, CryptX, and ten
                  online events — Pitching, Design, Programming, Gaming, Group
                  Discussion, Quiz, Crossword, Surprise, Photography, and a Filmmaking
                  Event. Each event will have a unique theme based around Make.
                </p>
                <p>
                  After two long years, we’re finally hosting the symposium <span class="semi">offline</span>! However, to make sure that 
                  all COVID-19 guidelines and precautions are adhered to, we will be conducting the events 
                  partially online. Participants will be intimated accordingly.

                </p>
                <br />
                <a href="/discord" target="_blank">
                  <button class="primary save cool discordbtn">
                    Join the discord
                  </button>
                </a>
              </div>
              <div class="imagemake">
                <div class="center">
                  <img
                    src="../assets/images/make.svg"
                    alt="Make."
                    class="makeline"
                    draggable="false"
                  />
                </div>
              </div>
            </div>
          </div>
        </section>

        <div class="container">
          <section id="theteam" data-aos="fade">
            <div class="flexteam">
              <div class="teamimg">
                <img
                  src="../assets/images/team3.png"
                  alt
                  class="team"
                  draggable="false"
                />
              </div>
              <div>
                <div class="flex-center">
                  <div class="teamtext">
                    <h1 class="semi">
                      The
                      <br class="nvm" />Team.
                    </h1>
                    <nuxt-link to="/members/" class="memberslink">
                      <button class="cust">
                        <span>meet the members</span>
                        <img
                          src="../assets/images/arrow.png"
                          alt
                          class="arrow"
                          draggable="false"
                        />
                      </button>
                    </nuxt-link>
                  </div>
                </div>
              </div>
            </div>
            <div class="marginplspl"></div>
          </section>
        </div>
      </div>
    </Layout>
  </div>
</template>

<script>
export default {
  metaInfo: {
    title: "Home",
  },
};
</script>

<style lang="scss" scoped>
.flexteam {
  display: flex;
  .teamtext {
    margin-left: 1.3em;
    h1 {
      font-size: 4.5em;
    }
  }
}

@media (max-width: 750px) {
  .flexteam {
    flex-direction: column;
    .memberslink {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
    }
    .teamtext {
      margin-left: 0;
      margin-top: 1em;
      h1 {
        font-size: 3em;
      }
    }
  }
}

.nicebtn {
  border-radius: 2em;
  border-radius: 50px;
  background: #ffffff;
  box-shadow: 25px 25px 50px #a1a1a1, -25px -25px 50px #ffffff;
  transition: 0.5s;
}

.marginplspl {
  height: 3em;
}

.discordbtn {
  margin-top: 1em;
}

.date {
  color: #595959;
  z-index: 3;
  margin: 0;
  margin-bottom: 1em;
  margin-top: -2em;
}

.semi.subtitle {
  font-size: 1em;
  line-height: 1.5em;
}

.cust {
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 4em;
  border: #222;
  transition: 0.5s;
}
.arrow {
  width: 2em;
  margin-left: 1em;
}
#theteam {
  margin-top: 7em;
  margin-bottom: 3em;
}
.team {
  width: 100%;
}
.belowlanding {
  margin-top: 5em;
}
#x20 {
  margin-top: 6em;
  border-top: solid #a1a1a13b;
  border-bottom: solid #a1a1a13b;
  background-color: #f7f7f7a9;
  padding: 5em 0;
}
.make {
  width: 80%;
  margin-top: 1em;
}

.makeline {
  width: 60%;
}

.imagemake,
.textmake {
  width: 45%;
}

.makesec {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
button {
  border-style: none;
  margin: 0;
  color: #222;
  background: #ffffff00;
}
.butt {
  border-radius: 50px;
  display: flex;
  background: #ffffff;
  box-shadow: 25px 25px 50px #a1a1a1, -25px -25px 50px #ffffff;
}

button.right {
  border-radius: 0 50px 50px 0;
}

button.left {
  border-radius: 50px 0 0 50px;
}

button:hover {
  color: #222;
  border-style: none;
  background-color: rgb(228, 228, 228);
}

button.primary {
  color: #fff;
  background-color: #962B44;
  box-shadow: 0px 0px 15px#ca647b;
}

button.primary:hover {
  background-color: #541C4C;
  box-shadow: none;
}
.home {
  color: #222;
//   height: 70vh;
  padding: 2em;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  z-index: -2;
}
@media (max-width: 550px) {
  .nvm {
    display: none;
  }
}


@media (max-width: 750px) {
  .home {
    //height: 35vh;
    width: 100%;
    background-size: cover;
    margin-top: -2em;
  }
  .date {
    margin-top: 0em;
  }
  .respflexcen {
    display: flex;
    justify-content: center;
  }
  .makesec {
    flex-direction: column-reverse;
  }
  .imagemake,
  .textmake {
    width: 100%;
  }
  .imagemake p {
    margin-top: 1em;
  }
  .textmake h1 {
    text-align: center;
  }
  .make {
    margin-top: 2em;
  }
  .makeline {
    display: none;
  }
  #x20 {
    margin-top: 3em;
  }
}
@media (max-width: 353px) {
  .home {
    width: 100%;
    background-size: contain;
  }
}

.home {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.dash {
  margin-top: -9em;
  display: flex;
  flex-direction: column;
}

.minet {
  color: #6699ee;
  margin: 0;
}

.x20 {
  width: 100%;
}

a {
  color: #fff;
  text-decoration: none;
}

.x {
  font-family: "SF medium";
  font-size: 12vw;
}

.minet {
  font-size: 4vw;
}

@media (max-width: 550px) {
  .x {
    font-size: 15vw;
  }

  .minet {
    font-size: 6.5vw;
  }
}

@media (max-width: 1100px) {
	
	.dash {
		margin-top: -2em
	}
}

@media (max-width: 750px) {
  .dash {
    margin-top: -2em;
  }
}
</style>
