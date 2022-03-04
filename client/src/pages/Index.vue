<template>
  <q-page class="fullscreen q-pt-lg">
    <div class="col q-pt-lg q-px-md">
      <div class="text-h3 text-center text-bold">
        Designer, cross-platform full stack developer
      </div>
      <div class="q-pt-lg text-light text-center">
        I design and code and develop systems and websites on a small and large
        scale, making your job a simple task
      </div>
      <div class="text-center">
        <img
          alt="Quasar logo"
          src="~assets/neil.png"
          style="width: 200px; height: 200px; border-radius: 7em"
        />
      </div>
    </div>
    <div class="col">
      <div class="text-center q-pt-lg q-px-lg">
        <img
          alt="Quasar logo"
          src="~assets/fondo2.png"
          style="width: 200px; height: 200px"
        />
      </div>
    </div>
    <!--- Div con informacion personal-->
    <div
      style="background-color: #1976d2"
      class="col text-center q-pt-lg q-px-lg"
    >
      <div class="q-pt-lg q-px-lg">
        <div class="tq-pt-md q-pa-md text-h4 text-center text-white text-bold">
          Hi, I'm Steven. Nice to meet you
        </div>
        <div class="q-pt-md q-pa-xl text-center text-white">
          Since I started my adventure as a freelance web developer almost 3
          years ago, I have worked remotely for agencies, personal entities and
          collaborated with talented people to create digital products for
          commercial use and personal consumption. I am quietly confident,
          naturally curious and perpetually work to improve my skills, to
          provide the best user experience
        </div>
      </div>
    </div>
    <!--Div flotador con las tecnologias que manejo-->
    <div
      style="
        background-color: rgb(236, 236, 236);
        margin-top: -3em;
        border-radius: 5em;
        padding-bottom: 1em;
      "
      class="col text-center q-pt-lg q-px-lg shadow-1"
    >
      <div class="q-pt-lg q-px-lg">
        <div
          class="
            q-pt-md q-pa-md q-pb-lg
            text-h4 text-center text-black text-bold
          "
        >
          I'll explain a little what I do
        </div>
        <div class="row">
          <div
            style="border-bottom: 0px solid #fff; border-right: 1px solid #fff"
            class="col-xs-11 col-sm-4 col-md-4"
          >
            <div class="text-center text-bold text-h5">
              <div class="text-center q-pt-lg q-px-lg">
                <img
                  alt="Quasar logo"
                  src="~assets/front.png"
                  style="width: 70px; height: 70px"
                />
              </div>
              Front-end
            </div>
            <div class="q-pa-xl text-center">
              I like to code things from scratch and enjoy bringing ideas to
              life in the browser.
            </div>
            <div class="q-pa-md text-center text-bold text-h7 text-secondary">
              Languages I speak
            </div>
            <div class="text-center">HTML, CSS, Sass, Less</div>
            <div class="q-pa-md text-center text-bold text-h7 text-secondary">
              I also manage some frameworks to give life to the app
            </div>
            <div class="text-center">Vue (Quasar, Vuesax, Vuetify), React</div>
            <div class="q-pa-md text-center text-bold text-h7 text-secondary">
              Dev Tools:
            </div>
            <div v-for="index in devTools" :key="index" class="text-center">
              {{ index }}
            </div>
          </div>
          <div
            style="border-bottom: 0px solid #fff; border-right: 1px solid #fff"
            class="col-xs-11 col-sm-4 col-md-4"
          >
            <div class="text-center text-bold text-h5">
              <div class="text-center q-pt-lg q-px-lg">
                <img
                  alt="Quasar logo"
                  src="~assets/yuna.png"
                  style="width: 70px; height: 70px"
                />
              </div>
              Back-end
            </div>
            <div class="q-pa-xl text-center text-black">
              I like to write light, short and precise code for handling data
            </div>
            <div class="q-pa-md text-center text-bold text-h7 text-secondary">
              Languages I speak
            </div>
            <div class="text-center">JavaScript and PHP</div>
            <div class="q-pa-md text-center text-bold text-h7 text-secondary">
              I also manage some frameworks to give life to the app
            </div>
            <div class="text-center">AdonisJs and Laravel</div>
            <div class="q-pa-md text-center text-bold text-h7 text-secondary">
              Dev Tools:
            </div>
            <div v-for="index in backTools" :key="index" class="text-center">
              {{ index }}
            </div>
          </div>
          <div class="col-xs-11 col-sm-4 col-md-4">
            <div class="text-center text-bold text-h5">
              <div class="text-center q-pt-lg q-px-lg">
                <img
                  alt="Quasar logo"
                  src="~assets/db.png"
                  style="width: 70px; height: 70px"
                />
              </div>
              Databases
            </div>
            <div class="q-pa-xl text-center text-black">
              I analyze the need you have in order to instantiate the database
              that suits your need
            </div>
            <div class="q-pa-md text-center text-bold text-h7 text-secondary">
              Languages I speak
            </div>
            <div class="text-center">MySql and NoSql</div>
            <div class="q-pa-md text-center text-bold text-h7 text-secondary">
              Within them are managed:
            </div>
            <div v-for="index in bdTools" :key="index" class="text-center">
              {{ index }}
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="col text-center q-pt-lg q-px-lg">
      <div class="q-pt-lg q-px-lg">
        <div class="q-pt-md q-pa-md text-h4 text-center text-bold">
          My Recent Work
        </div>
        <div class="q-pt-md q-pa-xl text-center">
          Here are some apps I've recently worked on
        </div>
      </div>
    </div>
    <!--Papa tarjetas de los projects-->
    <div
      style="margin-top: -3em; padding-bottom: 1em;"
      class="text-center q-pt-lg q-px-lg"
    >
      <div class="row items-center justify-center">
        <div
          v-for="info in works"
          :key="info.name"
          class="col-xs-9 col-sm-4 col-md-4"
        >
          <vs-card style="padding-left: 1em;padding-top: 1em;" class="text-bold" type="2">
            <template #title>
              <h3>{{ info.title }}</h3>
            </template>
            <template #img>
              <img :src="`${info.img}`" alt="" />
            </template>
            <template #text>
              <p>{{ info.text }}</p>
            </template>
            <template #interactions>
              <vs-button @click="showsInfo(info)" rounded>
                <q-icon name="info"></q-icon>
              </vs-button>
              <a :href="info.btnUrl" target="_blank">
                <vs-button
                  class="btn-chat bg-secondary text-black"
                  shadow
                  primary
                >
                  Visit website
                  <q-icon style="margin-left: 0.5em" name="done" />
                </vs-button>
              </a>
            </template>
          </vs-card>
        </div>
      </div>
      <vs-dialog prevent-close v-model="band">
        <template #header>
          <h4 class="not-margin">{{ copyInfo.title }}</h4>
        </template>

        <div class="con-form">
          <p class="text-center text-justify">{{copyInfo.info}}</p>
        </div>

        <template #footer>
          <div class="footer-dialog">
            <vs-button @click="band = false"> Close </vs-button>
          </div>
        </template>
      </vs-dialog>
    </div>
  </q-page>
