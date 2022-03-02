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
          src="~assets/perfil.png"
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
      style="background-color: rgb(236, 236, 236); margin-top: -3em; border-radius: 5em"
      class="col text-center q-pt-lg q-px-lg"
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
          <div style="border-bottom: 0px solid #FFF;border-right: 1px solid #FFF;" class="col-xs-11 col-sm-4 col-md-4">
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
          <div style="border-bottom: 0px solid #FFF;border-right: 1px solid #FFF;" class="col-xs-11 col-sm-4 col-md-4">
            <div class="text-center text-bold text-h5">
              <div class="text-center q-pt-lg q-px-lg">
                <img
                  alt="Quasar logo"
                  src="~assets/back.png"
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
    <div
      class="col text-center q-pt-lg q-px-lg"
    >
      <div class="q-pt-lg q-px-lg">
        <div class="tq-pt-md q-pa-md text-h4 text-center text-bold">
          Hi, I'm Steven. Nice to meet you
        </div>
        <div class="q-pt-md q-pa-xl text-center">
          Since I started my adventure as a freelance web developer almost 3
          years ago, I have worked remotely for agencies, personal entities and
          collaborated with talented people to create digital products for
          commercial use and personal consumption. I am quietly confident,
          naturally curious and perpetually work to improve my skills, to
          provide the best user experience
        </div>
      </div>
    </div>
  </q-page>
</template>

<script>
export default {
  name: "PageIndex",
  data() {
    return {
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
    };
  },
};
</script>
