<template>
  <div class="top">
    <div class="main">
      <div class="content">
        <div class="upper_content">
          <div class="lazap_features">
            <p class="one" @click="jumpTo('lightweight')" >Lightweight</p>
            <p class="two" @click="jumpTo('cross_platform')">Cross-platform</p>
            <p class="three" @click="jumpTo('game_launcher')">Game launcher</p>
          </div>
          <div class="seperating_line"></div>
          <img class="lazap_logo" src="../assets/128x128.png" alt="Lazap Icon">
          <p class="program_name">Lazap</p>
        </div>
        <div class="download">
          <a class="button" :href="lazap_latest_release_page">Get Lazap</a>
          <a class="button" href="#lightweight">Learn More</a>
        </div>
      </div>
    </div>

    <div class="lightweight" id="lightweight">
      <p class="lightweight_text">Lazap is a lightweight, cross-platform game launcher designed to provide seamless experience to gamers. Alongside being lightweight, Lazap has a minimalistic, simplistic and modernistic look. Lazap's user-friendly design makes it run smoothly and efficiently on any device. With Lazap, gamers can enjoy a minimalistic and modernistic user interface, cross-platform compatibility, and a lightweight design that ensures optimal performance.</p>
      <img class="image" src="https://source.unsplash.com/random">
    </div>

    <div class="cross_platform" id="cross_platform">
      <img class="image" src="https://source.unsplash.com/random">
      <p class="cross_platform_text">As a cross-platform game launcher, Lazap is compatible with Windows as well as Linux. Lazap's cross-platform compatibility does not hinder its performance or its lightweight experience and tries to maintain the same performance in both Windows and Linux.</p>
    </div>

    <div class="game_launcher" id="game_launcher">
      <p class="game_launcher_text">With Lazap, gamers can easily access their games that have been installed on their computer from a singular place without the hassle of loading different game launchers before deciding what to game. The app consists of a glancing and modernist UI which makes it easier for users to interact. Lazap also provides a range of customisations, such as accent color and the ability to add custom games which are not automatically detected by the launcher.</p>
      <img class="image" src="https://source.unsplash.com/random">
    </div>
  </div>
</template>

<script>
export default {
  data() {
    const lazap_latest_release_page = "https://github.com/Lazap-Development/Lazap/releases/latest"

    return {
      lazap_latest_release_page
    }
  },
  methods: {
    jumpTo(location) {
      window.location.href = `#${location}`;
    }
  }
}
</script>

<style scoped>
  @import url("@/styles/scoped/MainPage.css");
</style>