<template>
  <Layout>
    <div data-aos="fade">
      <div class="container">
        <h1 class="zero semi">Request an Invite</h1>
        <h5 class="subtext">Fill out the form below if your team hasn’t recieved an invite yet.</h5>

        <div class="flex-center" id="theboxthing">
          <div class="six columns">
            <div class="card" id="request">
              <h3 class="subtext">{{msg.msg}}</h3>
              <form v-if="!submitted" @submit="addUser">
                <label for>Name of School</label>
                <input type="text" required v-model="school" name id placeholder="School" />
                <label for>Point of Contact</label>
                <input type="text" required v-model="name" name id placeholder="Name of Student" />
                <label for>Email</label>
                <input type="email" required v-model="email" name id placeholder="Email" />
                <label for>Website</label>
                <textarea
                  name="website"
                  id
                  cols="30"
                  rows="10"
                  v-model="website"
                  required
                  placeholder="Website and other relevant links"
                ></textarea>
                <div class="flex-center">
                  <button class="save button-primary cool" :disabled="disable">
                    <span v-if="!loading">Request</span>
                    <span v-if="loading">Loading</span>
                  </button>
                </div>
              </form>
            </div>
          </div>
          <div class="u-cf"></div>
        </div>
        <div class="u-cf"></div>

        <div class="fkn">
          <section id="more">
            <div class="seven columns">
              <div>
                <h1 class="zero semi">Need help?</h1>
                <h6 class="subtext">
                  We're here to help. Reach out to us via our official
                  <a
                    href="//instagram.com/minetclub"
                    target="_blank"
                  >Instagram</a>,
                  <a href="mailto:minet@themis.in">Email</a>,
                  <a href="//facebook.com/minet.mis">Facebook</a> or
                  <a href="//minet.co/discord">Discord</a> server. If you want
                  to speak to us over the phone, DM us on Instagram and we’ll arrange a call with an official.
                </h6>
                <div class="buttons noselect">
                  <a href="//minet.co/discord">
                    <button class="button-primary save cool mright">Discord</button>
                  </a>
                  <br class="anti" />
                  <a href="//instagram.com/minetclub" target="_blank">
                    <button class="button-primary save cool mright">
                      <i class="fab fa-instagram"></i>
                      minetclub
                    </button>
                  </a>
                  <br class="anti" />
                  <a href="mailto:minet@themis.in" target="_blank">
                    <button class="button-primary save cool mright">
                      <i class="far fa-envelope"></i>
                      minet@themis.in
                    </button>
                  </a>
                </div>
              </div>
            </div>
            <div class="five columns">
              <div class="flex-center">
                <g-image draggable="false" class="insta" src="../assets/images/nametag.png" />
              </div>
            </div>
            <div class="u-cf"></div>
          </section>
        </div>
      </div>
    </div>
  </Layout>
</template>

<script>
import axios from "axios";
export default {
  metaInfo: {
    title: "Request",
  },
  data() {
    return {
      disable: false,
      loading: false,
      school: "",
      name: "",
      email: "",
      website: "",
      submitted: false,
      msg: "",
    };
  },
 
  methods: {
    async addUser(e) {
      e.preventDefault();
      this.disable = true;
      this.loading = true;
      await axios
        .post("https://localhost:5000/request", {
          pName: this.name,
          insName: this.school,
          links: this.website,
          email: this.email,
        })
        .then((response) => {
          const data = response.data;
          //console.log(data);
          this.msg = data;
        });
      this.loading = false;
      this.submitted = true;
    },
  },
};
</script>

<style scoped lang="scss">
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

button {
  color: #fff;
}

button:disabled {
  background-color: #4371c2;
  transform: translateY(0px);
  -webkit-box-shadow: none;
  -moz-box-shadow: none;
  box-shadow: none;
}

.insta {
  width: 70%;
  border-radius: 30px;
  margin-top: 1em;
	border-radius: 15px;
	border: solid rgba(102, 152, 238, 0.5) 1px;
	transition: 0.3s;
  margin-left: 10em;
  // margin-bottom: 5em;
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

.widthcust {
  width: 70%;
}

.contactmore {
  margin-top: 8em;
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
#theboxthing {
  margin-bottom: 4em;
}
.marginbtm {
  margin: 2em;
}

button {
  margin: 0;
  margin-top: 1em;
}

.marginbhai {
  margin-top: 4em;
}

#request {
  margin-top: 2em;
}
.card {
  width: 100%;
  padding: 2em 2em 0.2em 2em;
  border-radius: 1.5em;
}
.rightalign {
  text-align: right;
}
button i {
  color: #fff;
  font-size: 1em;
}
.mright {
  margin-right: 01em;
}
.messenger {
  width: 70%;
  margin-bottom: 1em;
}
#more {
  margin-top: 5em;
  margin-bottom: 6em;
}

.cust {
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 4em;
  border: #222;
  transition: 0.5s;
}
.cust:hover {
  background: rgb(182, 182, 182);
  box-shadow: 20px 20px 60px #d5d5d5, -20px -20px 60px #ffffff;
}
.arrow {
  width: 2em;
  margin-left: 1em;
}
input,
textarea {
  min-width: 100%;
  max-width: 100%;
}
.center {
  text-align: center;
}

.title {
  margin-bottom: 0.5em;
}
/* .vh {
	height: 80vh;
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	width: 100%;
} */
@media (max-width: 750px) {
  .card.req {
    width: 100%;
  }
}
</style>