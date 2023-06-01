<template>
  <div id="homepage" class="row">
    <div class="col-sm-6">
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
      <div id="myspace-url-section" class="mb-4 mt-4">
        <strong>Myspace URL:</strong><br />
        https://www.myspace.com/genesisbelmonte
      </div>
      <interests-container />
    </div>
    <div class="col-sm-6">
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
      <p>
        In order to fall asleep, we have to pretend to be asleep. (<a
          class="blog-page-link"
          href="#"
          >view more</a
        >)
      </p>
      <p>
        Can you daydream at night? (<a class="blog-page-link" href="#"
          >view more</a
        >)
      </p>
      <p>
        Making a typo in an online argument is the equivalent of voice cracking
        in a verbal argument. (<a class="blog-page-link" href="#">view more</a>)
      </p>
      <h5 class="blurbs-header">Genesis Belmonte's Blurbs</h5>
      <h5 class="blurbs-header-title">About me:</h5>
      <p>
        I am a Software Engineer with {{ yearsExperience }} years experience
        using mainly Javascript. That includes React, React Native and Vue more
        recently. In past I have used C#, Java and some php. I've also used some
        Kubernetes, AWS, MongoDb, SQLSERVER. <br />
      </p>
      <blockquote>The best thing is 🌈✨I can learn anything✨🌈!</blockquote>
      <p>
        In my spare time I like to work on personal projects and/or hobbies, for
        example: tending to my plants, working on my app, hanging out with kids
        and husband. I am married to by bestie and we have 3 kids together. They
        are fun and pretty cool. I don't want to get rid of them yet so that
        must be a good sign, right 😉?
      </p>
      <h5 class="blurbs-header-title">Who I'd like to meet:</h5>
      <p>
        Uplifting, fun-loving, nice people. I like to go out and have fun and
        joke a lot. So anyone I had out with has to like lame jokes and be ok
        looking silly.
      </p>
      <h5 class="blurbs-header">Genesis Belmonte's Friend Space:</h5>
      <p>
        <strong
          >Genesis Belmonte has
          <span class="blurbs-header-title">the best</span> friends.</strong
        >
      </p>
      <div class="row g-1">
        <div class="col">
          <p class="myface-friend text-center">
            Carm<br />
            <img height="300" src="../assets/carmines-profile-pic.jpg" />
          </p>
        </div>
        <div class="col">
          <p class="myface-friend text-center">
            Lilian<br />
            <img height="200" src="../assets/lilians-profile-pic.jpg" />
          </p>
        </div>
        <div class="col">
          <p class="myface-friend text-center">
            Dominic<br />
            <img height="300" src="../assets/dom-profile-pic.jpeg" />
          </p>
        </div>
      </div>
      <div class="row g-1">
        <div class="col-4">
          <p class="myface-friend text-center">
            Carmine<br />
            <img height="350" src="../assets/carmine-profile-pic.jpeg" />
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
<style scoped>
.myface-friend img {
  border: #1c4ed8 solid 3px;
}

.myface-friend {
  color: #1c4ed8;
}
</style>
