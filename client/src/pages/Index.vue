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
      <div class="text-center" style="padding-top: 5em">
        <img
          alt="Quasar logo"
          src="~assets/neil.png"
          style="width: 250px; height: 250px; border-radius: 10em"
        />
      </div>
    </div>
    <div class="col">
      <div class="text-center q-pt-lg q-px-lg">
        <img
          alt="Quasar logo"
          src="~assets/ux.png"
          style="width: 200px; height: 200px"
        />
      </div>
    </div>
    <!--- Div con informacion personal-->
    <div
      style="margin-top: -0.7em"
      class="col text-center q-pt-lg q-px-lg bg-primary"
    >
      <div class="q-pt-lg q-px-lg" style="padding: 5rem 1.5rem">
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
        background-color: #fff;
        margin-top: -3em;
        border-radius: 12px;
        padding-bottom: 1em;
        margin-right: 1em;
        margin-left: 1em;
        border: 1px solid #e6ecf8;
      "
      class="text- shadow-1 items-center justify-center"
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
            :style="$q.platform.is.mobile ? '' : 'border-right: 1px solid #E6ECF8'"
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
            :style="
              $q.platform.is.mobile
                ? ''
                : 'border-bottom: 0px solid #E6ECF8; border-right: 1px solid #E6ECF8'
            "
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
          Here are some apps I've recently worked on, my startup projects
        </div>
      </div>
    </div>
    <!--Papa tarjetas de los projects-->
    <div
      style="margin-top: -3em; padding-bottom: 15em"
      class="text-center q-pt-lg q-px-lg"
    >
      <div
        class="row items-center justify-center columns is-multiline is-mobile"
      >
        <div
          v-for="info in works"
          :key="info.name"
          class="col-xs-7 col-sm-6 col-md-4"
        >
          <vs-card
            style="padding-left: 1em; padding-top: 1em"
            class="text-bold"
            type="2"
          >
            <template #title>
              <h3>{{ info.title }}</h3>
            </template>
            <template #img>
              <img :src="`${info.img}`" alt="img" />
            </template>
            <template #text>
              <p>{{ info.text }}</p>
            </template>
            <template #interactions>
              <vs-button @click="showsInfo(info)" rounded>
                <q-icon name="info"></q-icon>
              </vs-button>
              <a
                style="text-decoration: none"
                :href="info.btnUrl"
                target="_blank"
              >
                <vs-button
                  class="btn-chat bg-secondary text-black"
                  shadow
                  primary
                  v-if="info.btnUrl"
                >
                  {{ $q.platform.is.mobile ? "Website" : "Visit website" }}
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
          <p class="text-center text-justify">{{ copyInfo.info }}</p>
        </div>

        <template #footer>
          <div class="footer-dialog">
            <vs-button @click="band = false"> Close </vs-button>
          </div>
        </template>
      </vs-dialog>
    </div>

    <section
      class="bg-primary section call-to-action is-primary has-text-centered"
    >
      <div class="container is-narrow">
        <div class="box bg-secondary shadow-1">
          <div class="columns level">
            <div class="column level-item">
              <h3 class="text-bold">Let's start a project</h3>
            </div>
            <div class="columns level-item">
              <p>Interested in a project? we should chat for a bit</p>
            </div>
            <div class="columns level-item">
              <vs-button
                flat
                rounded
                animation-type="vertical"
                class="bg-white text-black"
              >
                Message
                <template #animate> <q-icon name="email" /> Send </template>
              </vs-button>
            </div>
          </div>
        </div>
      </div>
    </section>
    <footer class="section is-primary is-small has-text-centered bg-primary">
      <div class="container is-narrow">
        <div class="text-center q-pt-lg q-px-lg">
          <img
            alt="Img logo"
            src="https://drive.google.com/uc?id=1tJCPjdp0ieJoVliydp5ppvWCDMOqi22E"
            style="width: 200px; height: 200px"
          />
        </div>
        <div class="row q-pa-md items-center justify-center">
          <h5>Living, learning and raising the bar one day at a time.</h5>
        </div>
        <div class="q-pa-md row item-center justify-center">
          <div v-for="btn in btns" :key="btn.name">
            <a :href="btn.url" target="_blank">
              <vs-button circle border dark class="bg-white">
                <box-icon type="logo" :name="btn.name" />
              </vs-button>
            </a>
          </div>
        </div>
      </div>
    </footer>
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
          img: "https://drive.google.com/uc?id=1VoOXKX7eW2hgkeuL4BhZqQ9b56sGTsXL",
          text: "Application and control of academic admission for the Adventist University Institute of Venezuela",
          btnUrl: "https://admision.iunav.com/?#/",
          info: " Web system, developed on the Front-end side with Vue Js (Quasar and Vuesax), on the Back-end side with Nodejs (Adonisjs) and manages a NoSql Database (MongoDB). The main function of the system is to collect the information of the applicants and help them to carry out their admission process, from the delivery of documents, payments, presentation of tests (psychotechnical, knowledge, etc), contact with coordinators or any department of the institute until the approval or denial of the request. It has automatic and personalized email sending, lists and forms for displaying the necessary information, as well as automatic pdf for spreadsheets and others. It is currently in use by the Adventist University Institute of Venezuela",
        },
        {
          title: "Production control",
          img: "https://drive.google.com/uc?id=16ysyk_sJem3gHmYWNZ3C7ToKm0m4GDDm",
          text: "Inventory control application for Organizations-Food in Rio de Janeiro-Brazil",
          btnUrl: "http://sistemas-agricultura-go.es/#/login",
          info: "Web system, developed on the front-end side with Vue Js (Quasar and Vuesax), on the Back-end side with Nodejs (Adonisjs) and manages a NoSql Database (MongoDB). The main function of the system is the control of inventories within Organizations-Food for counting food and carrying out its administrative control.  The system has lists, forms and pdf for the visualization of the necessary data",
        },
        {
          title: "Corporación Visual Sucre C.A",
          img: "https://gitlab.com/bgonzales.wx/telecorp/-/raw/dev/client/src/assets/HomeTv.gif",
          text: "Multiplatform system for cable television company control",
          info: "Multi-platform system, developed on the Front-end side with Vue Js (Quasar and Vuesax), on the Back-end side with Php (Laravel 7) and manages a MySQL Database (PostgreSQl). The main function of the system is inventory control within Corporacion Visual Sucre CA for the registration of its teleclients, monthly charges of debt generated according to the plan per client, the creation of modules for employees (Collectors and Technicians) to know their work daily according to collection or pending work. The system has lists, forms and pdf for the visualization of the necessary data, as well as connection in immediate time for communication between the departments.",
        },
      ],
      btns: [
        {
          name: "facebook",
          url: 'https://www.facebook.com/baironstiven.gonzalezgarcia/',
        },
        {
          name: "linkedin",
          url: 'https://www.linkedin.com/in/bairon-steven-gonzalez-garcia-a24774190',
        },
        {
          name: "whatsapp",
          url: 'https://api.whatsapp.com/send?phone=34651944417'
        },
        {
          name: "gmail",
          url: 'mailto:bgonzales.wx@gmail.com?Subject=Interesado%20en%20un%20trabajo'
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
.section.is-primary
  color: #fff
.section
  padding: 5rem 1.5rem

.section
  padding: 3rem 1.5rem

.has-text-centered
  text-align: center !important

.container.is-narrow
  max-width: 1200px

.container
  -webkit-box-flex: 1
  flex-grow: 1
  margin: 0 auto
  position: relative
  width: auto

*, ::before, ::after
  box-sizing: inherit

.section.is-primary
  color: #fff

.has-text-centered
  text-align: center !important

.section.call-to-action .box
  padding: 3.5rem 2rem
  margin-top: -14rem

.box
  border-radius: 12px

.box
  background-color: white
  border-radius: 6px
  display: block
  padding: 1.25rem

  .columns:last-child
    margin-bottom: -0.75rem

.columns
  margin-left: -0.75rem
  margin-right: -0.75rem
  margin-top: -0.75rem

.level
  -webkit-box-align: center
  align-items: center
  -webkit-box-pack: justify
  justify-content: space-between

.level-item:not(:last-child)
  margin-bottom: 0.75rem

.column
  display: block
  flex-basis: 0
  -webkit-box-flex: 1
  flex-grow: 1
  flex-shrink: 1
  padding: 0.75rem

.level-item
  -webkit-box-align: center
  align-items: center
  display: -webkit-box
  display: flex
  flex-basis: auto
  -webkit-box-flex: 0
  flex-grow: 0
  flex-shrink: 0
  -webkit-box-pack: center
  justify-content: center

.columns.is-multiline
  flex-wrap: wrap

.columns.is-mobile
  display: -webkit-box
  display: flex

.columns:last-child
  margin-bottom: -0.75rem

.vs-card
  max-width: 100%
  max-height: 100%
</style>