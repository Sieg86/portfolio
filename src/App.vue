<template>
  <v-app>
    <div>
      <v-navigation-drawer
      dark
      src="https://cdn.vuetifyjs.com/images/backgrounds/bg-2.jpg"
      permanent
      class="navBar"
    >
    <div class="ctnrImg">
      <v-img
        class="imgSR"
        src="./assets/SébastienROBERT.jpg"
      ></v-img>
    </div>
      <v-list>
        <v-list-item
          v-for="([icon, text, refAnchor], i) in items"
          :key="i"
          link
        >
          <a class="linkMenu" v-bind:href="refAnchor">
          <v-list-item-icon>
            <v-icon>{{ icon }}</v-icon>
          </v-list-item-icon>
          </a>

          <a class="linkMenu sublink" v-bind:href="refAnchor">
          <v-list-item-content>
            <v-list-item-title>{{ text }}</v-list-item-title>
          </v-list-item-content>
          </a>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-main class="content">
      <section id="about" class="resume-section">
        <span class="prenom">
        Sébastien
        </span>
        <span class="nom">
          Robert
        </span>
        <div class="addresseMail">
          <span class="address">2 impasse des biefs 44390 Nort-Sur-Erdre - </span>
          <span class="mail"><a href="mailto:sbrobert86@gmail.com">sbrobert86@gmail.com</a></span>
        </div>
        <div class="btnGit">
          <a href="https://github.com/Sieg86">
          <v-btn
            class="mx-2"
            fab
            dark
            large
            color="#318ED3"
          >
            <v-icon dark>
              mdi-github
            </v-icon>
          </v-btn>
          </a>
        </div>
      </section>
      <v-divider/>
      <section class="resume-section" id="experiences">
        <div class="section-title">
          Expériences
        </div>
        <v-container class="cntr-exp">
          <v-row no-gutters>
            <v-col
              cols="12"
              sm="6"
              md="8"
            >
              <div class="exp-content-title">
                Lorem Ipsum
              </div>
              <div class="exp-content-subtitle">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              </div>
              <div class="exp-content">
                <ul>
                  <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                  <li>Sed aliquam eget ex sit amet ultricies.</li>
                  <li>Maecenas condimentum turpis vitae lacinia tempus.</li>
                  <li>Fusce accumsan sollicitudin neque a pellentesque.</li>
                </ul>
              </div>
            </v-col>
            <v-col
              cols="6"
              md="4"
            >
              <div class="exp-long">
                Lorem Ipsum dolor sit amet.
              </div>
            </v-col>
          </v-row>
        </v-container>
        <v-container class="cntr-exp">
          <v-row no-gutters>
            <v-col
              cols="12"
              sm="6"
              md="8"
            >
              <div class="exp-content-title">
                Lorem Ipsum
              </div>
              <div class="exp-content-subtitle">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              </div>
              <div class="exp-content">
                <ul>
                  <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                  <li>Sed aliquam eget ex sit amet ultricies.</li>
                  <li>Maecenas condimentum turpis vitae lacinia tempus.</li>
                  <li>Fusce accumsan sollicitudin neque a pellentesque.</li>
                </ul>
              </div>
            </v-col>
            <v-col
              cols="6"
              md="4"
            >
              <div class="exp-long">
                Lorem Ipsum dolor sit amet.
              </div>
            </v-col>
          </v-row>
        </v-container>
        <v-container class="cntr-exp">
          <v-row no-gutters>
            <v-col
              cols="12"
              sm="6"
              md="8"
            >
              <div class="exp-content-title">
                Lorem Ipsum
              </div>
              <div class="exp-content-subtitle">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              </div>
              <div class="exp-content">
                <ul>
                  <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                  <li>Sed aliquam eget ex sit amet ultricies.</li>
                  <li>Maecenas condimentum turpis vitae lacinia tempus.</li>
                  <li>Fusce accumsan sollicitudin neque a pellentesque.</li>
                </ul>
              </div>
            </v-col>
            <v-col
              cols="6"
              md="4"
            >
              <div class="exp-long">
                Lorem Ipsum dolor sit amet.
              </div>
            </v-col>
          </v-row>
        </v-container>
      </section>
      <v-divider/>
      <section class="resume-section" id="diplomes">
        <div class="section-title">
          Diplômes
        </div>
        <div class="exp-content-title">
          Lorem Ipsum
        </div>
        <div class="exp-content-subtitle">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit.
        </div>
        <div class="exp-content-title">
          Lorem Ipsum
        </div>
        <div class="exp-content-subtitle">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit.
        </div>
        <div class="exp-content-title">
          Lorem Ipsum
        </div>
        <div class="exp-content-subtitle">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit.
        </div>
        
      </section>
      <v-divider/>
      <section class="resume-section" id="competences">
        <div class="section-title">
          Compétences
        </div>
      </section>
      
    </v-main>
    </div>
  </v-app>
</template>

<script>

export default {
  
  name: 'App',

  components: {
  },

  data: () => ({
    items: [
        ['mdi-information-outline', 'À propos', '#about'],
        ['mdi-account-supervisor-circle-outline', 'Expériences', '#experiences'],
        ['mdi-certificate-outline', 'Diplômes', '#diplomes'],
        ['mdi-application-brackets-outline', 'Compétences', '#competences'],
        ['mdi-briefcase-outline', 'Portfolio', ''],
        ['mdi-card-account-phone-outline', 'Contact', ''],
      ],
  }),
};
</script>
<style>
.sublink{
  padding: 0.5rem 2rem;
}
  html{
    scroll-behavior: smooth;
  }
  .navBar{
    width:14% !important;
    position: fixed;
    height:100%;
  }
  .imgSR{
    width: 9rem;
    border-radius: 50%;
  }
  .ctnrImg{
    margin-top:50%;
    margin-left: auto;
    margin-right: auto;
    width:10rem;
  }
  .content{
    margin-top:10%;
    margin-left:19rem;
  }
  .prenom{
    text-transform: uppercase;
    font-size: 35px;
  }
  .nom{
    text-transform: uppercase;
    color:#318ED3;
    font-size: 35px;
    font-weight: bold;
  }
  .addresseMail{
    text-transform: uppercase;
    font-size:14px;
  }
  .mail{
    color:#318ED3;
    font-weight: bold;
  }
  a:link{
    text-decoration: none;
  }
  .btnGit{
    margin-top:2rem;
  }
  .section-title{
    margin-top:1rem;
    margin-bottom: 2rem;
    text-transform: uppercase;
    font-size:20px;
    font-weight: bold;
  }
  .resume-section{
    min-height: 100vh;
  }
  .style11 {
	height: 6px;
	background: url(http://ibrahimjabbari.com/images/hr-11.png) repeat-x 0 0;
    border: 0;
}
.exp-content-title{
  font-size:18px;
  font-weight: 450;
}
.exp-content-subtitle{
  color:slategray;
  font-size: 17px;
  font-weight: 350;
  margin-bottom: 1rem;
}
.exp-long{
  color:#318ED3;
  font-weight: 500;
}
.cntr-exp{
  margin-bottom: 2rem;
}
.linkMenu{
  color:white !important;
}
</style>