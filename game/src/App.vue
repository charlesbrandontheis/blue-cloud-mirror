<template>
  <div id="app">
    <b-navbar toggleable="md" type="dark" style="background-color: #053c9f !important;">
      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
      <b-navbar-brand style="margin-right:40px">Blue Cloud Mirror - IBM Cloud Showcase</b-navbar-brand>

      <b-collapse is-nav id="nav_collapse">
        <b-navbar-nav>
          <b-nav-item>
            <router-link style="color:white" to="/about">About</router-link>
          </b-nav-item>
          <b-nav-item>
            <router-link style="color:white" to="/start">Start</router-link>
          </b-nav-item>
          <b-nav-item>
            <router-link style="color:white" to="/emotions">Emotions</router-link>
          </b-nav-item>
          <b-nav-item>
            <router-link style="color:white" to="/poses">Poses</router-link>
          </b-nav-item>
          <b-nav-item>
            <router-link style="color:white" to="/results">Results</router-link>
          </b-nav-item>
          <li class="nav-item">
            <a href="#" class="nav-link">
              <a
                target="_blank"
                href="https://blue-cloud-mirror-highscore.de-cloudfoundry-check-cl.eu-de.containers.appdomain.cloud/"
                class
                style="color: white;"
              >Highscores</a>
            </a>
          </li>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <b-container>
      <div style="margin-top:20px;"></div>
      <notchrome></notchrome>
      <router-view/>
      <b-row>
        <b-col style="text-align:center">
          <div style="margin-top:50px;margin-bottom:10px;font-size: smaller;color: darkgray;">Brought to you by the <a target="_blank" style="color:#053c9f" href="https://developer.ibm.com/cities/berlin-de/">IBM Developer Advocacy DACH</a> team</div>
          <div style="margin-top:10px;margin-bottom:10px;font-size: smaller;color: darkgray;">Read more about the code pattern <a target="_blank" style="color:#053c9f" href="https://developer.ibm.com/patterns/cloud-showcase-blue-mirror/">Mirror game app showcases 15 cloud technologies and components</a></div>
          <div style="margin-top:10px;margin-bottom:10px;font-size: smaller;color: darkgray;">Get a free <a target="_blank" style="color:#053c9f" href="https://ibm.biz/nheidloff">IBM Cloud</a> account. Get the <a target="_blank" style="color:#053c9f" href="https://github.com/ibm/blue-cloud-mirror">code</a></div>
          <div style="margin-top:10px;margin-bottom:10px;font-size: smaller;color: darkgray;"><a target="_blank" style="color:#053c9f" href="https://www.ibm.com/privacy/us/en/">IBM Privacy Statement</a> and <a target="_blank" style="color:#053c9f" href="https://www.ibm.com/legal/us/en/">Terms of Use</a></div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>


<script>
import notchrome from '@/components/NotChrome.vue';

export default {
  mounted() { 
  },
  components: {
    notchrome
  }
}
</script>

<style>
.mybackground {
   color: #193277 !important;
}
</style>