</template>

<script>
export default {
  name: "PageIndex",
  data() {
    return {
      band: false,
      copyInfo: {},
      devTools: [
        "Visual Studio Code",
        "Bitbucket",
        "Bootstrap",
        "Bootstrap-vue",
        "Bulma",
        "Codekit",
        "Codepen",
        "Github",
        "Gitlab",
        "Terminal",
      ],
      backTools: [
        "Visual Studio Code",
        "Bitbucket",
        "Codepen",
        "Github",
        "Gitlab",
        "Terminal",
      ],
      bdTools: ["MySQL", "Oracle Database", "PostgreSQL", "MongoDB"],
      works: [
        {
          title: "Academic Admission",
          img: "back.png",
          text: "Application and control of academic admission for the Adventist University Institute of Venezuela",
          btnUrl: "https://admision.iunav.com/?#/",
          info: " Web system, developed on the Front-end side with Vue Js (Quasar and Vuesax), on the Back-end side with Nodejs (Adonisjs) and manages a NoSql Database (MongoDB). The main function of the system is to collect the information of the applicants and help them to carry out their admission process, from the delivery of documents, payments, presentation of tests (psychotechnical, knowledge, etc), contact with coordinators or any department of the institute until the approval or denial of the request. It has automatic and personalized email sending, lists and forms for displaying the necessary information, as well as automatic pdf for spreadsheets and others. It is currently in use by the Adventist University Institute of Venezuela",
        },
        {
          title: "Production control",
          img: "two.png",
          text: "Inventory control application for Organizations-Food in Rio de Janeiro-Brazil",
          btnUrl: "http://sistemas-agricultura-go.es/#/login",
          info: "Web system, developed on the front-end side with Vue Js (Quasar and Vuesax), on the Back-end side with Nodejs (Adonisjs) and manages a NoSql Database (MongoDB). The main function of the system is the control of inventories within Organizations-Food for counting food and carrying out its administrative control.  The system has lists, forms and pdf for the visualization of the necessary data",
        },
      ],
    };
  },
  methods: {
    async showsInfo(info) {
      this.copyInfo = info;
      this.band = true;
    },
  },
};
</script>
<style lang="sass">
.vs-button
  font-size: 12pt

.a
  text-decoration: none
</style>