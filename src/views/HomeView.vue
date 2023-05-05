<template>
  <div id="homepage" class="row">
    <div class="col-6">
      <h5><b>Genesis Belmonte</b></h5>
      <div class="col d-inline-flex">
        <img
          id="profile-pic"
          class="d-inline"
          src="../assets/profile-pic.png"
        />
        <div class="px-2 w-50">
          <small
            >"Don't cry because it's over smile because it happened."</small
          >
          <br /><br />
          <small>
            Female<br />30 years old<br />Pueblo West<br />COLORADO<br />United
            States
          </small>
          <br /><br />
          <small class="profile-pic-text">
            Last Login: {{ currentDate }}
          </small>
        </div>
        <!-- <div> -->
        <!-- </div> -->
      </div>
      <div id="under-photo-section">
        <p>
          <strong>Mood: </strong>productive 😁 <br />View My:
          <strong>
            <a class="pics-and-video-links" href="/pics">Pics</a></strong
          >
          |
          <strong>
            <a class="pics-and-video-links" href="/videos">Videos</a>
          </strong>
        </p>
      </div>
      <contacting-options />
      <div id="myface-url-section" class="mb-4 mt-4">
        <strong>Myface URL:</strong><br />
        https://www.myface.com/genesisbelmonte
      </div>
      <interests-container />
    </div>
    <div class="col">
      <div id="extended-network-banner">
        <h4>Genesis is in your extended network.</h4>
      </div>
      <p class="mt-4">
        <strong>
          Genesis Belmonte's Latest Blog Entry [<a
            class="blog-page-link"
            href="#"
            >Subscribe to this Blog</a
          >]
        </strong>
      </p>
      <p>
        If a duckling is a little duck, then a dumpling is a little dump. (<a
          class="blog-page-link"
          href="#"
          >view more</a
        >)
      </p>
      <p>
        Babies are annoying. I know. I have one. (<a
          class="blog-page-link"
          href="#"
          >view more</a
        >)
      </p>
      <h5 class="blurbs-header">Genesis Belmonte's Blurbs</h5>
      <h5 class="blurbs-header-title">About me:</h5>
      <p>
        I am a Software Engineer with {{ yearsExperience }} years experience
        using mainly Javascript. That includes React, React Native and Vue more
        recently. In past I have used C#, Java and some php. I've also used some
        Kubernetes, AWS, MongoDb, SQLSERVER. <br />The best thing is 🌈✨I can
        learn anything✨🌈!
      </p>
      <h5 class="blurbs-header-title">Who I'd like to me:</h5>
      <p>
        Praesent vitae velit libero. Ut pharetra bibendum metus nec eleifend.
        Donec a mi at ex vestibulum dictum eget sed dui. Donec a est
        fringilla,✉️ volutpat ligula nec, venenatis eros. In arcu urna,
        malesuada quis dui sit amet, interdum mollis odio. Integer in risus
        sapien. Praesent sollicitudin varius ipsum, nec malesuada felis maximus
        sed.
      </p>
      <h5 class="blurbs-header">Genesis Belmonte's Friend Space:</h5>
      <p>
        <strong
          >Genesis Belmonte has
          <span class="blurbs-header-title">a gajillion</span> friends.</strong
        >
      </p>
      <div class="row g-0">
        <div class="col">
          <p class="myface-friend">
            Friend<br />
            <img src="https://placekitten.com/200/300" />
          </p>
        </div>
        <div class="col">
          <p class="myface-friend">
            Friend<br />
            <img src="https://placekitten.com/100/100" />
          </p>
        </div>
        <div class="col">
          <p class="myface-friend">
            Friend<br />
            <img src="https://placekitten.com/200/150" />
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import InterestsContainer from "@/components/InterestsContainer.vue";
import ContactingOptions from "@/components/ContactingOptions.vue";
export default {
  components: { InterestsContainer, ContactingOptions },
  computed: {
    currentDate() {
      const today = new Date();
      const yyyy = today.getFullYear();
      let mm = today.getMonth() + 1; // Months start at 0!
      let dd = today.getDate();

      if (dd < 10) dd = "0" + dd;
      if (mm < 10) mm = "0" + mm;

      const formattedToday = mm + "/" + dd + "/" + yyyy;

      return formattedToday;
    },
    yearsExperience() {
      const today = new Date();
      const year = today.getFullYear();
      return year - 2016;
    },
  },
};
</script>
